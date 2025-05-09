
# 🏃‍♂️ Human Gait Detection System

An AI-powered physiotherapy tool for detecting gait abnormalities from walking videos using **MediaPipe**, **OpenCV**, and **Flask**. The system analyzes gait to identify issues such as slouching, limping, circumduction, and asymmetric arm swing, generating clear reports for physiotherapist review.

---

## 🔧 Features

- 🎥 Upload patient walking videos
- 🤖 Detect gait abnormalities using pose estimation
- 📊 Store patient data, videos, and analysis logs
- 📝 Generate detailed gait reports with improvement suggestions
- 🔐 Secure physiotherapist login and dashboard

---

## 🚀 Demo Flow

1. Login as physiotherapist
2. Add new patient
3. Upload walking video
4. Video is processed using MediaPipe Pose
5. Pose metrics are extracted and analyzed
6. Gait abnormalities are detected
7. Report is generated and viewable on dashboard

---

## 📁 Project Structure

```

human-gait-system/
│
├── static/                 # CSS, JS, and uploaded video files
├── templates/              # HTML templates (dashboard, report, etc.)
├── models/                 # Database models (SQLite)
├── gait\_analysis/          # Pose analysis and gait logic
│   ├── pose\_extractor.py   # Extract joint angles from video
│   └── gait\_analyzer.py    # Detect abnormalities
├── main.py                 # Main Flask application
├── requirements.txt        # Python dependencies
└── README.md               # Project documentation

````

---

## ⚙️ Setup Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/manishzzz/human-Gait-system.git
   cd human-Gait-system
```

2. **Create a virtual environment**

   ```bash
   python -m venv venv
   source venv/bin/activate   # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

4. **Run the Flask app**

   ```bash
   python main.py
   ```

5. **Open your browser and go to**

   ```
   http://127.0.0.1:5000/
   ```

---

## 🧠 Gait Abnormalities Detected

| Abnormality         | Detection Criteria                                  |
| ------------------- | --------------------------------------------------- |
| Slouch Posture      | Forward-leaning torso or misaligned spine posture   |
| Limp                | Asymmetry in step length or inconsistent hip motion |
| Circumduction       | Lateral leg arc during forward motion               |
| Arm Swing Asymmetry | Disparity in left/right arm angle/swing pattern     |

---

## 📝 Sample Report Includes

* Patient info (ID, name, age)
* Video snapshot and summary
* Detected gait issues (✓ or ✗)
* Pose metric data (joint angles, step count)
* Improvement suggestions for each issue

---

## 🛡️ Authentication

* Physiotherapist login via secure form
* Access restricted to authenticated users
* Add/edit/delete patient records and view gait reports

---

## 📚 Requirements

* Python 3.8 or higher
* Flask
* OpenCV
* MediaPipe
* SQLite3

Install all with:

```bash
pip install -r requirements.txt
```

---

## 📈 Future Enhancements

* 🧠 Integrate ML models for smarter anomaly detection
* 📱 Add mobile-friendly UI
* 📄 Export reports to downloadable PDF
* 🩺 Track recovery progress across multiple sessions

---

## 👨‍⚕️ Made for Physiotherapists

This project empowers physiotherapists with a data-driven tool to assess and monitor patient gait using simple walking videos and automated visual feedback.

---

## 📩 Contact

For questions or collaboration:
**[manishmaniyadhav@gmail.com](mailto:manishmaniyadhav@gamil.com)**

---

```

Let me know if you want badges (e.g. Python version, Flask, License) or a GitHub deploy-ready version with screenshots.
```
