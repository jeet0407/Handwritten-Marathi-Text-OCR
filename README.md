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

## Documentation - https://drive.google.com/file/d/1l6Fsw2-6c4X818qJ7VGx_RrQ51asv8um/view

## ⚙️ Setting Up the Project

Follow these steps to set up the project on your local machine:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/Handwritten-Marathi-Text-OCR.git
   cd Handwritten-Marathi-Text-OCR
   ```

2. **Create a virtual environment:**
   ```bash
   python -m venv .venv
   ```

3. **Activate the virtual environment:**
   - On Windows:
     ```bash
     .venv\Scripts\activate
     ```
   - On macOS/Linux:
     ```bash
     source .venv/bin/activate
     ```

4. **Install the required libraries:**
   ```bash
   pip install -r requirements.txt
   ```

5. **Create necessary directories:**
   - Create a directory named `pls` in the root of the project. Inside `pls`, create three subdirectories: `train`, `val`, and `test`.
   - Create a directory named `images` in the root of the project. This is where you will store the images you want to test.

6. **Run the Jupyter Notebook:**
   - Start Jupyter Lab:
     ```bash
     jupyter lab
     ```
   - Open and run the `ocr_model.ipynb` notebook to train the model.
   - Open and run the `outputs.ipynb` notebook to test the model on your images.
