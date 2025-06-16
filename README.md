# Real-Time Things Identification

**Real-Time Things Identification** is an advanced web-based application powered by **YOLOv8** and built using **Flask**, designed to perform a wide range of real-time vision tasks. This includes:

- 🧠 Image Classification
- 🧱 Instance Segmentation
- 🧍 Human Pose Estimation
- 🎯 Object Detection

It supports a variety of input formats — from static images and video files to **live webcam feeds**, **YouTube videos**, and **RTSP camera streams** — making it ideal for real-world applications in automation, surveillance, education, and AI-based analysis.

---

## 🚀 Key Features

- 🔍 **Image Classification** – Identify the main object category in an image.
- 🧱 **Instance Segmentation** – Detect and mask individual objects.
- 🧍 **Human Pose Estimation** – Detect human body keypoints in real time.
- 🎯 **Object Detection** – Locate and label multiple objects simultaneously.
- 📥 **Multi-Input Support** – Works with:
  - 📸 Local Images
  - 🎞️ Video Files
  - 📷 Live Webcam Feeds
  - 📺 YouTube Videos
  - 📡 RTSP IP Camera Streams
- 💾 Save annotated results for later analysis
- 🌐 Simple and intuitive web interface using Flask

---

## 📦 Installation

### 1. Clone the Repository

```bash
git clone https://github.com/jathinvasukula/REAL-TIME-THINGS-IDENTIFICATION.git
cd REAL-TIME-THINGS-IDENTIFICATION

2. Create a Virtual Environment

python -m venv venv
source venv/bin/activate    # On Windows: venv\Scripts\activate

3. Install Dependencies

pip install -r requirements.txt

🧪 Run the Application
For object detection: python app.py --weights yolov8s.pt
For instance segmentation: python app.py --weights yolov8s-seg.pt
For image classification: python app.py --weights yolov8s-cls.pt
For human pose estimation: python app.py --weights yolov8s-pose.pt

🗂️ Project Structure

REAL-TIME-THINGS-IDENTIFICATION/
│
├── app.py
├── requirements.txt
├── README.md
├── LICENSE
├── .gitignore
│
├── static/           # CSS, JavaScript, etc.
├── templates/        # HTML pages
└── data/             # Input/output files (images/videos)

💡 Use Cases
	•	🛡️ Smart Surveillance and Security
	•	🧑‍🏫 Educational Demos in AI & CV
	•	🚗 Traffic and Crowd Analysis
	•	📊 Data Labeling and Annotation
	•	🤖 Live AI Demonstrations

🤝 Contributing

Pull requests are welcome! If you have ideas or bug fixes, feel free to fork the repo, make changes, and submit a PR.