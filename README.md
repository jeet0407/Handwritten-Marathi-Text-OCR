# 📝 Handwritten Marathi OCR

A deep learning-based OCR system that recognizes **handwritten Marathi sentences** using image preprocessing, contour-based segmentation, and a CNN model trained on 92,000 labeled characters.

## 🚀 Features
- Recognizes full **handwritten Marathi sentences**
- Custom segmentation for **Shirorekha** handling
- Achieves **98.79% test accuracy**
- Built with **OpenCV** + **TensorFlow/Keras**

## 🧠 Model
- Input: 32×32 grayscale character images  
- CNN → ReLU → MaxPooling → Dense → Softmax  
- Trained on 46 Marathi character classes

## 📁 Dataset
- 92,000 images (2000/class)  
- From [UCI ML Repository] https://archive.ics.uci.edu/dataset/389/devanagari+handwritten+character+dataset
- Split: 80% train, 10% val, 10% test

## 💻 Run Locally

git clone https://github.com/jeet0407/Handwritten-Marathi-Text-OCR.git
cd marathi-ocr
pip install -r requirements.txt
jupyter notebook model2.ipynb
