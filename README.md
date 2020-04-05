# [Does Imagenet Pretraining work for Chest Radiography Images(COVID-19)?](https://deep-and-shallow.com/2020/04/05/does-imagenet-pretraining-work-for-chest-radiography-imagescovid-19/)

[This is the supplementary repository for the blog post of the same name.](https://deep-and-shallow.com/2020/04/05/does-imagenet-pretraining-work-for-chest-radiography-imagescovid-19/)

In this repository, we explore the suitability of Imagenet Pretraining for Chast Radiography Images, specifically in the COVID-19 context.

**Disclaimer:** The pretrained models provided here are intended to be used as reference models that can be built upon and enhanced as new data becomes available. They are currently at a research stage and not yet intended as production-ready models (not meant for direct clinicial diagnosis). Please do not use these models for self-diagnosis and seek help from your local health authorities.

Inspired by the work that came out of University of Waterloo, Canada by Linda Wang and Alexander Wong titled, [COVID-Net: A Tailored Deep Convolutional Neural Network Design for Detection of COVID-19 Cases from Chest Radiography Images](https://github.com/lindawangg/COVID-Net). 

We apply ImageNet pretrained models to the problem to study the suitability.
## Dataset 
[COVID-Net](https://github.com/lindawangg/COVID-Net) introduced a  chest radiography dataset, called COVIDx.  It is comprised of 16,756 chest radiography images across 13,645 patient cases from two open access data repositories.
The current COVIDx dataset is constructed by the following open source chest radiography datasets:

-   [https://github.com/ieee8023/covid-chestxray-dataset](https://github.com/ieee8023/covid-chestxray-dataset)
-   [https://www.kaggle.com/c/rsna-pneumonia-detection-challenge](https://www.kaggle.com/c/rsna-pneumonia-detection-challenge)
![This image has an empty alt attribute; its file name is train-set.png](https://deepandshallowml.files.wordpress.com/2020/04/train-set.png?w=1024)
![This image has an empty alt attribute; its file name is train-set.png](https://deepandshallowml.files.wordpress.com/2020/04/train-set.png?w=1024)
# Training
1. DenseNet - covid_fastai_densenet_121_training.ipynb
2. Xception - covid_fastai_xception_training.ipynb

# Pre-Trained Models
Place the models in saved_models folder before running the inference notebooks
[DenseNet 121](https://drive.google.com/open?id=1Fqt9QH34wjxXW-n3FD3NdsokBxj6Duxb)
[Xception](https://drive.google.com/open?id=1TGhBuVW6-DtU4REO14VWERpQZVs2_9cG)
# Results
![This image has an empty alt attribute; its file name is image-12.png](https://deepandshallowml.files.wordpress.com/2020/04/image-12.png?w=956)

# GradCAM
![This image has an empty alt attribute; its file name is image-16.png](https://deepandshallowml.files.wordpress.com/2020/04/image-16.png?w=895)

# t-SNE Feature Representation

![This image has an empty alt attribute; its file name is image-24.png](https://deepandshallowml.files.wordpress.com/2020/04/image-24.png?w=855)