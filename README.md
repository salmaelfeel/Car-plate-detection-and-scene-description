# Car-plate-detection-and-scene-description
---

## Project Overview

This project integrates three computer vision components into a single pipeline, served via an interactive Gradio interface. The system performs the following tasks on any uploaded scene image:

1. **License Plate Detection**
   A YOLOv11 model (`best.pt`) is used to detect vehicle license plates and extract bounding box coordinates with confidence scores.

2. **Text Recognition**
   PaddleOCR is applied to each detected plate region to extract text and recognition confidence.

3. **Scene Captioning**
   A VisionEncoderDecoder model (`nlpconnect/vit-gpt2-image-captioning`) is used to generate a natural language description of the entire scene.

All outputs are compiled into a JSON file containing the image caption, plate coordinates, plate confidence scores, recognized texts, and their confidence values.

---

## How to Use

* Simply run the provided notebook.
* A Gradio app will launch for interaction.
* Upload any scene image and the system will process it.
* Sample test images are already included in the repository.

---

