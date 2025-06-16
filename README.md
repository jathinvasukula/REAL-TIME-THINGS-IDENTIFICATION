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


## 📥 Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/KOTAHARSHA25/YOLOv8-Image-and-Video-Processing-Application.git
   cd YOLOv8-Image-and-Video-Processing-Application
   ```
2. Create a virtual environment and activate it:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```
3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## 🎮 Usage
### Running the Application
```bash
python app.py --weights <model_weights> --source <input_source> --device <cpu/gpu>
```
Example:
```bash
python app.py --weights yolov8s.pt --source data/images --device cpu
```
### Command Line Arguments
- `--weights`: Path to the YOLOv8 model weights file (default is `yolov8s.pt`).
- `--source`: Directory path for input images or videos.
- `--device`: Specify the device to run the model on (`cpu` or `gpu`).

## 🖥️ User Interface
The project provides a user-friendly interface through HTML templates for interacting with the application and selecting different input sources and tasks.


## 📊 Model Usage
- For object detection: `python app.py --weights yolov8s.pt`
- For instance segmentation: `python app.py --weights yolov8s-seg.pt`
- For image classification: `python app.py --weights yolov8s-cls.pt`
- For human pose estimation: `python app.py --weights yolov8s-pose.pt`

## 🚀 Deployment
Run the `app.py` script with the desired model and input source to start the Flask application on the specified port (default is 5000).

## 💻 Source Code
Refer to `app.py` for the main application logic, including prediction functions and Flask routes.

## 🗂️ Project Structure

REAL-TIME-THINGS-IDENTIFICATION/
     REAL-TIME-THINGS-IDENTIFICATION/
│
├── app.py                      # Main Flask application
├── requirements.txt            # Python dependencies
├── README.md                   # Project documentation
├── LICENSE                     # Project license
│
├── static/                     # Static assets (CSS, JS, uploads)
│   ├── uploads/                # Uploaded files (image/video)
│   └── style.css               # Optional styling
│
├── templates/                  # HTML frontend templates
│   ├── index.html
│   ├── image.html
│   ├── video.html
│   ├── webcam.html
│   ├── yt.html
│   └── rtsp.html
│
├── yolov8_utils/               # YOLOv8 processing scripts
│   ├── detect.py               # Object detection logic
│   ├── classify.py             # Image classification logic
│   ├── segment.py              # Instance segmentation logic
│   ├── pose.py                 # Pose estimation logic
│   └── utils.py                # Shared utility functions
│
├── data/
│   └── raw/                    # Sample input files (keep under 100MB)
│
└── outputs/                    # Output results (annotated files)
    ├── images/
    ├── videos/
    └── logs/

## 💡 Use Cases
	•	🛡️ Smart Surveillance and Security
	•	🧑‍🏫 Educational Demos in AI & CV
	•	🚗 Traffic and Crowd Analysis
	•	📊 Data Labeling and Annotation
	•	🤖 Live AI Demonstrations

## 🤝 Contributing

Pull requests are welcome! If you have ideas or bug fixes, feel free to fork the repo, make changes, and submit a PR.

## ✅ Conclusion
This project showcases the YOLOv8 model's capabilities for various image processing tasks, providing accurate results for image classification, object detection, and human pose estimation.

## 🌟 Future Enhancements
Potential future enhancements include real-time processing, expanded training datasets, multi-camera support, advanced tracking algorithms, and complex interaction recognition.