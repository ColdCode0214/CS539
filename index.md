# CS539-COVID CT CLASSIFICATION

Github Link: https://colab.research.google.com/drive/1UxfVkl6cqcn0gnZqFF3gj36UOqfXXQCz#scrollTo=nPBxMYePSnX0

## Background & Motivation

Our project is to find a set of models and parameters that would give precise predictions about a patient’s health situation: whether he/she is healthy, has been infected by COVID-19 or has been experiencing normal pneumonia.

Our models could potentially help doctors diagnose COVID-19 patients given lung CT scans. Our models are also useful for distinguishing COVID patients from normal pneumonia patients.

## Data

The orginial dataset contains 75000 images. We trained on our dataset containing 15000 images.

There are 5000 images for each category: COVID, Pneumonia, Normal.

Here are three sample images from different categories:

<p>
  <img src="assets/CP_595_2957_0048.png" alt="covid" width="250"/>
</p>
<p>
  <em>COVID Lungs</em>
</p>
<p>
  <img src="assets/NCP_270_1687_0019.png" alt="pneumonia" width="250"/>
</p>
<p>
  <em>Pneumonia Lungs</em>
</p>
<p>
  <img src="assets/Normal_805_240_0109.png" alt="normal" width="250"/>
</p>
<p>
  <em>Normal Lungs</em>
</p>

## Network

We used 6 different models to train the dataset. The three main networks are VGG, ResNet and DenseNet.

## Very Deep Convolutional Network (VGG)

### VGG16

<p>
  <img src="https://neurohive.io/wp-content/uploads/2018/11/vgg16-1-e1542731207177.png" alt="vgg16" width="500"/>
</p>

**VGG16** is a convolutional neural network model proposed by K. Simonyan and A. Zisserman from the University of Oxford in the paper “Very Deep Convolutional Networks for Large-Scale Image Recognition”. It was one of the famous model submitted to ILSVRC-2014. It makes the improvement over AlexNet by replacing large kernel-sized filters (11 and 5 in the first and second convolutional layer, respectively) with multiple 3×3 kernel-sized filters one after another.

### VGG19

**VGG19** is a convolutional neural network that is 19 layers deep.

<p>
  <img src="https://neurohive.io/wp-content/uploads/2018/11/Capture-564x570.jpg" alt="vgg19" width="500"/>
</p>

## Deep Residual Neural Network (ResNet)

### ResNet101

A **residual neural network (ResNet)** is an artificial neural network (ANN) of a kind that builds on constructs known from pyramidal cells in the cerebral cortex. Residual neural networks do this by utilizing skip connections, or shortcuts to jump over some layers. Typical ResNet models are implemented with double- or triple- layer skips that contain nonlinearities (ReLU) and batch normalization in between.

<p>
  <img src="https://neurohive.io/wp-content/uploads/2019/01/resnet-570x328.png" alt="resnet" width="500"/>
</p>

### ResNet152

**ResNet152** has a depth of 152 layers.

<p>
  <img src="https://miro.medium.com/max/1000/1*2ns4ota94je5gSVjrpFq3A.png" alt="resnet152" width="500"/>
</p>

## Densely Connected Convolutional Networks (DenseNet)

### DenseNet161

A **DenseNet** is a type of convolutional neural network that utilises dense connections between layers, through Dense Blocks, where we connect all layers (with matching feature-map sizes) directly with each other. To preserve the feed-forward nature, each layer obtains additional inputs from all preceding layers and passes on its own feature-maps to all subsequent layers.

<p>
  <img src="https://user-images.githubusercontent.com/92838953/146097211-fde3c669-0042-40fd-aacf-e2367c7198dd.png" alt="densenet" width="500"/>
</p>


### DenseNet201

**DenseNet201** has a depth of 201 layers

<p>
  <img src="https://user-images.githubusercontent.com/92838953/146097292-5540faeb-eba1-45cc-acc2-b73166e3c708.png" alt="densenet201" width="500"/>
</p>


## Result

Training Loss : 0.0007
<p>
  <img src="assets/train_loss.png" width="500"/>
</p>


Training Accuracy : 99.9733%
<p>
  <img src="assets/train_accu.png" width="500"/>
</p>

Validation Loss : 0.6512
<p>
  <img src="assets/val_loss.png" width="500"/>
</p>


Validation Accuracy : 81.0667%
<p>
  <img src="assets/val_accu.png" width="350"/>
</p>

Prediction Rate by Categories
<p>
  <img src="assets/prediction.png" width="500"/>
</p>

Confusion matrix, without normalization
<p>
  <img src="https://user-images.githubusercontent.com/90018380/145900795-70b5ce75-148c-4b67-a0b8-32245ac99aae.png" width="500"/>
</p>
MACRO-averaged: prediction= 86.32 %,recall= 81.07 %,f1= 83.61

## Team

Yan Zhang

Zeyu Hu

Chang Liu

Jiani Wang

Ziyang Xu

## References

https://www.nature.com/articles/s41598-021-93832-2

https://neurohive.io/en/popular-networks/vgg16/

https://en.wikipedia.org/wiki/Residual_neural_network

https://paperswithcode.com/method/densenet
