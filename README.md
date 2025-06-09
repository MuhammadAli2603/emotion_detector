🤖 Emotion Detector: Real‑Time Facial Expression Recognition

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MuhammadAli2603/emotion-detection/blob/main/test.ipynb)  
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)  
[![Python](https://img.shields.io/badge/python-3.8%2B-blue.svg)]()  
[![TensorFlow](https://img.shields.io/badge/TensorFlow-%3E%3D2.0-orange.svg)]()  
[![OpenCV](https://img.shields.io/badge/OpenCV-%3E%3D4.0-yellow.svg)]()  
[![Keras](https://img.shields.io/badge/Keras-%3E%3D2.3-red.svg)]()

Project Overview
An end‑to‑end real‑time emotion recognition system built with Deep Learning:

- Backbone: MobileNet pre‑trained on ImageNet, fine‑tuned on FER2013.
- Face Detection: Haar cascade classifier (ali.xml).
- Inference: Real‑time video capture + emotion prediction via OpenCV & Keras.
- Demo: “Open in Colab” notebook runs everything—no local install required!
Why this matters
• Interactive: See live emotion labels overlaid on webcam feed.
• Compact: MobileNet head achieves high accuracy with low latency.
• Extensible: Swap in other models, add data augmentation, or expand emotion classes.
## 📂 Repository Structure

```text
emotion-detection/
├── test.py                ← Real‑time webcam demo
├── train.py               ← Training & fine‑tuning script
├── emotion_model.h5       ← Pre‑trained Keras model
├── ali.xml                ← Haar cascade face detector
├── requirements.txt       ← Python dependencies
├── README.md              ← Project overview & instructions
└── LICENSE                ← MIT License

````` 

Quickstart

1️⃣ Run Demo in Colab (No Setup!)
   1. Click Open in Colab above.
   2. Runtime → Run all to:
      - Download dependencies
      - Load face detector & model
      - Launch webcam demo in notebook

2️⃣ Run Locally
```
git clone https://github.com/MuhammadAli2603/emotion-detection.git
cd emotion-detection
python3 -m venv .venv && source .venv/bin/activate
pip install --upgrade pip
pip install -r requirements.txt

# Run real‑time demo:
python test.py
```
Usage Highlights
• Real‑Time Inference:
  ```bash
  python test.py
  ```

• Training:
  ```bash
  python train.py
  ```
Sample Results
Emotion    | Example Frame
-----------|----------------
Happy 😊   | docs/happy_sample.png
Sad 😢     | docs/sad_sample.png
Surprise 😲| docs/surprise_sample.png
Angry 😠   | docs/angry_sample.png
Critical Considerations
• Class Imbalance: FER2013 is skewed—consider class weighting or augmentation.
• Lighting & Resolution: Good lighting improves detection & classification accuracy.
• Model Choice: Try lighter backbones (e.g. MobileNetV2) for faster mobile deployment.
Contributing
1. Fork this repo
2. Create a feature branch (git checkout -b feature/awesome)
3. Make your changes & add tests
4. Commit & push to your fork
5. Open a Pull Request describing your improvements
License
This project is released under the MIT License. See LICENSE for details.
