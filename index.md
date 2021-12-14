# CS539-COVID CT CLASSIFICATION

Team Member: Yan Zhang, Zeyu Hu, Jiani Wang, Chang Liu, Ziyang Xu

Github Link: https://colab.research.google.com/drive/1UxfVkl6cqcn0gnZqFF3gj36UOqfXXQCz#scrollTo=nPBxMYePSnX0

## Background & Motivation

Our project is to find a set of models and parameters that would give precise predictions about a patient’s health situation: whether he/she is healthy, has been infected by COVID-19 or has been experiencing normal pneumonia.


```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [Basic writing and formatting syntax](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).

## Data

The orginial dataset contains 75000 images. We trained on dataset containing 15000 images.

There are 5000 images for each label. Here are sample images from the training set:

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

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.

## Very Deep Convolutional Network (VGG)

### VGG16

<p>
  <img src="https://neurohive.io/wp-content/uploads/2018/11/vgg16-1-e1542731207177.png" alt="vgg16" width="350"/>
</p>

**VGG16** is a convolutional neural network model proposed by K. Simonyan and A. Zisserman from the University of Oxford in the paper “Very Deep Convolutional Networks for Large-Scale Image Recognition”. It was one of the famous model submitted to ILSVRC-2014. It makes the improvement over AlexNet by replacing large kernel-sized filters (11 and 5 in the first and second convolutional layer, respectively) with multiple 3×3 kernel-sized filters one after another.

### VGG19

## Deep Residual Neural Network (ResNet)

### ResNet101

### ResNet152

## Densely Connected Convolutional Networks (DenseNet)

### DenseNet161

### DenseNet201



## Result

![image](https://user-images.githubusercontent.com/90018380/145900795-70b5ce75-148c-4b67-a0b8-32245ac99aae.png)


## Team


## Reference
https://www.kaggle.com/itkang/covidct-2a
https://www.kaggle.com/hgunraj/covidxct
https://www.nature.com/articles/s41598-021-93832-2
https://neurohive.io/en/popular-networks/vgg16/
