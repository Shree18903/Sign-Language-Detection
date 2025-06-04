# Sign-Language-Detection

# Sign Language Detection using Deep Learning

## Overview
This project implements a **Sign Language Detection System** using Deep Learning. It trains a model to recognize hand gestures representing different letters or words in sign language, and provides a **GUI-based interface** to detect real-time signs through a webcam.

## Project Structure
```
├── Models/               # Pre-trained deep learning models
├── dataSet/              # Dataset for training and testing
├── app.py                # Main application file (GUI + Prediction)
├── Model_Training.ipynb  # Notebook to train deep learning models
├── README.md             # Project documentation
```

## Prerequisites
- Python 3.9.0
- pip (latest version)

### Required Python Libraries
Install the required libraries using:
```bash
pip install --upgrade pip
pip install numpy
pip install opencv-python
pip install tensorflow
pip install keras
pip install tk
pip install Pillow
pip install pyenchant
pip install cyhunspell
```

> **Note:**  
> `strings` and `os-sys` are built-in modules and don't need separate installation.

### Recommended Package Versions
- `tensorflow==2.12.0`
- `keras==2.12.0`
- `opencv-python==4.10.0.84`
- `deepface==0.0.93`
- `flask==3.1.0`
- `scikit-learn==1.6.0`
- `matplotlib==3.9.4`
- `pillow==11.0.0`

## Installation

### 1. Clone the Repository
```bash
git clone <your-repository-url>
cd sign-language-detection
```

### 2. (Optional) Create a Virtual Environment
```bash
python -m venv venv

# Activate it
# On Windows
venv\Scripts\activate
# On Linux/Mac
source venv/bin/activate
```

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```
*(or install manually as mentioned above)*

## Dataset and Models
- Extract `dataSet.zip` into the `dataSet/` folder.
- Extract `Models.zip` into the `Models/` folder.

Make sure both folders are placed in the same directory as `app.py`.

## How to Run

### Step 1: Train the Model (Optional)
- Open `Model_Training.ipynb` in **Jupyter Notebook** or **Google Colab**.
- Execute all cells to train the model.
- Save the trained model into the `Models/` directory.

*(Skip this step if you are using pre-trained models.)*

### Step 2: Launch the Application
```bash
python app.py
```
- A GUI window will open.
- Show your hand gesture in front of the webcam.
- The system will **predict and display** the recognized sign in real-time.

## Important Notes
- Ensure you grant **webcam access** when running the application.
- Use **clear hand gestures** against a **plain background** for better detection.
- The **GUI** is developed using **tkinter**.
- **Real-time detection** is powered by **OpenCV**.
- **Model predictions** are performed using **TensorFlow** and **Keras**.

## Future Enhancements
- Recognize complete sentences with dynamic signing.
- Deploy a **web-based** version of the application.
- Further improve **real-time prediction accuracy** and **user feedback**.

## License
This project is intended for **educational** and **personal use only**.
