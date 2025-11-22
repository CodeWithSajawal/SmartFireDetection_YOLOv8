📦 Installation
1️⃣ Clone the Repository
git clone https://github.com/your-username/smart-fire-detection-system.git
cd smart-fire-detection-system

2️⃣ Install Dependencies
pip install -r requirements.txt

3️⃣ Download YOLOv8 Model
yolo download model=yolov8n.pt


(Or use your custom-trained fire model.)

🚀 How to Run
🔹 Run on Webcam
python detect.py --source 0 --model yolov8n.pt

🔹 Run on Video File
python detect.py --source fire_test.mp4 --model yolov8n.pt

🔹 Run on IP Camera (RTSP)
python detect.py --source rtsp://user:password@ip_address:port/stream --model yolov8n.pt

📊 Dataset

If you used a custom dataset:

Annotated using Roboflow or LabelImg

Trained on fire + smoke datasets

YOLOv8 format
