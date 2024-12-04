# Cervical-Cancer-Detection-using-Python 🩺💻

# Objective: 🎯
This project, developed as part of my capstone work, focuses on classifying cervical cell images into five distinct classes taken from SIPaKMeD database. It involves preprocessing techniques and the application of advanced deep learning models to compare their performance. The project utilizes SLIC-based superpixel segmentation and Canny edge detection for preprocessing cervical cell images, enhancing feature extraction. Several pre-trained convolutional neural network (CNN) models were fine-tuned and evaluated to determine the best-performing model for this task.

**Models Evaluated:** 🤖
1. ResNet50: It is a deep CNN architecture that uses residual learning to help train deeper networks. It includes 50 layers, and the key feature of ResNet is the use of skip connections or residual connections to mitigate the vanishing gradient problem, making it easier to train very deep networks. ResNet50 is known for its effectiveness in image classification tasks and has been widely used in computer vision due to its high performance and depth.
  
2. VGG16: It is a deep CNN architecture known for its simplicity and effectiveness. It uses a series of 16 layers (13 convolutional layers and 3 fully connected layers) with small 3x3 filters and a uniform architecture. VGG16 was one of the first models to show that very deep networks could perform well, even with simple design principles. It is often used for transfer learning due to its strong generalization ability on image recognition tasks.
  
3. InceptionV3: It is a deep CNN architecture that improves upon the original Inception network. It employs Inception modules, which are designed to handle multiple filter sizes at each layer, allowing the model to capture features at different scales. InceptionV3 is optimized for computational efficiency and achieves high accuracy on image classification tasks. It is widely recognized for its model size and speed, making it suitable for both high-performance and resource-constrained environments.
  
4. EfficientNetB0: It is part of the EfficientNet family, which is designed to optimize both accuracy and efficiency. It uses a compound scaling method that uniformly scales the depth, width, and resolution of the network, balancing these aspects to achieve state-of-the-art performance with fewer parameters. EfficientNetB0 is the smallest model in the EfficientNet series and is known for delivering high accuracy with low computational cost, making it ideal for tasks requiring resource efficiency.

5. EfficientNetB7: It is the largest and most accurate model in the EfficientNet family. Like EfficientNetB0, it uses the compound scaling method to balance network depth, width, and resolution. EfficientNetB7 achieves state-of-the-art accuracy on image classification tasks, albeit at a higher computational cost than EfficientNetB0.

6. MobileNetV2: It is a lightweight CNN architecture designed for mobile and edge devices. It uses depthwise separable convolutions to reduce computation and memory requirements. MobileNetV2 introduces inverted residuals and linear bottlenecks to improve efficiency while maintaining accuracy. It is widely used for image classification and transfer learning in resource-constrained environments.

7. MobileNetV3: It is an improvement over MobileNetV2, leveraging techniques such as NAS (Neural Architecture Search) to optimize for both speed and accuracy. MobileNetV3Large is designed for high-accuracy tasks, balancing resource efficiency with enhanced performance.
   
**Classification classes:** 📊
1. Diskeratotic cells: They are squamous cells which undergone premature abnormal keratinization within individual cells or more often in three-dimensional clusters. They exhibit a brilliant orangeophilic cytoplasm. They are characterized by the presence of vesicular nuclei, identical to the nuclei of koilcytotic cells. In many cases there are binucleated and/or multinucleated cells.
  
2. Koilocytotic cells: These cells correspond most commonly in mature squamous cells (intermediate and superficial) and some times in metaplastic type koilocytotic cells. They appear most often cyanophilic, very lightly stained and they are characterized by a large perinuclear cavity. The periphery of the cytoplasm is very dense stained. The nuclei of koilocytes are usually enlarged, eccentrically located, hyperchromatic and exhibit irregularity of the nuclear membrane contour.
  
3. Metaplastic cells: They are in essence small or large parabasal-type cells with prominent cellular borders, often exhibiting eccentric nuclei and sometimes containing a large intracellular vacuole. The staining in the center portion is usually light brown and it often differs from that in the marginal portion. Also, there is essentially a darker-stained cytoplasm and they exhibit great uniformity of size and shape compared to the parabasal cells, as their characteristic is the well defined, almost round shape of cytoplasm.
  
4. Parabasal cells: Parabasal cells are immature squamous cells and they are the smallest epithelial cells seen on a typical vaginal smear. The cytoplasm is generally cyanophilic and they usually contain a large vesicular nucleus. It must be noted that parabasal cells have similar morphological characteristic with the cells identified as metaplastic cells and it is difficult to be distinguished from them.
  
5. Superficial-Intermediate cells: They constitute the majority of the cells found in a Pap test. Usually they are flat with round, oval or polygonal shape cytoplasm stains mostly eosinophilic or cyanophilic. They contain a central pycnotic nucleus. They have well defined, large polygonal cytoplasm and easily recognized nuclear limits (small pycnotic in the superficial and vesicular nuclei in intermediate cells). These type of cells show the characteristics morphological changes (koilocytic atypia) due to more severe lessions.

# Dataset: 📂
The SIPaKMeD Database consists of 4049 images of isolated cells that have been manually cropped from 966 cluster cell images of Pap smear slides. These images were acquired through a CCD camera adapted to an optical microscope. The cell images are divided into five categories containing normal, abnormal and benign cells. This dataset is a subset of the SIPaKMeD. Only the single-cell images are rearranged for purpose of experiment. 

The original dataset can be found here - https://www.cs.uoi.gr/~marina/sipakmed.html.

You can find the dataset on Kaggle [here](https://www.kaggle.com/datasets/mohaliy2016/papsinglecell)

The dataset comprises cervical cell images divided into training and testing subsets:

- Training Data: 3549 Pre-labeled images organized into five classes.
- Testing Data: 500 Unseen data for evaluating model performance.

The SIPaKMeD database is publicly available and it can be used for experimental purposes with the request to cite the paper. It can be sited as follows,

Plissiti, M. E., Dimitrakopoulos, P., Sfikas, G., Nikou, C., Krikoni, O., & Charchanti, A. (2018, October). Sipakmed: A new dataset for feature and image based classification of normal and pathological cervical cells in pap smear images. In 2018 25th IEEE international conference on image processing (ICIP) (pp. 3144-3148). IEEE.

# Results: 📈
The performance of the models was compared based on accuracy, precision, recall and f1-score.




📍 EfficientNetB0 demonstrated the best performance, achieving the highest accuracy and macro ROC-AUC scores.

📍 The preprocessing steps involving SLIC and Canny significantly improved the models' ability to differentiate between classes, as demonstrated by strong separability metrics (ROC-AUC > 0.90 for all classes).

# 
Languages used : 

![python-logo-only](https://github.com/user-attachments/assets/a78aa447-fe92-4892-aaed-4dd6ea761795)

# 
📣 Feel free to have a look at all the files in this repository !🤗

❎ In case you find issues in any of my Repositories, you can Hit Me Up [here](https://github.com/issues)! 👈


