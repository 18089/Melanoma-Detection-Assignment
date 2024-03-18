# Melanoma Detection Assignment
> Problem Statement
> To build a CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution which can evaluate images and alert the dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.


<!-- You can include any other section that is pertinent to your problem -->

## General Information
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
 

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
1. **Overfitting and Imbalanced Data:**

    Overfitting tends to occur notably when the dataset is imbalanced.
    Models trained on imbalanced data exhibit varied behaviors:
    Model.1: Shows underfitting with low training and validation accuracies.
  
    Model.2 and Model.3: Exhibit clear signs of overfitting with high training accuracies but significantly lower validation accuracies.
  
    Model.3 incorporates an additional dropout layer but still demonstrates overfitting, suggesting that tweaking dropout factors or adding more layers might mitigate overfitting to some extent.
  
    Model.4 shows decent performance with intermediate dropout layers, indicating that adding more layers with additional dropout layers might not significantly enhance performance but can reduce training time.

2. **Impact of Data Augmentation:**

    Augmentation helps in balancing the dataset, mitigating the effects of imbalance.
  
    Model.4, when trained on augmented data, shows improved performance:
    Training accuracy remains high at above 92%.
    Validation accuracy significantly improves to 88%.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
pathlib - version 1.0.1
tensorflow - version 2.15.0
pandas - version 1.5.3
numpy - version 1.24.3
pillow - version 10.2.0
glob - version 0.7
matplotlib - version 3.7.1
Augmentor - version 0.2.12

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->



<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->
