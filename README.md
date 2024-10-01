## Object Detection with YOLOv5 and Multilingual Support

Project Overview

This project aims to implement object detection using the YOLOv5 model, with a focus on providing a user-friendly and accessible solution. It supports both image and video inputs, detecting objects, drawing bounding boxes, and providing object counts in both English and Arabic.

Key Features

Image Object Detection: Detects objects in uploaded images and draws bounding boxes around them.
Video Object Detection: Processes videos frame by frame, detecting objects and drawing bounding boxes.
Multilingual Support: Translates detected object labels from English to Arabic for Arabic-speaking users.
Interactive Interface: Utilizes Gradio for a user-friendly interface that simplifies interaction with the model.
Expected Outputs

Image Input:
Original image with bounding boxes around detected objects.
Table displaying object names and counts in English and Arabic.
Video Input:
Processed video with bounding boxes around detected objects in each frame.
Table showing overall object counts across the entire video in English and Arabic.
Model Choices

Object Detection: YOLOv5 - A fast and accurate deep learning model for real-time object detection. The yolov5s model is used for its balance of speed and accuracy.
Translation: Helsinki-NLP/opus-mt-en-ar - A powerful neural machine translation model for English-to-Arabic translation.
Pipeline Explanation

Object Detection: The input image or video is fed into the YOLOv5 model, which outputs bounding boxes, class labels, and confidence scores for detected objects.
Bounding Box Drawing: Bounding boxes are drawn around detected objects using OpenCV or PIL.
Label Translation: Detected object labels are translated from English to Arabic using the Helsinki-NLP model.
Results Output: The modified image or video is displayed alongside a table of detected object counts in both languages.
Justification for Model and Pipeline Choices

YOLOv5 is chosen for its speed, accuracy, and efficiency in both image and video object detection.
Helsinki-NLP's translation model ensures seamless English-to-Arabic translation, making the project accessible to a wider audience.
Gradio provides a user-friendly interface for easy interaction with the model.
Arabic Language Support

The project prioritizes accessibility for Arabic-speaking users by automatically translating object labels to Arabic. This feature expands the project's reach and value for users in Arabic-speaking regions.
