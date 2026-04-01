# Sign Language Recognition (SLR) System

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![Deep Learning](https://img.shields.io/badge/DL-CNN%20%7C%20LSTM%20%7C%20I3D-orange.svg)](https://en.wikipedia.org/wiki/Deep_learning)
[![Status](https://img.shields.io/badge/Status-Completed-green.svg)]()

A comprehensive system designed to bridge the communication gap between the hearing-impaired and the general population. This project utilizes vision-based and sensor-based deep learning models to recognize both static (alphabets/digits) and dynamic (word-level) sign gestures.

---

## 🌟 Features

- **Static Gesture Recognition:** Uses high-accuracy CNN models to recognize letters from the MNIST and custom alphabet datasets.
- **Dynamic Gesture Recognition (Leap Motion):** Captures 3D fingertip coordinates in real-time and interprets them using LSTM networks to maintain temporal context.
- **Continuous Sign Recognition (Video-Based):** Employs the **I3D (Inflated 3D)** model fine-tuned on the **WLASL 2000** dataset for full-word ASL recognition.
- **Transfer Learning Integration:** Leverages **Inception V3** pre-trained on ImageNet to maximize classification accuracy with fewer training samples.

---

## 📁 Project Structure

```bash
📦 Sign-Language-Recognition
 ┣ 📂 Static Gesture Detection   # CNN-based recognition for alphabets and digits
 ┣ 📂 Dynamic_Leap Motion       # LSTM models using Leap Motion Controller data
 ┣ 📂 Dynamic_WLASL            # I3D video classification architecture (WLASL 2000)
 ┣ 📜 docs.md                  # Comprehensive Technical Documentation
 ┣ 📜 Final Report.pdf          # Full academic report
 ┣ 📜 Presentation.pdf         # Project slides
 ┗ 📜 README.md                # Project overview and quick start
```

---

## 📊 Results Summary

| Approach    | Model        | Dataset       | Test Accuracy |
| :---------- | :----------- | :------------ | :------------ |
| **Static**  | 5-Layer CNN  | Alphabets     | **99.8%**     |
| **Static**  | Inception V3 | Words + Alph. | **94.8%**     |
| **Dynamic** | LSTM         | Leap Motion   | **92.9%**     |
| **Video**   | I3D (Top-10) | WLASL 2000    | **81.0%**     |

_For detailed analysis and methodology, please refer to [docs.md](./docs.md)._

---

## 🛠️ Technology Stack

- **Languages:** Python
- **Deep Learning:** TensorFlow/Keras, PyTorch
- **Computer Vision:** OpenCV, Mediapipe
- **Sensors:** Leap Motion Controller APIs
- **Datasets:** MNIST, WLASL 2000, Custom ASL Alphabet datasets

---

## 📝 Usage

To explore the specific components of the project:

1.  **Static Recognition:** Navigate to `Static Gesture Detection/` for CNN implementation details.
2.  **Leap Motion:** Review `Dynamic_Leap Motion/` for LSTM sequence processing.
3.  **WLASL Video Models:** Check `Dynamic_WLASL/` for the I3D fine-tuning process.

---

## 🤝 Project Background

According to the WHO, over 7% of the world’s population has hearing impairment. This project aims to provide a data-driven solution that enables seamless communication through automated sign-to-text translation.

## Created & Complied by Narmada Natarajan (23BAI11088) VIT Bhopal University