<h1 align="center">GreenDetect</h1>
This is a ResNet50-based model for plant disease detection. It employs transfer learning, data augmentation and class balancing to handle imbalanced datasets. The model processes images efficiently, achieving accurate classification of healthy and diseased plants.

## Execution Guide:
1. Run the following command line in the terminal:
   ```
   pip install tensorflow numpy matplotlib scikit-learn
   ```
   
2. Download the dataset (link to the dataset: **https://drive.google.com/file/d/1kA_JWhHQhyzzuzlpzppK2nNTtbiR2N77/view**)

3. Copy and paste the path in the code

4. After running all the cells, in the last cell enter the path of the plant image you want to run the model on

## Accuracy & Loss Over Epochs

![image](https://github.com/user-attachments/assets/57b7c79b-cf37-4669-bf05-7bc9b518712d)

![image](https://github.com/user-attachments/assets/23e5416c-90d1-4dcd-8dc8-02a9c4b0aed1)

## Model Prediction:

   ![image](https://github.com/user-attachments/assets/19dbb952-82fc-4adb-89a2-8bb8f847842f)

   ![image](https://github.com/user-attachments/assets/dc156ce4-8537-40f3-b509-eada91fb8141)

## Overview:
This project focuses on detecting plant diseases using a convolutional neural network (CNN) based on the **ResNet50 architecture**. The model is designed to identify whether a plant is healthy or diseased from input images.  

#### Key Features:  
1. **Transfer Learning:** A pre-trained ResNet50 model is used as the base, leveraging its learned features to improve performance on the plant disease dataset.  

2. **Custom Architecture:** Additional layers are added on top of ResNet50, including a global average pooling layer, dense layers, and a dropout layer for better generalization.  

3. **Data Augmentation:** The training dataset undergoes augmentation (e.g., rotation, flipping, zooming) to increase diversity and improve robustness.  

4. **Class Balancing:** Class weights are calculated to handle imbalanced data, ensuring the model doesn’t favor one class over the other.  

5. **Efficient Processing:** Images are preprocessed and resized to 224x224, ensuring compatibility with ResNet50 while maintaining computational efficiency.  

6. **Binary Classification:** The model outputs a sigmoid activation, classifying images as either “Healthy” or “Diseased.”  

#### Performance:  
- **Validation Accuracy:** Achieves 88.89%, demonstrating strong capability in distinguishing between healthy and diseased plants.  
- **Loss Trends:** Training and validation loss/accuracy curves indicate consistent learning and minimal overfitting.  

This model provides a reliable solution for plant health monitoring, aiding farmers and agricultural industries in early disease detection and crop management.
