# MultiModel Skin Cancer Classification (ConvNext+Vit+Mamba)

This repository contains a high-performance deep learning pipeline designed to classify skin lesions into 8 distinct categories using a ConvNext+Vit+Mamba backbone optimized for multi-GPU training.

## 📊 Dataset & Classes
The model trains on balanced clinical skin images across 8 target classes:
*   `AK` (Actinic Keratosis)
*   `BCC` (Basal Cell Carcinoma)
*   `BKL` (Benign Keratosis)
*   `DF` (Dermatofibroma)
*   `MEL` (Melanoma)
*   `NV` (Melanocytic Nevus)
*   `SCC` (Squamous Cell Carcinoma)
*   `VASC` (Vascular Lesions)

## 🛠️ Prerequisites
Before setting up the project, ensure you have the following installed on your host system:
*   **Python 3.12**
*   **pip** (Python package manager)
*   **CUDA Toolkit** (Compatible with your NVIDIA GPU drivers for PyTorch acceleration)

---

## 🚀 Installation & Setup

Follow these steps to set up a clean, isolated local environment and run the notebook.

### 1. Clone the Repository
```bash
git clone [https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git](https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git)
cd YOUR_REPOSITORY_NAME

cd vision
python -m venv venv
source venv/bin/activate # Mac
venv\Scripts\activate.bat # Windows
pip install --upgrade pip
pip install -r requirements.txt

cd NLP
python -m venv venv
source venv/bin/activate # Mac
venv\Scripts\activate.bat # Windows
pip install --upgrade pip
pip install -r requirements.txt

cd experiments
python -m venv venv
source venv/bin/activate # Mac
venv\Scripts\activate.bat # Windows
pip install --upgrade pip
pip install -r requirements.txt

To access the live application on the link http://129.151.134.18:8501/