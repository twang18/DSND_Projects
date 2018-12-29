# Capstone Project - Dog Breed Classification

### Table of Contents

1. [Installation](https://github.com/twang18/Dog_Breed#installation)
2. [Project Motivation & Methodology](https://github.com/twang18/Dog_Breed#motivation)
3. [File Descriptions](https://github.com/twang18/Dog_Breed#files)
4. [Results](https://github.com/twang18/Dog_Breed#results)

## Installation

The following extra libraries are required:

- numpy, matplotlib, sklearn, keras, glob, tensorflow, cv2, tqdm, PIL
- python version: 3.6

## Project Statement & Methodology

In this project, the goal is to classify images of dogs according to their breeds. At the end of this project, the code is supposed to accept any user-supplied images as input, detect objects such as dogs, human or neither, and then make predictions on their classes. If a dog is detected in the image, it will predict the dog's breed. If a human is detected, it will identify the dog breed that is the most resembling.

In order to achieve the project goal, seven steps are followed:

- Step 0: Import Datasets
- Step 1: Detect Humans
- Step 2: Detect Dogs
- Step 3: Create a CNN to Classify Dog Breeds (from Scratch)
- Step 4: Use a CNN to Classify Dog Breeds (using Transfer Learning)
- Step 5: Create, Compare and Optimize a CNN to Classify Dog Breeds (Comparing 4 Transfer Learning Models)
- Step 6: Write My Algorithm to Classify Dog Breeds
- Step 7: Test My Algorithm

## File Descriptions

- dog_app.ipynb: jupyter notebook where the full codes are stored
- images: additional images I used are added here
- extract_bottleneck_features.py
- haarcascades: an opencv classifier for face detection
- DSND Capstone Project Report

## Results

- For complete full codes, please refer to the jupyter notebook.
- For complete description, results and analysis, please refer to the project report.