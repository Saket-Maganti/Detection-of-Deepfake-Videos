# 🧠 Detection of Deepfake Videos

This project is a full-stack solution for detecting deepfake videos using deep learning models and a Django-based web interface. It enables users to upload videos and receive predictions on their authenticity.

---

## 📁 Project Structure

```
Detection-of-Deepfake-Videos/
│
├── Django Application/                # Web application using Django framework
│   ├── manage.py                      # Django management script
│   ├── ml_app/                        # Core application logic
│   ├── models/                        # ML model integration
│   ├── static/, templates/           # Static files and HTML templates
│   └── uploaded_videos/              # Uploaded videos for prediction
│
├── Model Creation/                   # Model development and training
│   ├── Model_and_train_csv.ipynb     # Main training notebook
│   ├── Predict.ipynb                 # Model prediction demo
│   ├── preprocessing.ipynb           # Preprocessing pipeline
│   ├── Helpers/                      # Utilities for training and testing
│   ├── labels/, Readme.md            # Data and metadata
```

---

## ⚙️ Features

- 📹 Upload video files for prediction
- 🧠 Deep learning model trained for deepfake detection
- 🧪 Real-time prediction via Django interface
- 📊 Preprocessing and feature extraction pipeline
- 📝 Notebooks for reproducibility and experimentation

---

## 🛠️ Tech Stack

- **Frontend**: HTML, Bootstrap (within Django templates)
- **Backend**: Django, Python
- **ML/AI**: TensorFlow/Keras, OpenCV, NumPy, Pandas
- **Database**: SQLite (Django default)
- **Deployment**: Local or server-based (Gunicorn, Nginx)

---

## 🚀 How to Run

### 🔧 Prerequisites

- Python 3.7+
- Virtualenv (optional but recommended)
- Required Python packages (Django, TensorFlow, OpenCV, etc.)

### 🔄 Setup

```bash
# Navigate to the Django app directory
cd 'Django Application'

# Create virtual environment
python -m venv venv
source venv/bin/activate  # or venv\Scripts\activate on Windows

# Install dependencies
pip install -r requirements.txt  # (Ensure this file exists or install manually)

# Run migrations
python manage.py migrate

# Run the server
python manage.py runserver
```

Visit `http://127.0.0.1:8000/` in your browser to use the app.

---

## 🧪 Model Training & Prediction

1. Go to the `Model Creation/` directory.
2. Open the following notebooks:
   - `Model_and_train_csv.ipynb` for training
   - `Predict.ipynb` for inference
   - `preprocessing.ipynb` for image preprocessing

Ensure that the required CSV datasets and video/image data are available in the appropriate folders.

---

## 📌 Notes

- Make sure the trained model is saved inside the Django app’s `models/` directory to be loaded for predictions.
- Uploaded files are saved inside `uploaded_images/` or `uploaded_videos/`.
- Customize the ML model path in the Django app as per your setup.

---

## 🙋‍♂️ Author

Developed by Saket Maganti
Feel free to contribute or extend this project for academic or research purposes.

---

## 📜 License

This project is intended for educational and research use only.
