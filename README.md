# 🎓 Face Recognition Based Smart Attendance System  

## 📌 Overview  
<img width="1918" height="1078" alt="image" src="https://github.com/user-attachments/assets/793ebf52-d157-4a89-ad64-9bd17fcfbd5d" />

This project implements a **Smart Attendance System** using **Machine Learning (KNN classifier)** and **Computer Vision (OpenCV)**.  
The system automates the process of marking attendance by recognizing student faces in real time and storing records with timestamps.  

It is divided into two parts:  
1. **Local Execution** – face data collection & recognition (requires webcam).  
2. **Cloud Dashboard** – attendance visualization (deployed using **Streamlit Cloud**).  

This hybrid setup ensures **fast local recognition** while providing a **cloud-based dashboard** for accessibility.  

---

## 🚀 Features  
- ✅ Face data collection (100 images per user) with webcam  
- ✅ Face recognition using **K-Nearest Neighbors (KNN)** classifier  
- ✅ Automated attendance logging into CSV files with date & time  
- ✅ Text-to-speech confirmation when attendance is recorded (Windows only)  
- ✅ **Streamlit dashboard** for real-time and historical attendance records  

---

## 🛠️ Tech Stack  
- **Machine Learning**: Scikit-learn (KNN Classifier)  
- **Computer Vision**: OpenCV  
- **Data Handling**: Pandas, NumPy, CSV  
- **Frontend/Dashboard**: Streamlit, Streamlit-Autorefresh  
- **Others**: PyWin32 (Windows text-to-speech)  

---

## 📂 Project Structure  
```bash
Face-Recognition-Based-Smart-Attendance-System/
│
├── add_faces.py         # Collects face images for training
├── test.py              # Recognizes faces & marks attendance
├── app.py               # Streamlit dashboard for attendance
├── requirements.txt     # Dependencies
├── data/                # Haar Cascade + face datasets
└── Attendance/          # Attendance CSV logs
 ```

---

## ⚙️ Installation & Setup  

### 1️⃣ Clone the Repository  
```bash
git clone https://github.com/KAMLESH7939/Face-Recognition-Based-Smart-Attendance-System.git
cd Face-Recognition-Based-Smart-Attendance-System
```
### 2️⃣ Install Dependencies
```bash
pip install -r requirements.txt
```
### 3️⃣ Run Locally
Step 1: Collect face data
```bash
python add_faces.py
```
Step 2: Run recognition & mark attendance
```bash
python test.py
```
Step 3: Launch dashboard
```bash
streamlit run app.py
```
### streamlit run app.py

-📍 GitHub Repo: https://github.com/KAMLESH7939/Face-Recognition-Based-Smart-Attendance-System
-📍 Streamlit Demo: https://face-recognition-based-smart-attendance-system.streamlit.app
<img width="1918" height="1030" alt="image" src="https://github.com/user-attachments/assets/6e1ec5d0-5747-4fbd-917a-8785589ad450" />

---

## 📊 Workflow
- Data Collection → Capture face samples using OpenCV
- Training → Train a KNN classifier on the collected dataset
- Recognition & Attendance → Recognize faces in real time, log attendance into CSV
- Visualization → Attendance displayed via Streamlit dashboard

---

## 📌 Notes
- add_faces.py and test.py require local execution (due to webcam & speech).
- app.py can be deployed on Streamlit Cloud.
- Text-to-speech (TTS) works only on Windows.
---

## 🎯 Future Improvements
 - 1.Upgrade from KNN → Deep Learning (CNN, FaceNet, Dlib) for higher accuracy
 - 2.Store attendance in cloud database (MongoDB/Firebase)
 - 3.Web/Mobile UI for teachers and students
---
## 👨‍💻 Author
Kamlesh
🎓 Final Year Student | Passionate about AI/ML, Computer Vision, MERN Stack development, analysis, research & Accessibility related stufs.
🔗 GitHub: https://github.com/KAMLESH7939

✨ This project combines Machine Learning and Computer Vision to create a practical attendance automation system with cloud-based visualization.
