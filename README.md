The code was developed based on Starting Kit provided Areal Team. 

# Aerial-Image-Recognition
The competition is hosted on https://competitions.codalab.org/competitions/27749#learn_the_details-overview


The data set contains 9100 color images of size 128 x 128, images of 13 class, each having 700 images.
The classes are some kind of landscape or a natural environment, and more specifically :
beach, chaparral, cloud, desert, forest, island, lake, meadow, mountain, river, sea_ice, snowberg, wetland.

The goal of this challenge will be to classify each image and assign to it the correct label.

![img](https://raw.githubusercontent.com/ArealTeamM2AIC/Remote-Sensing-Image/dev_final/starting_kit/sample_images/sample_images.png)

### Literature review

In Section3 of a very comprehensive review of 
[Remote Sensing Image Scene Classification Meets Deep Learning: Challenges, Methods, Benchmarks,and Opportunities](https://arxiv.org/abs/2005.01094)
listed that deep learning based scene classification algorithms can be broadly divided
into three main categories: 

A. Autoencoder-Based Remote Sensing Image Scene Classification

B. CNN-Based Remote Sensing Image Scene Classification

(1) Using pre-trained CNNs as feature extractors

(2) Fine-tuning pre-trained CNNs

(3) Training CNNs from scratch

C. GAN-Based Remote Sensing Image Scene Classification

Generally Transfer learning works the best in the three categories according to research. 

### Model Structure

![img](lib/a-model.png)

### Experiment Tracking by Neptune

Check the following Link: 

https://ui.neptune.ai/xiaoya27/AerialImageClassification/experiments?viewId=standard-view

### Result
The modeled trained for 15 epochs on Mobilenet as feature extractor is submitted, the test accuracy is 0.90
Accuracy calculated by percentage of predicted values (yPred) that match with actual values (yTrue).

![img](lib/heatmap.png)


Class Activation Maps


Original            |  CAM
:-------------------------:|:-------------------------:
![img](lib/org.png)  |  ![img](lib/cam.png)


TODO :

Training for more epochs  
