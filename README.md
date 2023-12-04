# Melanoma Detection using Custom CNN model.

## Table of Contents
* [Problem Statement](#problem-statement)
* [Dataset](#dataset)
* [Conclusions](#conclusions)
* [Technologies Used](#technologies-used)
* [Contact](#contact)

### Problem Statement
To build a CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.

## Dataset 
The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, with the exception of melanomas and moles, whose images are slightly dominant. The dataset contains the following classes - 

The data set contains the following diseases:
- Actinic keratosis
- Basal cell carcinoma
- Dermatofibroma
- Melanoma
- Nevus
- Pigmented benign keratosis
- Seborrheic keratosis
- Squamous cell carcinoma
- Vascular lesion

## Conclusions
Final model performance
- Training accuracy: `0.9293`
- Validation accuracy: `0.8693`
- Training loss: `0.1717`
- Validation loss: `0.4156` 
- Predicts 6 of 9 classes on the holdout dataset correctly.
    - ✔ Actual Class: actinic keratosis | Predicted Class: actinic keratosis
    - ✔ Actual Class: basal cell carcinoma | Predicted Class: basal cell carcinoma
    - ❌ Actual Class: dermatofibroma | Predicted Class: pigmented benign keratosis
    - ✔ Actual Class: melanoma | Predicted Class: melanoma
    - ❌ Actual Class: nevus | Predicted Class: pigmented benign keratosis
    - ✔ Actual Class: pigmented benign keratosis | Predicted Class: pigmented benign keratosis
    - ❌ Actual Class: seborrheic keratosis | Predicted Class: melanoma
    - ✔ Actual Class: squamous cell carcinoma | Predicted Class: squamous cell carcinoma
    - ✔ Actual Class: vascular lesion | Predicted Class: vascular lesion

## Technologies Used
Trained using docker image from colab on a local GPU. <br> 
Image: `us-docker.pkg.dev/colab-images/public/runtime` <br>
Libaries used:
- Numpy - `1.23.5`
- Matplotlib - `3.7.1`
- Augmentor - `0.2.12`
- PIL - `9.4.0`
- tensorflow - `2.13.0`
- keras - `2.13.1`


## Contact
> Sudarshan | sudarshan_g@outlook.com
