# 🎓 Face Recognition Attendance System

A web-based employee attendance system that uses **facial recognition** to automatically record and track attendance in real time.

> Graduation Project — Computer Science, Imam Muhammad bin Saud Islamic University (2025)

---

## 📌 Overview

This system replaces traditional manual attendance methods with an automated facial recognition solution. Employees are identified through a live camera feed, and their attendance is instantly logged with a timestamp into a daily CSV report.

---

## ✨ Features

- 📷 Real-time face detection using **OpenCV** and Haar Cascade classifier
- 🤖 Face identification using **K-Nearest Neighbors (KNN)** algorithm
- ➕ Register new employees by capturing face images via webcam
- 📊 Automatic daily attendance logging saved to **CSV files**
- 🌐 Web dashboard to view attendance records (built with **Flask**)
- 🔁 Model retraining triggered automatically when new users are added

---

## 🛠️ Technologies Used

| Category | Tools |
|---|---|
| Language | Python |
| Web Framework | Flask |
| Computer Vision | OpenCV |
| Machine Learning | Scikit-learn (KNN) |
| Data Handling | Pandas, NumPy |
| Model Storage | Joblib |
| Frontend | HTML, CSS |

---

## 📁 Project Structure

```
├── app.py                          # Main Flask application
├── background.png                  # UI background image
├── haarcascade_frontalface_default.xml  # Face detection model
├── Attendance/
│   └── Attendance-MM_DD_YY.csv    # Daily attendance records
├── static/
│   ├── faces/                      # Registered employee face images
│   ├── face_recognition_model.pkl  # Trained KNN model
│   └── img/                        # UI assets
└── templates/
    └── home.html                   # Web dashboard
```

---

## 🚀 How to Run

### 1. Clone the repository
```bash
git clone https://github.com/Zainabh00/face-recognition-attendance.git
cd face-recognition-attendance
```

### 2. Install dependencies
```bash
pip install flask opencv-python scikit-learn pandas numpy joblib
```

### 3. Run the application
```bash
python app.py
```

### 4. Open your browser
```
http://localhost:5000
```

---

## 📖 How It Works

1. **Register Employee** — The system captures 10 face images via webcam and trains the KNN model
2. **Take Attendance** — Live camera feed detects and identifies faces in real time
3. **Log Attendance** — Recognized employees are automatically added to the daily CSV with timestamp
4. **View Dashboard** — Web interface displays today's attendance records

---

## 👩‍💻 Team

Developed as a graduation project by a team of Computer Science students at IMIASU (2025).

My contributions:
- Database design and management using **SQL**
- Face classification model implementation using **KNN**
- Data analysis and testing using **Jupyter Notebook**

---

## 📄 License

This project was developed for academic purposes.
