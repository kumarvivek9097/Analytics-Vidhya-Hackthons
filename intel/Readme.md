# Intel Scene Classification Competition
## Problem Statement 
To identify which kind of scene can the image be categorized into.

## Approach
- Participate in discussion forum
- Learn image recognition concept - CNN, Transfer Learning
- Build and improve the model

## Model
- Dataset  
There are 17034 images in train and 7301 images in test data. The categories of scenes and their corresponding labels in the dataset are 
'buildings' -> 0
'forest' -> 1
'glacier' -> 2
'mountain' -> 3
'sea' -> 4
'street' -> 5

- CNN 
A three layer convolutional network with relu & sigmoid activation function, uniform kernel initializer, a dropout of 0.3, 0.4 & 0.2 at each layer and a final dense layer with softmax activation was built. Model was compiled with categorical_crossentropy loss function , adam optimizer and accuracy performance matric . The model was trained for 30 epoch with batch size 128.


- Transfer Learning
A VGG16 with imagenet weight based transfer learning was used. After feature extraction from the model, a dense layer with softmax function was built to classify images into desired categories.
