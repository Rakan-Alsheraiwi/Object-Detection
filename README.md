# Object Detection

# Project Overview
This project focuses on **Object Detection** using **YOLOv5**. It detects objects in both images and videos, drawing bounding boxes around detected objects and providing object counts. The project integrates a multilingual translation pipeline, translating the detected object labels from **English** to **Arabic**, supporting Arabic-speaking users. The solution is built using **Python** and libraries like **Torch**, **OpenCV**, **PIL**, **Gradio**, **Pandas**, and **Hugging Face Transformers**.

# Features
1. **Image Object Detection**: Upload an image, and the model will detect objects, draw bounding boxes, and provide object counts in both **English** and **Arabic**.
2. **Video Object Detection**: Upload a video, and the model processes each frame to detect objects, draw bounding boxes, and generate overall object counts.
3. **Arabic Support**: Detected object labels are translated from **English** to **Arabic**, making the project accessible for Arabic-speaking users.
4. **Interactive Interface**: A user-friendly interface built using **Gradio** allows easy interaction with both image and video detection models.

# Expected Outputs
1. **Image Input**: The model returns: * The original image with bounding boxes around detected objects. * A table showing object names and counts in both **English** and **Arabic**.
2. **Video Input**: The model returns: * A processed video with bounding boxes around detected objects in each frame. * A table showing overall object counts across the entire video in both **English** and **Arabic**.”

# Model Choices
**YOLOv5 for Object Detection**: 
**YOLOv5** (**You Only Look Once**) is a fast and accurate deep learning model for real-time object detection.
** We use the `yolov5s` model for this project, which balances speed and accuracy, making it suitable for processing both images and videos.
* YOLOv5 on Hugging Face.”

“**Helsinki-NLP for Translation**:
**The translation model used is `Helsinki-NLP/opus-mt-en-ar`, a powerful neural machine translation model that supports **English-to-Arabic translation**.
**This model ensures that object labels are accessible for Arabic-speaking users.
**Helsinki\-NLP/opus\-mt\-en\-ar on Hugging Face.”

# Pipeline Explanation
**Object Detection (YOLOv5)**: * The input image or video is fed into the **YOLOv5** model, which outputs bounding boxes, class labels, and confidence scores for detected objects.
**Bounding Box Drawing**: * Using **OpenCV** or **PIL**, bounding boxes are drawn around detected objects in the image or video frames.
**Label Translation**: * Detected object labels are passed to the translation model, translating the English labels to Arabic.
**Results Output**: * The modified image or video is displayed alongside a table of detected object counts in both **English** and **Arabic**.

# Justification for Model and Pipeline Choices
**YOLOv5** is chosen for its speed, accuracy, and efficiency in both image and video object detection, making it suitable for real-time applications.
**Helsinki-NLP's translation model** was selected to provide seamless **English-to-Arabic translation**, crucial for supporting users in Arabic-speaking regions.”
“* The use of **Gradio** allows for easy interaction with the models, offering an intuitive user interface that requires no programming knowledge to use.”

# Arabic Language Support
“Special attention has been given to supporting the **Arabic language**: * Object labels are automatically translated to **Arabic** using the `Helsinki-NLP/opus-mt-en-ar` translation model. * This makes the project accessible for a wider audience, especially users from Arabic-speaking regions.”

# Installation

“Clone the repository:”
“git clone https://github.com/your-username/object-detection.git cd object-detection”
“* Install dependencies: bash نسخ الكود `pip install -r requirements.txt` * Run the application: bash نسخ الكود `python app.py`”

# Usage
“* **For Image Detection**: * Upload an image to detect objects with bounding boxes and object counts in both **English** and **Arabic**. * **For Video Detection**: * Upload a video to detect objects across frames and receive a processed video with object counts in **English** and **Arabic**.”


























































