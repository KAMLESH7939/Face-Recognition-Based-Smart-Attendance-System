🎓 Face Recognition Based Smart Attendance System
📌 Overview

This project implements a Smart Attendance System using Machine Learning (KNN classifier) and Computer Vision (OpenCV).
The system automates the process of marking attendance by recognizing student faces in real time and storing records with timestamps.

It is divided into two parts:

Local Execution – face data collection & recognition (requires webcam).

Cloud Dashboard – attendance visualization (deployed using Streamlit Cloud).

This hybrid setup ensures fast local recognition while providing a cloud-based dashboard for accessibility.

🚀 Features

✔️ Face data collection (100 images per user) with webcam.
✔️ Face recognition using K-Nearest Neighbors (KNN) classifier.
✔️ Automated attendance logging into CSV files with date & time.
✔️ Text-to-speech confirmation when attendance is recorded (Windows only).
✔️ Streamlit dashboard for real-time and historical attendance records.

🛠️ Tech Stack

Machine Learning: Scikit-learn (KNN Classifier)

Computer Vision: OpenCV

Data Handling: Pandas, NumPy, CSV

Frontend/Dashboard: Streamlit, Streamlit-Autorefresh

Others: PyWin32 (Windows text-to-speech)

📂 Project Structure
Face-Recognition-Based-Smart-Attendance-System/
│
├── add_faces.py         # Collects face images for training
├── test.py              # Recognizes faces & marks attendance
├── app.py               # Streamlit dashboard for attendance
├── requirements.txt     # Dependencies
├── data/                # Haar Cascade + face datasets
└── Attendance/          # Attendance CSV logs

⚙️ Installation & Setup
1️⃣ Clone the Repository
git clone https://github.com/KAMLESH7939/Face-Recognition-Based-Smart-Attendance-System.git
cd Face-Recognition-Based-Smart-Attendance-System

2️⃣ Install Dependencies
pip install -r requirements.txt

3️⃣ Run Locally

👉 Step 1: Collect face data

python add_faces.py


👉 Step 2: Run recognition & mark attendance

python test.py


👉 Step 3: Launch dashboard

streamlit run app.py

🌐 Live Demo

GitHub Repo: Face Recognition Attendance System

Streamlit Demo: [Add after deployment]

📊 Workflow

Data Collection → Capture face samples using OpenCV.

Training → Train a KNN classifier on the collected dataset.

Recognition & Attendance → Recognize faces in real time, log attendance into CSV.

Visualization → Attendance displayed via Streamlit dashboard.

📌 Notes

Local scripts (add_faces.py, test.py) require webcam access.

app.py can be deployed on Streamlit Cloud.

Text-to-speech works only on Windows (via PyWin32).

🎯 Future Improvements

Upgrade from KNN → Deep Learning models (CNN, FaceNet, Dlib) for higher accuracy.

Store attendance in cloud database (MongoDB/Firebase).

Web/Mobile UI for teachers and students.

👨‍💻 Author

Kamlesh
🎓 Final Year Student | Passionate about AI/ML, Computer Vision, Accessibility, Analysis, MERN Stack development & Competetive programming
🔗 GitHub: https://github.com/KAMLESH7939

✨ This project combines Machine Learning and Computer Vision to create a practical attendance automation system with cloud-based visualization.
