
# Rock Paper Scissor Dectector

Trained a deep neural net which can dectect hand gesture of rock, paper and scissor


## Deployment

The project currently is deployed and tested using openCV via webcams or images.

## Demo

![App Screenshot](https://github.com/nakulsingh1289/Projects/blob/master/Rock%20Paper%20Scissors%20with%20AI%20using%20keras%20and%20openCV/demo.jpeg)
  
## Tools & Libraries Used  

**Language** Python

**Libraries and FrameWorks:** Keras, Numpy, Matplotlib, OpenCV, Time

## Dataset Used
https://www.kaggle.com/frtgnn/rock-paper-scissor

Number of images in  train-set: 2520

Number of images in the test-set: 2520

Number of rocks in the train-set: 840 

Number of papers in the train-set: 840

Number of scissors in the train-set: 840

Number of rocks in the test-set: 840

Number of papers in the test-set: 840

Number of scissors in the test-set: 840

## Model Architecture

Convolution Layer (None, 75, 75, 64)

MaxPooling2 Layer (None, 37, 37, 64)

Convolution Layer (None, 37, 37, 64) 

MaxPooling2 Layer (None, 18, 18, 64)  

Convolution Layer (None, 18, 18, 128)  

MaxPooling2 Layer (None, 9, 9, 128) 

Convolution Layer (None, 9, 9, 128)

MaxPooling2 Layer (None, 4, 4, 128)

Flatten Layer      (None, 2048)  

Dense Layer       (None, 512)

Dropout   (0.2)        (Node, 512)

### CallBacks 
 EarlyStopping(monitor='val_accuracy', patience=5, verbose=1)

  ReduceLROnPlateau(monitor='val_accuracy', pateince=2, factor=0.5, min_lr=0.00001, verbose=1)

  ModelCheckpoint("model.h5",monitor='val_accuracy', save_best_only=True, verbose=1, mode='max')

  


  
