# 🏋️ AI Real-Time Gym Coach

An AI-powered virtual fitness coach that provides **real-time exercise tracking, pose estimation, repetition counting, form correction, workout history, and proactive voice coaching** using computer vision and large language models.

## 🚀 Features

* 🎥 **Real-time Pose Detection**

  * Uses MediaPipe Pose Landmarker for accurate body tracking.

* 💪 **Supported Exercises**

  * Squats
  * Push-ups
  * Biceps Curls
  * Shoulder Press
  * Lunges

* 🔢 **Automatic Rep Counting**

  * Counts repetitions in real time using exercise-specific motion analysis.

* 📊 **Workout Metrics**

  * Total repetitions
  * Current set progress
  * Sets completed
  * Workout duration

* ✅ **Form Analysis**

  * Detects improper posture and provides corrective feedback.

* 🤖 **AI Voice Coach**

  * Personalized coaching powered by Groq LLM.
  * Motivational and corrective voice feedback using Text-to-Speech.

* 👤 **User Authentication**

  * Secure login system for personalized workout tracking.

* 📝 **Workout History**

  * Stores previous workout sessions and displays progress over time.

* 🌐 **Browser-Based Experience**

  * No installation required for end users.
  * Works directly from the browser using WebRTC.

---

# 🛠️ Tech Stack

### Frontend

* Streamlit
* HTML/CSS
* Streamlit WebRTC

### Backend

* Python

### Computer Vision

* MediaPipe Pose Landmarker
* OpenCV

### AI

* Groq API (Llama 3.3 70B Versatile)
* Google Text-to-Speech (gTTS)

### Data Processing

* NumPy
* Pandas

### Database

* SQLite

---

# 📂 Project Structure

```text
AI-Real-Time-Gym-Coach/
│
├── backend/
│   ├── detectors/
│   ├── ml_models/
│   ├── services/
│   │   ├── auth/
│   │   ├── coaching/
│   │   ├── config/
│   │   ├── persistence/
│   │   ├── state/
│   │   ├── tracking/
│   │   ├── ui/
│   │   └── vision/
│   ├── static/
│   ├── main.py
│   ├── requirements.txt
│   └── .env
│
└── README.md
```

---

# ⚙️ Installation

## 1. Clone the repository

```bash
git clone https://github.com/ShivamBharti-29/AI-Real-Time-Gym-Coach.git
cd AI-Real-Time-Gym-Coach/backend
```

## 2. Create a virtual environment

```bash
python -m venv .venv
```

### Windows

```bash
.venv\Scripts\activate
```

### Linux / macOS

```bash
source .venv/bin/activate
```

---

## 3. Install dependencies

```bash
pip install -r requirements.txt
```

---

## 4. Configure environment variables

Create a `.env` file inside the `backend` folder.

```env
GROQ_API_KEY=YOUR_GROQ_API_KEY
```

---

## 5. Run the application

```bash
streamlit run main.py
```

---

# 📸 Application Workflow

1. Log in to your account.
2. Select an exercise.
3. Set the desired number of sets and repetitions.
4. Start the workout.
5. Allow camera access.
6. AI detects body posture.
7. Repetitions are counted automatically.
8. Form is analyzed continuously.
9. AI coach provides real-time voice feedback.
10. Workout statistics are saved automatically.

---

# 🧠 AI Form Analysis

The application evaluates exercise quality using multiple biomechanical metrics.

### Squats

* Knee Angle
* Back Angle
* Squat Depth

### Push-ups

* Elbow Angle
* Hip Alignment
* Body Alignment

### Biceps Curls

* Elbow Angle
* Shoulder Stability
* Swing Detection

### Shoulder Press

* Arm Extension
* Elbow Angle
* Back Arch Detection

### Lunges

* Front Knee Angle
* Torso Angle
* Balance Detection

---

# 🔊 AI Coaching Pipeline

```text
Camera
      │
      ▼
MediaPipe Pose Detection
      │
      ▼
Exercise Detector
      │
      ▼
Workout Metrics
      │
      ▼
Groq LLM Coach
      │
      ▼
Text-to-Speech
      │
      ▼
Voice Feedback
```

---

# 📦 Dependencies

* Streamlit
* Streamlit WebRTC
* MediaPipe
* OpenCV
* NumPy
* Pandas
* Groq SDK
* gTTS
* Python Dotenv

---

# 🎯 Future Improvements

* Multi-person pose tracking
* Additional exercise library
* Personalized workout recommendations
* Calorie estimation
* Heart-rate monitoring integration
* Mobile-friendly interface
* Cloud deployment
* Analytics dashboard
* Workout challenges and achievements

---

# 👨‍💻 Author

**Shivam Bharti**

GitHub: https://github.com/ShivamBharti-29

---

# 📄 License

This project is intended for educational and portfolio purposes.
