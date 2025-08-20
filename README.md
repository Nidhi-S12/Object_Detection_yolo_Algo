# Object Detection using YOLO

This repository demonstrates **object detection** using the **YOLO (You Only Look Once)** algorithm.  
It uses **YOLOv3** with pre-trained weights on the COCO dataset to detect objects in images such as `demo.jpg` and `example.png`.

---

## 📌 Features

- Real-time object detection using YOLOv3  
- Detects 80+ common object classes (COCO dataset)  
- Easy-to-run Python scripts (`main.py`, `yolomod.py`)  
- Works on static images with bounding boxes and labels  

---

## 🛠️ Requirements


- Python **3.6+**
- Required Python libraries:
  - `opencv-python`
  - `numpy`

You can install dependencies with:

```bash
pip install -r requirements.txt

```


## 📂 Project Structure

```bash 
Object_Detection_yolo_Algo/
│── coco.names         # List of object class labels
│── yolov3.cfg         # YOLOv3 model configuration
│── yolomod.py         # YOLO helper functions
│── main.py            # Main script to run detection
│── demo.jpg           # Sample test image
│── example.png        # Another test image

⚠️ Note: The yolov3.weights file is not included due to size limits. You must download it manually.

```

## 📥 Download YOLO Weights

Download the pre-trained weights (~200 MB):
```bash
wget https://pjreddie.com/media/files/yolov3.weights
```
Place yolov3.weights in the project root directory.

## 🚀 Usage

Run detection on the sample image:

```bash
python yolomod.py
```

## ⚡ Customization

Modify confidence threshold and NMS (Non-Max Suppression) values in the script to adjust detection sensitivity.

Replace coco.names with your own dataset labels if fine-tuning.

Use custom-trained weights for specific object detection tasks.

## ❗ Troubleshooting

Error: Cannot find weights file
→ Make sure yolov3.weights is downloaded and placed in the repo root.

ImportError: cv2 not found
→ Install OpenCV:
```bash
pip install opencv-python
```
Slow detection
→ Use GPU-enabled OpenCV/DNN or try lighter models like yolov3-tiny.

## 🤝 Contributing

Fork this repo

Create your feature branch: git checkout -b feature-name

Commit changes: git commit -m "Added new feature"

Push branch: git push origin feature-name

Open a Pull Request

## 📜 License

This project is licensed under the MIT License – feel free to use and modify.

