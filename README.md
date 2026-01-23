# Driver-Eye-Monitoring-AI
eye monitoring project


# 👁️ Driver Eye Monitoring AI

This project is an AI-powered real-time driver eye monitoring system that detects driver drowsiness or inattention using a Convolutional Neural Network (CNN).  
The system captures live webcam video, analyzes the eye state (open or closed), and shows real-time predictions.

The project uses TensorFlow for deep learning, OpenCV for image processing, FastAPI for backend model serving, and Streamlit for frontend visualization.  
This project is developed mainly for learning and academic purposes.

---

## Features

- Eye state detection (Open / Closed) using a trained CNN model  
- Real-time webcam video capture and processing using OpenCV  
- FastAPI backend to load and serve the trained model  
- Streamlit frontend for live eye monitoring  
- Simple and beginner-friendly project structure  

---

## Tech Stack

| Tool              | Purpose                                      |
|-------------------|----------------------------------------------|
| TensorFlow        | Loading and running the CNN model (`model.h5`) |
| FastAPI           | Backend API server                           |
| Streamlit         | Frontend interface                           |
| OpenCV            | Webcam video stream capture                  |
| Pillow            | Image pre-processing                         |
| Uvicorn           | ASGI server to run FastAPI                   |
| Requests          | Communication between frontend & backend     |
| python-multipart  | File upload and form support in FastAPI      |

---

## Project Structure

Driver-Eye-Monitoring-AI/
│
├── backend/
│   ├── app.py              # FastAPI backend application
│   └── model.h5            # Trained CNN model
│
├── frontend/
│   └── frontend.py         # Streamlit frontend for live eye monitoring
│
├── model/
│   └── modelnotebook.ipynb # Model training notebook
│
├── requirements.txt        # Project dependencies
├── .gitignore
└── README.md

---

## Running code

### open terminal and clone the repo first

git clone https://github.com/ravikumar266/Driver-Eye-Monitoring-AI.git  
cd Driver-Eye-Monitoring-AI  

python -m venv venv  

venv\Scripts\activate  # Windows  
source venv/bin/activate  # macOS/Linux  

pip install -r requirements.txt  

---

cd backend  
uvicorn app:app --reload  

---

### open new terminal but do not close old terminal of fastapi

cd Driver-Eye-Monitoring-AI  # if required  
cd frontend  

streamlit run frontend.py  

---

### you can see an option to open camera. after clicking it, you can see live eye monitoring predictions
