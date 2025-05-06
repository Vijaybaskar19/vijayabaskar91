# Traffic Analytics with YOLOv8 & Flask

A real-time object detection, tracking, counting and speed estimation system built with YOLOv8, ByteTrack and a simple Flask web interface. Upload video files or stream from a camera, watch live annotated feeds, view per-class and per-region counts, and examine per-minute statistics.

---

## 🚀 Features

- **Object Detection & Tracking**  
  Detects people, bicycles, motorcycles, cars, buses and trucks via YOLOv8 + ByteTrack.  
- **Unique Instance Counting**  
  Maintains running tallies for each class (total) and within user-defined regions.  
- **Speed Estimation**  
  Pixel→meter conversion and FPS-based algorithm to display estimated km/h.  
- **Flask Web App**  
  - Upload local videos or use a webcam stream  
  - Live MJPEG feed with bounding boxes, IDs, counts & speeds  
  - Per-minute logging of total and region-based counts  
  - “Stats” page to review historical data  
- **Easy Configuration**  
  - Change detection classes, regions, ROI thresholds or camera source in code  
  - Adjust logging interval and output resolution  

---

## 📦 Requirements

Add the following to your `requirements.txt` (or install via `pip`):

```text
Flask>=2.0
ultralytics>=8.0
opencv-python>=4.5
numpy>=1.21
# CPU-only PyTorch to reduce disk usage:
--extra-index-url https://download.pytorch.org/whl/cpu
torch==2.0.1+cpu
