# Dog Breed Algorithm
This project was created for Udacity's Data scientist Nanodegree. It includes different approaches of writing an algorithm to identify dog breeds for a breed identification app. The algorithm outputs either a detected dog breed, or a dog breed that looks similar to the detected face or object in the input image, such as:

![Image of app output](https://github.com/marenjulia/dog-breed-algorithm/blob/main/images/algorithm_output_example.PNG)

## Table of Contents
1. [Installations](#installations)
2. [Project Motivation](#motivation)
3. [File Overview](#overview)
4. [Key Results](#results)
4. [Acknowledgements](#acknowledgements)

## <a id="installations"/> Installations

This project used Python 3 within Jupyter Notebook, plus the following libraries: 
- pandas
- nimpy
- sklearn
- keras
- glob
- random
- cv2
- tqdm
- matplotlib
- PIL

## <a id="motivation"/> Project Motivation

The motivation of this project was to develop ideas for a dog identification app using deep learning concepts. The software is intended to accept any user-supplied image as input. If a dog is detected in the image, it will provide an estimate of the dog’s breed. If a human is detected, it will provide an estimate of the dog breed that is most resembling.The steps to achieve this result were:
* Step 0: Import Datasets
* Step 1: Detect Humans
* Step 2: Detect Dogs
* Step 3: Create a CNN to Classify Dog Breeds (from Scratch)
* Step 4: Use a CNN to Classify Dog Breeds (using Transfer Learning)
* Step 5: Create a CNN to Classify Dog Breeds (using Transfer Learning)
* Step 6: Write the Algorithm
* Step 7: Test the Algorithm

##  <a id="overview"/> File Overview

* dog_app.ipynb: A Jupyter notebook with the majority of the project code
* dog_app.html: An html file containing the same information as the Jupyter notebook
* extract_bottleneck_features.py: Helper functions to extract bottleneck features from models
* images/ : a folder containing example images
* haarcascades/ : a folder containing the haarcascade definition file for face recognition
* requirements/ : a folder containing requirement files
* saved_models/: a folder containing saved models from several of the employed models

## <a id="results"/> Key Results 

Within the project, several approaches were employed, including a convolutional network built from scratch. The best results were achieved when using a transfer learning model using the Inception V3 network. Here an accuracy of 83.6% was achieved.

There are still possibilities to improve upon the model, e.g. by gathering more training data, employing data augmentation or adding more layers. Still, the accuracy from the test and the tests with specific image samples suggest that the model could be used as part of a mobile or web app such as the one described above.

## <a id="acknowledgements"/> Acknowledgements 

This project is largely based on starter code provided by Udacity. 
