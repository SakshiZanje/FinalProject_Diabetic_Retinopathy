# Detection of Diabetic Retinopathy

Diabetic Retinopathy is the most common diabetic eye disease. Diabetic retinopathy usually only affects people who have had diabetes (diagnosed or undiagnosed) for a significant number of years. Retinopathy can affect all diabetics and becomes particularly dangerous, increasing the risk of blindness, if it is left untreated. The risk of developing diabetic retinopathy is known to increase with age as well with less well controlled blood sugar and blood pressure level.

In this scenario, early identification of Diabetic retinopathy is more essential to recover the eyesight and provide help for timely treatment. The detection of DR is manually performed by ophthalmologists.

Ophthalmologists uses various methods to detect diabetic retinopathy but there are some drawbacks:
• It is time consuming task
• Preclinical signs are not easily detected with manual grading
• It is very expensive task

Types of Diabetic Retinopathy

Generally, diabetic retinopathy is divided into two levels:
1. Proliferative diabetic retinopathy (PDR)
2. Non-proliferative diabetic retinopathy (NPDR).

NPDR is further subdivided into
1. Mild
2. Moderate
3. Severe non-proliferative diabetic retinopathy.

# System Architecture
Figure represents our proposed system architecture. Here, In First phase I have used ATPOS 2019 kaggle dataset from which input image is taken. Then in second phase Preprocessing is done on the dataset so that training of model will imporve. In this phase various technique like cropping, resizing, conveting to gray and gaussian blur is has applied. Then in third phase of architecture feature extraction is there which includes various features like Microaneurysm, exudates, hemorrhages and blood vessesl. Here, in this phase varois features are extracted and then in fourth phase classification is done. Classification is done by detecting it has Dr or No DR.
                        ![system](https://user-images.githubusercontent.com/69428803/122645964-a6b32a00-d13a-11eb-81b8-6adc622624d9.png)


# Dataset 
I have used dataset from ATPOS 2019 kaggle challenge which contains 3662 train and 1928 test images. I have used 2929 for training 733 for testing.

This is dataset is divided into 5 classes:
CLASSES = ['0 - No DR', '1 - Mild', '2 - Moderate', '3 - Severe', '4 - Proliferative DR']

You can download this dataset from this link:
https://www.kaggle.com/c/aptos2019-blindness-detection/data

# CNN Models
1. ResNet50
2. VGG16

# Steps for the project:

1. First go through the analysis phase 
    1. Visulazing the data
    2. Image Preprocessing on the data
        1. Resizing
        2. Converting to Gray
        3. Cropping
        4. Gaussian Blur

2. Second, Go through process_2 phase
    1. Do data splitting making for ready for training.
    2. Do preprocessing on the data set and saving it to another folder.
  
3. Third, for training go through DR_colab phase
    1. For training i have used google colab
