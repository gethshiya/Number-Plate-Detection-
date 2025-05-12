# Number Plate Detection using OCR and EasyOCR
# 📌 Overview
This project implements an image-based number plate detection system using computer vision and OCR (Optical Character Recognition). It identifies and reads vehicle license plates from static images, which can be used in traffic monitoring, toll systems, parking management, law enforcement, and smart cities.

# 🧠 Key Technologies
OpenCV: For image preprocessing and visualization.

EasyOCR: For extracting text from number plates.

Google Colab: Used for coding and image processing.

Whisper AI (for extension): Included in the pipeline to demonstrate emotion detection from audio (not directly used for number plates).

# 🚀 How It Works
Image Input: Loads images from a dataset folder in Google Drive.

Preprocessing: Converts images to grayscale, applies filters.

Text Detection: EasyOCR identifies text regions.

Text Extraction: Extracts the number plate text.

Output Display: Highlights the plate area and shows detected text.

# 📁 Folder Structure

/Indian_Number_Plates/
    └── Sample_Images/
        ├── image1.jpg
        ├── image2.jpg
        └── ...
# 🔧 Installation

pip install openai-whisper librosa scikit-learn easyocr opencv-python

# 💻 Usage

from google.colab import drive
drive.mount('/content/drive')

# Load dataset path and run analysis
dataset_path = '/content/drive/MyDrive/Indian_Number_Plates/Sample_Images'
detected_texts = analyze_dataset(dataset_path)
# Dataset link:
        https://www.kaggle.com/datasets/dataclusterlabs/indian-number-plates-dataset
        
# ✅ Features
Detects and extracts number plates from images.

Uses OCR to get readable text.

Supports multiple formats and fonts.

Can be extended for real-time or video input.

# ⚠️ Limitations

May struggle with blurry or angled images.

Not optimized for real-time use.

Only supports standard English characters.

Doesn’t handle multiple plates per image effectively.

# 🔮 Future Improvements
Add real-time video support.

Improve accuracy under poor lighting.

Use advanced OCR or LLMs for context validation.

Support for international number plate formats.

# 🧾 Conclusion
This project demonstrates a foundational pipeline for number plate detection using EasyOCR and OpenCV, capable of identifying and extracting plate numbers from images. While the system performs well under clean conditions, it has limitations in real-world scenarios such as motion blur or occlusions. The bonus emotion detection module serves as a proof of concept for multimodal AI integration. With future improvements and real-time capabilities, this project can evolve into a practical, intelligent traffic and surveillance tool.
