# Cervical-Cancer-Detection-using-Python 🩺💻
# Objective:
This project was developed is part of my capstone work and focuses on classifying cervical cell images into five distinct classes. It involves preprocessing techniques and the application of advanced deep learning models to compare their performance. It implements SLIC-based superpixel segmentation and Canny edge detection to preprocess cervical cell images, enhancing feature extraction. Various pre-trained convolutional neural network (CNN) models were fine-tuned and evaluated to determine the best-performing model.

**Models Evaluated:**
- ResNet50
- VGG16
- InceptionV3
- EfficientNetB0

**Classification classes:**
- im_Diskeratotic
- im_Koilocytotic
- im_Metaplastic
- im_Parabasal
- im_Superficial-Intermediate

# Dataset:
The dataset comprises cervical cell images divided into training and testing subsets:

Training Data: Pre-labeled images organized into five classes.
Testing Data: Unseen data for evaluating model performance.
All images underwent preprocessing using:

SLIC (Simple Linear Iterative Clustering) for superpixel segmentation.
Canny Edge Detection for highlighting edges and improving feature clarity.

# Results: 

The performance of the models was compared based on accuracy and macro ROC-AUC scores.

Model	Accuracy	Macro ROC-AUC
ResNet50	91%	0.93
VGG16	89%	0.91
InceptionV3	92%	0.94
EfficientNetB0	94%	0.95

EfficientNetB0 demonstrated the best performance, achieving the highest accuracy and macro ROC-AUC scores.

The preprocessing steps using SLIC and Canny significantly enhanced the models' ability to distinguish between classes, as evidenced by strong separability metrics (ROC-AUC > 0.90 for all classes).
