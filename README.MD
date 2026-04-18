# 🪖 Helmet Detection using YOLOv8

This project detects:
- ✅ Helmet (Yes)
- ❌ No Helmet
- 🔢 Number Plate

Built using **YOLOv8 (Ultralytics)** and trained on a custom dataset.

---

## 📁 Project Structure

```
project-folder/
│── input_images/
│── results/
│── best.pt
│── data.yaml
│── helmet_detection.ipynb
│── README.md
```

---

## 🚀 How to Run

```python
from ultralytics import YOLO

model = YOLO("best.pt")

model.predict(
    source="input_images",
    save=True
)
```

---

## 📊 Dataset Info

- Classes: `Helmet`, `No Helmet`, `Number Plate`
- Format: YOLOv8
- Source: Roboflow

---

## 🧠 Training Details

- Model: YOLOv8n (Nano - fast and lightweight)
- Epochs: 5
- Image Size: 416
- Batch Size: 16
- Device: GPU (recommended)

---

## 📸 Sample Results

### Before Detection
![Input](input_images/10_mp4-0003_jpg.rf.d8078de8bfa7c8051cab5a0b540e5d4a.jpg)

### After Detection
![Output](results/10_mp4-0003_jpg.rf.d8078de8bfa7c8051cab5a0b540e5d4a.jpg)

---

## 🔧 Optional Improvements

- Increase epochs for better accuracy  
- Add real-time detection (video/webcam)  
- Deploy using Streamlit or Flask  
- Expand dataset  

---

## 📌 Notes

- Ensure correct file paths when running locally  
- GPU speeds up training significantly  
- Outputs are saved in `runs/detect/`  

---

## ✅ Final Checklist

- [x] README.md correct  
- [x] Notebook uploaded  
- [x] Model (`best.pt`) included  
- [x] Images added  

---

💡 Simple and fast helmet detection using YOLOv8.