
# Facial Expression Recognition

Training a Deep Neural Net for Facial Expression Recognition

Kaggle Notebook ->  https://www.kaggle.com/nakulsingh1289/face-expression-detection-from-scratch

### Dataset
https://www.kaggle.com/jonathanoheix/face-expression-recognition-dataset 

## Deployment

Currently the model can be deployed or tested through opencv for 
Face Expression Recognition in the backend of the applications.

### File structure

**expression_recognition_model.ipynb** Contains code for the architecture of the model
along with the training of the model

**openCV real time face expression.ipynb**  Contains code for the deployment 
of trained model using openCV and webcam

**data/xyz/haarcascade_frontalface_default.xml** : model used for face detection

**data/xyz/model_weights.h5** : trained model weights

**data/xyz/model.json** : Architecture of model




  
## Libraries

**Language:** Python 

**Libraries and Frameworks:** Keras, numpy, openCV, matplotlib, seaborn, os, tensorflow

![App Screenshot](https://github.com/nakulsingh1289/Projects/blob/master/Expression%20Recognition/result.png)

### Architecture of Model 

  
conv2d (Conv2D)              (None, 48, 48, 64)        640       
_________________________________________________________________
batch_normalization (BatchNo (None, 48, 48, 64)        256       
_________________________________________________________________
activation (Activation)      (None, 48, 48, 64)        0         
_________________________________________________________________
max_pooling2d (MaxPooling2D) (None, 24, 24, 64)        0         
_________________________________________________________________
dropout (Dropout)            (None, 24, 24, 64)        0         
_________________________________________________________________
conv2d_1 (Conv2D)            (None, 24, 24, 128)       204928    
_________________________________________________________________
batch_normalization_1 (Batch (None, 24, 24, 128)       512       
_________________________________________________________________
activation_1 (Activation)    (None, 24, 24, 128)       0         
_________________________________________________________________
max_pooling2d_1 (MaxPooling2 (None, 12, 12, 128)       0         
_________________________________________________________________
dropout_1 (Dropout)          (None, 12, 12, 128)       0         
_________________________________________________________________
conv2d_2 (Conv2D)            (None, 12, 12, 512)       590336    
_________________________________________________________________
batch_normalization_2 (Batch (None, 12, 12, 512)       2048      
_________________________________________________________________
activation_2 (Activation)    (None, 12, 12, 512)       0         
_________________________________________________________________
max_pooling2d_2 (MaxPooling2 (None, 6, 6, 512)         0         
_________________________________________________________________
dropout_2 (Dropout)          (None, 6, 6, 512)         0         
_________________________________________________________________
conv2d_3 (Conv2D)            (None, 6, 6, 512)         2359808   
_________________________________________________________________
batch_normalization_3 (Batch (None, 6, 6, 512)         2048      
_________________________________________________________________
activation_3 (Activation)    (None, 6, 6, 512)         0         
_________________________________________________________________
max_pooling2d_3 (MaxPooling2 (None, 3, 3, 512)         0         
_________________________________________________________________
dropout_3 (Dropout)          (None, 3, 3, 512)         0         
_________________________________________________________________
flatten (Flatten)            (None, 4608)              0         
_________________________________________________________________
dense (Dense)                (None, 256)               1179904   
_________________________________________________________________
batch_normalization_4 (Batch (None, 256)               1024      
_________________________________________________________________
activation_4 (Activation)    (None, 256)               0         
_________________________________________________________________
dropout_4 (Dropout)          (None, 256)               0         
_________________________________________________________________
dense_1 (Dense)              (None, 512)               131584    
_________________________________________________________________
batch_normalization_5 (Batch (None, 512)               2048      
_________________________________________________________________
activation_5 (Activation)    (None, 512)               0         
_________________________________________________________________
dropout_5 (Dropout)          (None, 512)               0         
_________________________________________________________________
dense_2 (Dense)              (None, 7)                 3591      

Total params: 4,478,727
Trainable params: 4,474,759
Non-trainable params: 3,968
_________________________________________________________________
  
