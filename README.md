# 🍅 Tomato Price Prediction System using YOLO

An AI-powered system that uses the YOLO (You Only Look Once) object detection algorithm to detect tomatoes in images and predict their market price based on visual features like ripeness and quality.

## 🔍 Project Overview

Tomatoes vary in price depending on their ripeness, size, and condition. This system automates the price estimation process using image inputs. It's built using a YOLO model trained on tomato images and predicts price per kilogram after detecting tomatoes and analyzing their condition.

## 🧠 Technologies Used

- Python
- YOLOv5 / YOLOv8 (object detection)
- PyTorch
- OpenCV
- PIL
- Jupyter Notebook

## 📁 Repository Structure

```
├── best (2).pt                 # Trained YOLO model file
├── lakshay_ka_dost.ipynb       # Notebook with preprocessing, detection, and prediction
├── green-tomato.jpg            # Sample input image
└── README.md                   # Project documentation
```

## ⚙️ Setup Instructions

1. **Clone the Repository**
   ```bash
   git clone https://github.com/your-username/tomato-price-prediction.git
   cd tomato-price-prediction
   ```

2. **Install Requirements**
   > Create a virtual environment (recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate   # or venv\Scripts\activate on Windows
   ```

   > Then install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

   If `requirements.txt` isn't provided, install manually:
   ```bash
   pip install torch torchvision opencv-python pillow matplotlib
   ```

3. **Download YOLOv5/YOLOv8 (if not already)**
   ```bash
   git clone https://github.com/ultralytics/yolov5.git
   cd yolov5
   pip install -r requirements.txt
   ```

4. **Place the model file**
   - Move `best (2).pt` to the `yolov5` or project root directory.

## 🚀 Usage

Open the notebook:

```bash
jupyter notebook lakshay_ka_dost.ipynb
```

Steps:
1. Load the model (`best (2).pt`)
2. Upload an image of tomatoes (like `green-tomato.jpg`)
3. Run inference using YOLO
4. The notebook:
   - Draws bounding boxes
   - Analyzes tomato quality
   - Estimates the price per kg

## 📈 Model Info

- YOLO model trained on a dataset of tomatoes at various ripeness stages.
- Outputs include:
  - Bounding boxes of detected tomatoes
  - Category: Green, Semi-ripe, or Ripe
  - Estimated market price based on visual class

## 🧪 Sample Output

![Sample](./green-tomato.jpg)

*Model detects unripe tomato and outputs estimated price range.*

## 🔮 Future Work

- Support video and real-time webcam input
- Improve pricing algorithm based on market data APIs
- Expand to detect and price other vegetables/fruits
- Build a web/mobile interface

## 🤝 Contributors

- [Your Name]
- [Collaborator Names]

---

Feel free to star 🌟 the repo or contribute by creating a PR!
