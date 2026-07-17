# Real-Time Mask Control 😷

A real-time face mask detection system built in Python, developed during an internship/project at Adana Science and Technology University. The system uses a webcam feed to detect whether a person is wearing a mask and provides real-time audio feedback.

## 📋 Overview

The application captures live video from a camera, detects faces using Haar Cascade classifiers, and classifies whether each detected face is wearing a mask or not — giving immediate audio feedback ("Thanks for wearing a mask" / "Please wear a mask").

## ✨ Features

- **Real-time face detection** using OpenCV Haar Cascade (`haarcascade_frontalface_default.xml`)
- **Mask classification** via a trained machine learning model
- **Audio alerts** depending on detection result (`WearMask.mp3`, `Thanks2Wear.mp3`)
- **Dataset tools** for building and manipulating training data (`CamToPix`)
- Packaged as a standalone Windows executable via PyInstaller

## 🛠️ Tech Stack

- **Python**
- **OpenCV** — face detection and image processing
- **Machine Learning** (classification model for mask/no-mask prediction)
- **Pandas / CSV** — dataset handling and manipulation

## 📁 Project Structure

```
MedicalMaskControl/
├── CamToPix/              # Machine learning training tools + CSV/dataset manipulation
├── data/
│   ├── Dataset.csv        # Training dataset
│   ├── LastPhoto.csv      # Most recent captured frame data
│   └── theFrame.png       # Captured frame from camera
├── GetFaceImg.py          # Face detection / image capture logic
├── MLAPI.py               # Machine learning model interface
├── RealTimeMaskControl.py # Main application entry point
├── haarcascade_frontalface_default.xml  # Pre-trained face detection model
├── WearMask.mp3           # Audio alert: mask not detected
├── Thanks2Wear.mp3        # Audio alert: mask detected
└── Real Time Mask Control Report Osman INCI.docx  # Project report/documentation
```

## 🚀 Getting Started

```bash
# Install dependencies
pip install opencv-python pandas

# Run the application
python RealTimeMaskControl.py
```

> Note: A pre-built Windows executable (`RealTimeMaskControl.exe`) can also be generated using PyInstaller — see `ReadMe.txt` for details.

## 📄 Project Report

A detailed project report is included: `Real Time Mask Control Report Osman INCI.docx`, covering the methodology, dataset preparation, and evaluation of the model.

## 👤 Author

**Osman Inci**
- GitHub: [@dev2imp](https://github.com/dev2imp)
- LinkedIn: [Osman Inci](https://www.linkedin.com/in/osman-inci-868435221/)
