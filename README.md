# 👁️ Intelligent Surveillance System

A real-time, AI-driven video surveillance architecture engineered to automatically detect violent anomalies in live camera feeds. This system leverages a powerful combination of **Convolutional Neural Networks (CNNs)** for spatial feature extraction and **Long Short-Term Memory (LSTM)** networks for temporal sequence analysis, wrapped in a lightweight **Flask** web application.

## 🚀 Features
- **Real-Time Video Analytics:** Processes CCTV/webcam streams in real time.
- **Spatio-Temporal Detection:** Accurately maps both *what* is happening (CNN) and *how* it progresses over time (LSTM) to correctly identify violent interactions.
- **Flask Control Panel:** A clean, responsive web dashboard serving the processed video feed and displaying dynamic threat alerts.
- **High Accuracy Filtering:** Tuned to reduce false positives in highly populated areas.

## 🛠️ Technology Stack
- **Deep Learning Architecture:** Keras / TensorFlow (CNN + LSTM)
- **Computer Vision:** OpenCV (Video frame extraction and pre-processing)
- **Backend Framework:** Python & Flask
- **Frontend Dashboard:** HTML5, CSS3, JavaScript

## ⚙️ How It Works
1. **Frame Extraction:** OpenCV intercepts the live video feed and extracts numerical frame data at a standardized FPS.
2. **Spatial Mapping (CNN):** The Convolutional layer strips the raw frames down to their core structural features (edges, figures, movements).
3. **Temporal Mapping (LSTM):** The LSTM layer analyzes *sequences* of these structural frames to determine if the continuous motion constitutes a violent act.
4. **Alert Trigger:** If the confidence threshold is exceeded, the Flask API instantly emits a visual trigger to the web dashboard.

## 💻 Local Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/akg1998/Intelligent-Surveiilance-System.git
   cd Intelligent-Surveiilance-System
   ```

2. **Create a virtual environment:**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Run the Flask server:**
   ```bash
   python app.py
   ```
   *The dashboard will be available at `http://localhost:5000`.*

---
*Developed by [Akshay Ghavale](https://github.com/akg1998) as part of an advanced exploration into Applied Computer Vision.*
