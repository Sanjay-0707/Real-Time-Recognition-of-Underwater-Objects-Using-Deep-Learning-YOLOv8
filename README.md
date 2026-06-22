## 🐠 Underwater Detection - YOLOv8

**Real-Time Recognition of Underwater Objects Using Deep Learning**

### Description

This project implements a deep learning-based system for real-time detection and classification of underwater objects, specifically trained to identify **Fish** and **Human** presence in underwater environments. Using YOLOv8 (You Only Look Once), a state-of-the-art object detection framework, this system provides fast and accurate detection suitable for marine surveillance, underwater robotics, and research applications.

### Features

- ✅ **Real-Time Detection**: Live video stream processing from webcam
- ✅ **Dual Classification**: Detects and classifies two object types:
  - 🐟 Fish
  - 👤 Human
- ✅ **Optimized Model**: Pre-trained YOLOv8 model (best.pt) for underwater scenarios
- ✅ **Visual Output**: Bounding boxes with labels and color-coded detection (green for fish, red for humans)
- ✅ **Easy Integration**: Python-based with Jupyter notebook examples

### Project Structure

```
├── datasets/
│   ├── Training/
│   │   ├── Fish/
│   │   └── Human/
│   └── Testing/
│       ├── Fish/
│       └── Human/
├── best.pt              # Pre-trained YOLOv8 model
├── detection.ipynb      # Detection model training & evaluation
├── yD.ipynb            # Real-time detection with webcam
├── a.cs                # Utility encryption module
└── README.md
```

### Requirements

- Python 3.8+
- OpenCV (`cv2`)
- Ultralytics YOLOv8
- NumPy, Pandas, Matplotlib, Scikit-learn

### Installation

```bash
pip install ultralytics opencv-python numpy pandas matplotlib scikit-learn
```

### Usage

**Real-Time Detection (Webcam)**:
```python
from ultralytics import YOLO
import cv2

model = YOLO("./best.pt")

# Use the provided yD.ipynb notebook for live detection
```

Press `q` to quit the detection window.

### Dataset

The project includes labeled training and testing datasets with two categories:
- **Fish**: Underwater fish species
- **Human**: Divers or humans in underwater environment

### Model

The best.pt file contains the trained YOLOv8 model optimized for underwater object detection.

### Performance

- Detects and classifies underwater objects in real-time
- Provides bounding box coordinates and confidence scores
- Optimized for both accuracy and speed

### Applications

- 🤿 Underwater surveillance systems
- 🦾 Marine robotics
- 🔬 Aquatic research
- 🏊 Safety monitoring in swimming areas
- 📊 Marine biodiversity studies

