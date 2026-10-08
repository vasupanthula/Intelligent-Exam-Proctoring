# 🛡️ Intelligent Exam Proctoring System — EduGuard AI

EduGuard AI is an **AI-powered intelligent exam proctoring system** designed to assist in monitoring online examinations and identifying potentially suspicious student behavior.

The project combines **Machine Learning, behavioral analysis, threshold-based classification, and rolling-window analysis** to improve the reliability of suspicious-activity detection while reducing unnecessary alerts.

---

## 📌 Project Overview

Online examinations require reliable monitoring to maintain academic integrity. Traditional manual monitoring can be time-consuming and difficult to scale, especially when a large number of students are taking examinations simultaneously.

EduGuard AI aims to provide an automated **decision-support system** that analyzes examination-related behavioral and system events and identifies patterns that may require further investigation.

The system does **not replace human proctors**. Detected events should be reviewed by an authorized human before any academic decision is made.

---

## 🎯 Objectives

- Detect potentially suspicious examination behavior.
- Analyze behavioral and system-related events.
- Apply Machine Learning for classification.
- Reduce false-positive alerts.
- Use a strict decision threshold for conservative detection.
- Apply rolling-window analysis to distinguish short events from persistent behavior.
- Evaluate model performance using standard classification metrics.
- Provide a foundation for an intelligent online examination monitoring system.

---

## 🚀 Key Features

### 🤖 Machine Learning Detection
Uses a trained Machine Learning model to classify examination-related behavior based on extracted features.

### 🎚️ Strict Decision Threshold
The system evaluates predictions using a **90% decision threshold** to make suspicious-activity alerts more conservative.

### 📊 Model Evaluation
The project evaluates the model using:

- Confusion Matrix
- Precision
- Recall
- F1-Score
- Precision-Recall analysis

### 🔄 Rolling-Window Analysis
Rolling-window analysis helps distinguish between short, isolated events and behavior that persists over multiple observation windows.

This can help prevent temporary actions such as brief movements or other short-duration events from immediately becoming suspicious alerts.

### 👨‍🏫 Human-in-the-Loop
The system is intended as a **decision-support tool**. Suspicious alerts should be verified by an authorized human proctor.

---

## 🏗️ System Workflow

```text
Student Examination
        │
        ▼
Behavior & System Events
        │
        ▼
Data Collection
        │
        ▼
Data Preprocessing
        │
        ▼
Feature Engineering
        │
        ▼
Machine Learning Model
        │
        ▼
Probability Prediction
        │
        ▼
90% Decision Threshold
        │
        ▼
Rolling-Window Analysis
        │
        ▼
Suspicious Activity Alert
        │
        ▼
Human Proctor Review
```

---

## 🧠 Machine Learning Approach

The project follows a standard Machine Learning workflow:

1. Data collection
2. Data preprocessing
3. Feature extraction
4. Training and testing split
5. Model training
6. Probability prediction
7. Threshold adjustment
8. Model evaluation
9. Suspicious-activity classification

The model generates probabilities for the target classes. A stricter threshold is then applied to reduce unnecessary suspicious-activity alerts.

---

## 📊 Evaluation

The model is evaluated using different decision thresholds.

### Default Threshold

```text
Threshold = 0.50
```

This provides the standard classification decision boundary.

### Strict Threshold

```text
Threshold = 0.90
```

The strict threshold requires a higher model confidence before generating a suspicious-activity prediction.

The project compares the two thresholds using confusion matrices and precision-recall analysis.

---

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Python | Core programming language |
| Pandas | Data processing |
| NumPy | Numerical operations |
| Scikit-learn | Machine Learning |
| Matplotlib | Data visualization |
| Jupyter Notebook | Development and experimentation |
| Machine Learning | Behavioral classification |
| Computer Vision | Visual monitoring components where applicable |

---

## 📁 Project Structure

```text
Intelligent Exam Proctoring/
│
├── Intelligent_Exam_Proctoring.ipynb
├── README.md
├── .gitignore
│
├── data/
│   ├── video_telemetry.csv
│   └── system_events.csv
│
├── models/
│   └── trained_model.pkl
│
└── results/
    ├── confusion_matrix.png
    └── precision_recall_curve.png
```

> The exact files and folders may vary depending on the final project implementation.

---

## 📈 Expected Benefits

- Automated examination monitoring support
- Reduced manual monitoring workload
- More consistent behavioral analysis
- Reduced unnecessary alerts through conservative thresholding
- Scalable foundation for online examination monitoring
- Data-driven evaluation of suspicious activity detection

---

## ⚠️ Limitations

This project is an academic/prototype implementation and should not be treated as a fully autonomous disciplinary system.

Machine Learning predictions can contain both **false positives and false negatives**. A high threshold can reduce false positives but may also increase false negatives.

Therefore, suspicious activity should always be reviewed by an authorized human proctor before taking academic action.

---

## 🔮 Future Enhancements

- Real-time webcam monitoring
- Advanced Computer Vision-based behavior detection
- Face detection and face verification
- Multiple-person detection
- Eye-gaze and head-pose analysis
- Audio anomaly detection
- Real-time alert dashboard
- Cloud deployment
- Database integration
- Student/proctor authentication
- Comprehensive audit logs
- Improved models using larger real-world datasets

---

## 💻 Installation

Clone the repository:

```bash
git clone https://github.com/vasupanthula/Intelligent-Exam-Proctoring.git
```

Navigate to the project:

```bash
cd Intelligent-Exam-Proctoring
```

Install the required Python packages:

```bash
pip install pandas numpy scikit-learn matplotlib jupyter
```

Start Jupyter Notebook:

```bash
jupyter notebook
```

Open the project notebook and run the cells sequentially.

---

## ▶️ Usage

1. Clone the repository.
2. Install the required dependencies.
3. Place the required datasets in the appropriate project directory.
4. Open the Jupyter Notebook.
5. Run the preprocessing steps.
6. Train the Machine Learning model.
7. Evaluate the model.
8. Compare the 50% and 90% thresholds.
9. Analyze the confusion matrix and precision-recall results.

---

## 📊 Results

The final results should be reported using the actual evaluation output generated by the project.

Important metrics include:

```text
Accuracy
Precision
Recall
F1-Score
False Positives
False Negatives
```

The **50% and 90% thresholds** can be compared to determine the most appropriate operating point for the intended use case.

---

## 👨‍💻 Author

**Panthula Vasu**

B.Tech — Computer Science & Engineering (AI & ML)

### Connect With Me

- GitHub: https://github.com/vasupanthula
- LinkedIn: https://www.linkedin.com/in/vasu-panthula-022107295

---

## 📜 Disclaimer

EduGuard AI is an academic project developed for educational and research purposes. The system provides predictions that should be treated as supporting evidence rather than definitive proof of examination misconduct. Final decisions should always involve appropriate human review.

---

⭐ **If you find this project useful, consider giving the repository a star!**
