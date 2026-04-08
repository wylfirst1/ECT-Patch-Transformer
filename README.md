# ECT-Patch-Transformer
A patch-based transformer method for an accurate reconstruction of ECT images.  The complex capacitance-to-image mapping is systematically decoupled into the capacitance-to-patch feature extraction and patch-to-image reconstruction.

# Patch-Transformer for Electrical Capacitance Tomography Reconstruction (IROS 2024)

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
*(Replace with your figure)*

```text
Capacitance → CNN Encoder → Patch Features → Transformer → Decoder → Image
