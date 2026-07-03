# Phone-Detection-1.0

## About the Project

For this project, I made a program that can detect when someone is using a phone. It uses an NVIDIA Jetson Orin Nano, a webcam, and an AI model that I trained myself. When the camera sees a phone for a few seconds, the program recognizes the phone in their hand.

## How It Works

First, the webcam records a live video feed. Every frame is sent to my AI model, which looks for mobile phones. If the model detects a phone, the program displays a box around the phone in frame. If the phone is removed, there is no object box display around any recognized objects.

<img width="2238" height="1421" alt="image" src="https://github.com/user-attachments/assets/38d57466-1992-4021-a997-e74d8ef83fab" />


## How I Made It

I used NVIDIA's Jetson Inference library and DetectNet SSD to train my own object detection model. I trained it using the Open Images dataset, which has thousands of pictures of mobile phones with labeled bounding boxes. After training the model, I exported it and ran it on the Jetson Orin Nano.

## Materials Used

* NVIDIA Jetson Orin Nano
* USB Webcam
* Jetson Inference
* Python
* DetectNet SSD
* Open Images Dataset

## Challenges

One challenge was learning how to train the AI model and getting all of the files set up in the correct folders. I encountered an issue when after downloading and unzipping the images, it was stored in the wrong folder, rendering it innaccessible for triaining. To solve this, I re-downloaded the files, making sure to direct them into the correct folder.

## What I Learned

This project taught me how object detection works and how AI models are trained. I also learned how to use the Jetson Orin Nano, work with Python, and connect an AI model to a live camera feed.

## Future Improvements

I am currently working to improve on this project by integrating this detection system into a larger python project. I will create an entire workspace system that tracks phone pick-ups, allows for 30 seconds of being on the phone before an alert, offers a 5 minute bypass to be on a phone, breaks every 45 minutes, has a start-up screen and prompts user to start the system, and a stopwatch to track worktime, finally displaying all of work stats once finished.

**link to the video**: https://youtu.be/uqJCuXCJyqs 
