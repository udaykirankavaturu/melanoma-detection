# Melanoma Detection using CNN
To build a CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

## General Information
Objective is to build a multiclass classification model using a custom convolutional neural network in TensorFlow. 

The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, with the exception of melanomas and moles, whose images are slightly dominant.

The data set contains the following diseases:

    Actinic keratosis
    Basal cell carcinoma
    Dermatofibroma
    Melanoma
    Nevus
    Pigmented benign keratosis
    Seborrheic keratosis
    Squamous cell carcinoma
    Vascular lesion


## Conclusions

A regular CNN overfitted and was not able to do well on the validation dataset. 

Data augmentation technique to randomly rotate and flip the images helped the model to learn better and reduced overfitting. But there was still room for improvement. 

It was noticed that the dataset displayed class imbalance i.e., some classes were dominating their presence in the dataset while others were in smaller numbers. 

Augmentor module was used to create a pipeline and produce 500 images per class to avoid the class imbalance issue. 

Model showed promise with 20 epochs on the new dataset. 

Model further showed greater accuracy above 85% when ran with 50 epochs. 


## Technologies Used
- tensorflow
- matplotlib
- numpy
- pandas


## Contact
Created by [@udaykirankavaturu](https://github.com/udaykirankavaturu/melanoma-detection) - feel free to contact me!