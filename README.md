# Phone-Detection-1.0
# Phone Detection Alert System

## About the Project

For this project, I made a program that can detect when someone is using a phone. It uses an NVIDIA Jetson Orin Nano, a webcam, and an AI model that I trained myself. When the camera sees a phone for a few seconds, the program gives an alert telling the person to put their phone away.

## How It Works

First, the webcam records a live video feed. Every frame is sent to my AI model, which looks for mobile phones. If the model detects a phone and it stays visible for a few seconds, the program displays a warning message. If the phone is removed, the alert stops and the program starts watching again.

## How I Made It

I used NVIDIA's Jetson Inference library and DetectNet SSD to train my own object detection model. I trained it using the Open Images dataset, which has thousands of pictures of mobile phones with labeled bounding boxes. After training the model, I exported it and used it in a Python program that runs on the Jetson Orin Nano.

## Materials Used

* NVIDIA Jetson Orin Nano
* USB Webcam
* Jetson Inference
* Python
* DetectNet SSD
* Open Images Dataset

## Challenges

One challenge was learning how to train the AI model and getting all of the files set up correctly. Another challenge was making sure the program only alerts after a phone has been detected for a few seconds so it doesn't constantly give false alarms.

## What I Learned

This project taught me how object detection works and how AI models are trained. I also learned how to use the Jetson Orin Nano, work with Python, and connect an AI model to a live camera feed.

## Future Improvements

If I continue working on this project, I would like to make it smarter by detecting when someone is actually using a phone instead of just seeing one. I would also like to add voice alerts, save pictures when a phone is detected, and improve the accuracy by training the model with more images.

**link to the video**: 
