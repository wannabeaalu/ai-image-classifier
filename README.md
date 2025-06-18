# AI Image Classifier – Real-Time Web App

This project is a web-based image classification system built using Streamlit and a pre-trained MobileNetV2 model from TensorFlow for identifying objects in images.

## 🔍 What it does

- Lets users upload `.jpg` or `.png` images  
- Preprocesses the image to fit the model input (224x224 pixels)  
- Classifies the image using MobileNetV2 trained on ImageNet  
- Displays top 3 predictions with confidence scores  
- Caches the model for faster performance using Streamlit's `@st.cache_resource`

## ⚙️ Requirements

Make sure you use **Python 3.11**

> ⚠️ **Important:** TensorFlow support for versions beyond Python 3.11 is discontinued as of **March 2025**.

### Recommended Setup (using [uv](https://github.com/astral-sh/uv)):

```bash
uv venv
uv pip install streamlit tensorflow opencv-python pillow numpy
```

### Or, using pip:

```bash
pip install streamlit tensorflow opencv-python pillow numpy
```

## 🚀 How to Run

```bash
streamlit run app.py
```

Replace `app.py` with your actual filename if it differs.

## 🧠 Model Used

- MobileNetV2 from `tensorflow.keras.applications`  
- Trained on the ImageNet dataset  
- Uses `decode_predictions` to show class labels and probabilities

## 🛠️ Technologies Used

- Python  
- Streamlit  
- TensorFlow / Keras  
- OpenCV  
- Pillow (PIL)  
- uv (for dependency management)
