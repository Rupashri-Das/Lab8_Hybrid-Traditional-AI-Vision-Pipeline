Lab 8 — Hybrid Project: Traditional + AI
Overview

This project demonstrates a hybrid computer vision pipeline that combines both traditional image processing techniques and AI-based methods. The main goal is to understand how traditional pre-processing can enhance the performance of AI classification models.

Learning Objectives

After completing this lab, you will be able to:

Understand a basic hybrid computer vision pipeline combining traditional and AI methods.

Use traditional techniques for image preparation and segmentation.

Apply a pre-trained Convolutional Neural Network (CNN) for image classification.

Analyze how the combination of both methods improves accuracy and efficiency compared to using a single approach.

Code Explanation

The MATLAB script follows four main sections:

1. Load Image and AI Network

Loads a sample image (peppers.png) for testing.

Loads a pre-trained SqueezeNet CNN model for classification.

Displays the original image in the first figure panel.

2. Traditional Method (K-Means Color Segmentation)

Converts the image to Lab color space for better color separation.

Performs K-means clustering to segment the image into two regions.

Creates a mask to isolate the main object from the background.

Displays both the segmentation mask and the isolated object.

3. AI Method (Image Classification)

Resizes the isolated object to fit the CNN input size (227×227×3).

Classifies the object using the SqueezeNet model.

Outputs the predicted class and confidence score.

4. Results Analysis

Shows the resized input used for AI classification.

Prints the predicted label and confidence probability in the MATLAB console.
Demonstrates how traditional pre-processing improves classification focus and results.

How to Run

Open the MATLAB script.

Ensure that Deep Learning Toolbox and Image Processing Toolbox are installed.

Run the code directly in MATLAB.

Observe the outputs in the figure window and the classification result in the command window.
