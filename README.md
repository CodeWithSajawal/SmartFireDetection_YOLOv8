# SmartFireDetection_YOLOv8
This project implements a Smart Fire Detection System (SFDS) using YOLOv8 for real-time fire detection in smart cities 
The Smart Fire Detection System (SFDS) is an intelligent computer-vision–based solution designed to detect fire in real time using YOLOv8, one of the fastest and most accurate object detection models.
This project aims to support smart city safety infrastructure by enabling early fire detection through CCTV feeds, drones, or mobile cameras.

The system is built for:

Real-time monitoring

High accuracy fire recognition

Low latency alerting

Easy integration with IoT-based smart city platforms

🔥 Key Features

YOLOv8-based Fire Detection
Trained/finetuned YOLOv8 model to detect fire in indoor and outdoor environments.

Real-Time Video Processing
Supports live webcam feed, CCTV streams (RTSP), or video files.

High-Speed Inference
Powered by Ultralytics YOLOv8 for fast detection on both GPU and CPU.

Alert System (Optional)
Trigger notifications, alarms, or automated responses when fire is detected.

Modular Architecture
Easy to integrate with IoT systems, cloud dashboards, or smart city platforms.

🧱 Project Structure
📁 Smart-Fire-Detection-SFDS
│── 📁 dataset/          # Images/videos used for training
│── 📁 models/           # Trained YOLOv8 fire detection models
│── 📁 src/
│     │── detect.py      # Fire detection script
│     │── utils.py       # Helper functions
│── README.md            # Project documentation
│── requirements.txt     # Required Python libraries
│── train.py             # YOLOv8 training configuration

⚙️ Installation
1. Clone the repository
git clone https://github.com/yourusername/smart-fire-detection.git
cd smart-fire-detection

2. Install dependencies
pip install -r requirements.txt

3. Install YOLOv8 (Ultralytics)
pip install ultralytics

🎯 Training the Model

If you want to train your own fire detection model:

yolo detect train data=fire.yaml model=yolov8n.pt epochs=50 imgsz=640


fire.yaml contains:

Your dataset path

Class names (e.g., fire)
