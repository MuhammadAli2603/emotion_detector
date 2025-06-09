# 🤖 Emotion Detector: Real‑Time Facial Expression Recognition

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MuhammadAli2603/emotion-detection/blob/main/test.ipynb)  
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)  
[![Python](https://img.shields.io/badge/python-3.8%2B-blue.svg)]()  
[![TensorFlow](https://img.shields.io/badge/TensorFlow-%3E%3D2.0-orange.svg)]()  
[![OpenCV](https://img.shields.io/badge/OpenCV-%3E%3D4.0-yellow.svg)]()  
[![Keras](https://img.shields.io/badge/Keras-%3E%3D2.3-red.svg)]()

---

## 🚀 Project Overview

An end‑to‑end **real‑time** emotion recognition system built with Deep Learning:

- **Backbone**: MobileNet pre‑trained on ImageNet, fine‑tuned on FER2013.  
- **Face Detection**: Haar cascade classifier (`ali.xml`).  
- **Inference**: Real‑time video capture + emotion prediction via OpenCV & Keras.  
- **Demo**: “Open in Colab” notebook runs everything—no local install required!

<details>
<summary>🎯 Why this matters</summary>

- **Interactive**: See live emotion labels overlaid on webcam feed.  
- **Compact**: MobileNet head achieves high accuracy with low latency.  
- **Extensible**: Swap in other models, add data augmentation, or expand emotion classes.  
</details>

---

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
Quickstart
1️⃣ Running Emotion Detection (Real-Time)
- Execute the `test.py` script:
  ```bash
  python test.py
  ```
- Ensure you have `emotion_model.h5` and `ali.xml` in the project root.

2️⃣ Train the Model
- Run the `train.py` script to train or fine-tune the model:
  ```bash
  python train.py
  ```

3️⃣ Install Dependencies
```bash
pip install -r requirements.txt
```
Model Architecture
We utilize MobileNet for the emotion detection model. MobileNet is chosen for its efficiency
and suitability for mobile deployment while maintaining accuracy. The final model consists of:
- Pre-trained MobileNet backbone
- Custom classification head for 5 emotion classes
Critical Considerations
- Class Imbalance: The FER2013 dataset may have an imbalance—consider class weighting.
- Model Accuracy: Experiment with other architectures or data augmentation to improve performance.
- Real-Time Constraints: Use adequate lighting and resolution for best results.
Contributing
1. Fork this repo
2. Implement improvements (add classes, enhance training, etc.)
3. Commit & push to your fork
4. Open a Pull Request with a description of your changes

License
This project is licensed under the MIT License. See LICENSE for details.
