
# Patch-Transformer for Electrical Capacitance Tomography Reconstruction (IROS 2025)

## 🧠 Overview
This repository presents a Patch-Transformer based method for Electrical Capacitance Tomography (ECT) image reconstruction.

ECT is a highly ill-posed inverse problem, where low-dimensional capacitance measurements are used to recover high-resolution spatial permittivity distributions.  
To address this challenge, we propose a hybrid CNN-Transformer framework that effectively models both local features and global spatial dependencies.

This method enables high-quality reconstruction under noisy conditions and provides a potential solution for **robot near-field perception**, such as electronic skin and proximity sensing.

---

## 📄 Paper
**A Patch-Based Transformer Method for Electrical Capacitance Tomography Image Reconstruction**  
Accepted by *IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS 2025)*  

---

## 🚀 Key Contributions
- 🔹 Reformulate ECT as a patch-wise feature reconstruction problem  
- 🔹 Propose a CNN + Transformer hybrid architecture  
- 🔹 Introduce patch-level encoding with global attention modeling  
- 🔹 Achieve robust reconstruction under strong noise (10dB / 20dB)  

---

## 🏗️ Method Overview

### Pipeline
1. Input: 120-dimensional capacitance measurements  
2. CNN-based encoders extract local patch features  
3. Transformer aggregates global spatial relationships  
4. Decoder reconstructs high-resolution permittivity image  

---

## 🧩 Architecture
Capacitance → CNN Encoder → Patch Features → Transformer → Decoder → Image

## 📊 Results
| Metric | Value   |
| ------ | ------- |
| SSIM   | 0.95+   |
| PSNR   | 27.6 dB |
Robust under 10dB / 20dB noise
Outperforms traditional and deep learning baselines (e.g., ED-Net, WGAN)

(建议你放论文里的重建对比图)

## 📦 Installation
pip install -r requirements.txt

## ▶️ Usage
Training
python train.py
Testing
python test.py

## 📁 Dataset
Generated using COMSOL + MATLAB multi-physics simulation
45,000+ samples
Includes multi-object and varying-size scenarios

## 🔬 Applications
This method can be extended to:

🤖 Robot near-field perception (proximity sensing)
✋ Electronic skin for robotic manipulators
🧍 Human-robot interaction (safe distance estimation)

## 📌 Future Work
Integrate with real sensor data
Extend to multimodal perception (vision + capacitance)
Apply to robotic manipulation tasks

## 📫 Contact
Yuliang Wang
Email: wylfirst1@163.com
```text
Capacitance → CNN Encoder → Patch Features → Transformer → Decoder → Image
