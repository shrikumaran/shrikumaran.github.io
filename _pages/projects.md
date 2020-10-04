---
layout: single
title: "Projects"
permalink: /projects/
comments: true
author_profile: true
---

# Computer Vision and Deep Learning 
## Pneumonia Clasifier
Classifies given X-Ray images of lungs into two classes, Normal lungs and lungs infected with Pneumonia
Chest X-ray images (anterior-posterior) of pediatric patients of one to five years old from Guangzhou Women and Children’s Medical Center, Guangzhou was used to train the model. https://data.mendeley.com/datasets/rscbjbr9sj/2
* Used transfer learning to train a VGG19 model pre-trained on ImageNet. Got a validation set accuracy of 85.5% after 100 epochs.
* Developed a custom CNN model with 6 fully convolution layers and 3 fully connected layers with dropout implemented in each layer. Obtained a max validation set accuracy of 88.9%.
## Autoencoder
Devloped an autoencoder for MNIST dataset. Developed one fully using fully connected layers alone and another using fully convolutional layers.
## Crops and weed detector
* Collected images of local crops and weeds and labeled them using LabelImg.
* Trained a FRCNN model on this dataset to detect weeds in real life conditions.
## Shape clasifier
Developed an algorithm using contour approximation(ApproxPolyDP in OpenCV) to detect shapes shown to the camera.
## Room occupants detector
Developed an algorithm using the YOLOv2 detector to keep track of occupants in a room and only power up the appliances close to them.
## Object detection app
Developed a flutter application to perfom object detection on photos captured. Used Tflite to load MobileNet model to perform inferences.

# Robotics
## Precision Agriculture Bot
Farmers in India are facing an issue of raising weedicides costs and raising labor costs, to solve this issue we decided to make this robot to specifically target weeds and spray microdoses of weedicide. 
Various components of our project:
* Mechanics
  * Designed and fabricated a chasis considering the measurements we collected from various farms.
* Electronics
  * Repurposed old windshield wiper motors to power the bot.
  * Developed a differential locomotion system using heavy duty motor drivers to handle the huge current load.
  * Used ROS to transmit live video back to our laptop.
  * Implemented joystick control with ROS.
* Computer Vision 
  * Collected a custom datset of weeds from farms near us.
  * Trained a FRCNN model to detect weeds apart from crops.

## Line following robot
Participated a line following robot competition where corrdiantes of the destination were inputted as images shown to a camera and the bot must follow the line to that coordinate.
Developed a 2 wheel differential bot using Arduino. Fabricated a IR sensor array to detect the line. Developed an OpenCV algorithm to detect shapes shown to the camera.

## Maze solving robot arm
The aim of this project was to given an image of a maze the solution of the maze should be traced by the arm on the maze.
* Developed a computer vision algorithm using OpenCV to detect the solution of the maze.
* Fabricated a 2 DOF arm and controlled using Arduino to trace the maze's solution.


