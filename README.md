# 👁️ Driver-Eye-Monitoring-AI

> **Real-Time Driver Eye Monitoring System**  
> Detect driver drowsiness and inattention using deep learning and computer vision

---

## Overview

**Driver-Eye-Monitoring-AI** is an AI-powered real-time system that monitors a driver’s eye state to detect **drowsiness or inattention**.

The application captures live webcam video, processes eye images using **OpenCV**, and classifies the eye state (**Open / Closed**) using a **Convolutional Neural Network (CNN)**.  
A **FastAPI backend** serves the model, while a **Streamlit frontend** provides a live interactive interface.

This project is designed for **learning, academic projects, and portfolio demonstration**.

---

## Features

- Real-time eye state detection (Open / Closed)
- Live webcam feed using OpenCV
- CNN-based deep learning model (`model.h5`)
- FastAPI backend for inference
- Streamlit frontend for visualization
- Simple and beginner-friendly project structure

---

## Tech Stack

| Component | Tools |
|---------|-------|
| Deep Learning | TensorFlow / Keras |
| Backend | FastAPI, Uvicorn |
| Frontend | Streamlit |
| Computer Vision | OpenCV |
| Image Processing | Pillow |

---

## Processing Pipeline

    Webcam Feed
        ↓
    Frame Capture (OpenCV)
        ↓
    Image Preprocessing
        ↓
    CNN Model Prediction
        ↓
    Eye State (Open / Closed)
        ↓
    Live Display (Streamlit)

---

## 📁 Project Structure

    Driver-Eye-Monitoring-AI
    │
    ├── backend
    │   ├── app.py                 # FastAPI backend
    │   └── model.h5               # Trained CNN model
    │
    ├── frontend
    │   └── frontend.py            # Streamlit frontend
    │
    ├── model
    │   └── modelnotebook.ipynb    # Model training notebook
    │
    ├── requirements.txt
    ├── .gitignore
    └── README.md

---

## Installation

### Prerequisites

- Python 3.9+
- Webcam
- pip

---

## Local Setup

### 1. Clone Repository

    git clone https://github.com/ravikumar266/Driver-Eye-Monitoring-AI.git
    cd Driver-Eye-Monitoring-AI

---

### 2. Create Virtual Environment

    python -m venv venv

**Windows**

    venv\Scripts\activate

**macOS / Linux**

    source venv/bin/activate

---

### 3. Install Dependencies

    pip install -r requirements.txt

---

## Running the Application

### Start Backend (FastAPI)

    cd backend
    uvicorn app:app --reload

Keep this terminal running.

---

### Start Frontend (Streamlit)

Open a new terminal:

    cd Driver-Eye-Monitoring-AI
    cd frontend
    streamlit run frontend.py

---

## Usage

1. Open the Streamlit app in your browser  
2. Click **Open Camera**  
3. Allow webcam access  
4. View live eye state predictions  

---

## Author

**Harshit**  
GitHub: https://github.com/Harshit9569/Driver-Eye-Monitoring-AI
