# Face-Mask-Detection

This project is the face-mask detection with `InceptionV3 model` using the `imagenet` weights.

`Training-Model.ipynb` is the model training file with face mask dataset from kaggle.
  
The dataset can be downloaded from `https://www.kaggle.com/datasets/ashishjangra27/face-mask-12k-images-dataset`.


### Training Process
Firstly, load the dataset and preprocess with data augmentation.

Then load the model with pretrained weights. I use "mixed7" layer and add some dense layers and
dropout for regularization.

Model Checkpointing and callback are also used to avoid overfitting.


### Model Inferencing

In the model inferencing part, web cam is used for live detection.
