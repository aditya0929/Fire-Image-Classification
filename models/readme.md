# FIRE IMAGE CLASSIFICATION

![image](https://github.com/aditya0929/Fire-Image-Classification/assets/127277877/312e9c76-39c8-415a-9488-059faffab33b)

## SOCIAL SUMMER OF CODE 2023

The models that i have created are based on the approach for making a Deep Learning Model which deals with mutli isntance image classification as in the dataset selected we had four classes of images:-

1. `fire_images`
2. `non_fire_images`

## Important note:-
**for all the three models that i have created, the parts excluding the model architecture and its definition are mostly the same for the accuracy result to be based out on the same parameters.**


# Approach for Multi-Instance Image Classification

**1. Importing important libaries**

**2. Loading the datasets and creating image and label list for each category** 

**3. Division of train test ad split of the dataset**

**4. Data preprocessing and Image data generators**

**5. Division for images in training , testing and validation categories**

**6. Making of the models**

**A. MOBILENET**
     
     
     Implementing MobileNet architecture using Keras. 
     MobileNet is a lightweight convolutional neural network architecture designed for mobile and embedded vision applications.
     It defines a sequential model and sequential layers are added to construct the MobileNet architecture
     
     The desired input image size is (224x224x3)  MobileNet model is initialized as the base model. 
     This include_top=False argument to ensure that the top classification layer of the MobileNet model is excluded.
     
     After the convolutional layers, output is flattened and fully connected layers with dropout for regularization are added  
     
     Finally, the model ends with an output layer using softmax activation for multi-class classification.
     
     the model is compiled by specifying the loss function, optimizer, and evaluation metrics.
     
     The model is trained using the fit() function with provided training and validation datasets

  
   **B. ResNet50V2**
   
   
    The ResNet50V2 model is pre-trained on the ImageNet dataset and is used as a feature extractor.
    A sequential model is created. The base ResNet50V2 model is added as the first layer. 
    
    Global average pooling is applied to reduce the spatial dimensions of the output.
    Dropout layers are introduced to mitigate overfitting. 
    
    Two dense layers with ReLU activation are added, followed by a final dense layer with 
    softmax activation for multi-class classification.
   
    the model is compiled by specifying the loss function, optimizer, and evaluation metrics.
    
    the model is trained usinf the fit() function to the training data (train_images)

      
   **B. VGG19**
   
   
    -The VGG16 model is a deep convolutional neural network that has been pre-trained on the ImageNet dataset. 
    -Fine-tuning involves taking the pre-trained model and adapting it to a new task or 
     dataset by training the top layers while keeping the lower layers frozen.
    -Load the pre-trained VGG16 model
    -Freeze the layers in the base model
    -Add custom top layers
    -Create the fine-tuned model
    -Compile the model
    -Train the model

    
  **7.Training and Validation Metrics Visualization**
 
 
    plotting graphs showing 
    training loss,
    training accuracy,
    
   
    
**8.  Model prediction and evaluation**

**9.  Finally, Training and Validation Metrics Visualization**

**10. Accuracy Evaluation and Confusion Matrix**

**11. Additionally , the model architecture can also be visualized .**

### Learning resources  

  
  1.[Transfer Learning using mobilenet and keras](https://medium.com/towards-data-science/transfer-learning-using-mobilenet-and-keras-c75daf7ff299)
  
  2.[cnn-architectures](https://medium.com/@RaghavPrabhu/cnn-architectures-lenet-alexnet-vgg-googlenet-and-resnet-7c81c017b848)
  
  3.[how to build your own neural network](https://medium.com/towards-data-science/how-to-build-your-own-neural-network-from-scratch-in-python-68998a08e4f6)
  
  4.[cnn- deep learning](https://medium.com/@RaghavPrabhu/understanding-of-convolutional-neural-network-cnn-deep-learning-99760835f148)
  
  5.[ResNet50V2](https://medium.com/towards-data-science/build-a-custom-resnetv2-with-the-desired-depth-92892ec79d4b)
  

 ### GITHUB LINK - https://github.com/aditya0929
