# 🏜️ Off-Road Semantic Segmentation using PyTorch (ResNet34)

This project implements an efficient **semantic segmentation model** for off-road desert environments using **PyTorch** with a **ResNet34 encoder–decoder architecture**.  
The model achieves an impressive **0.8943 IoU**, outperforming typical baseline segmentation models.

---

## 🚀 Tech Stack
- Python  
- PyTorch  
- OpenCV  
- Albumentations  
- NumPy  
- Matplotlib  

---

## 📌 Project Highlights
- Achieved **0.8943 Intersection over Union (IoU)** on test set.  
- Based on a **ResNet34 encoder–decoder** segmentation architecture.  
- GPU-accelerated training for faster convergence and full-resolution data usage.  
- Custom augmentation pipeline improves generalization across unseen off-road terrains.  
- Handles sand, rocks, vegetation, and clutter-like textures effectively.

---

## 🧠 Model Architecture
- **Backbone:** ResNet34 (pretrained)  
- **Decoder:** Multi-stage upsampling with skip connections  
- **Output:** Pixel-wise classification mask  
- **Loss Function:** Cross Entropy  
- **Optimizer:** Adam  

Input Image → ResNet34 Encoder → Decoder → Segmentation Mask

---

## 📂 Project Structure
📁 Offroad-Segmentation-Project

---

## 📊 Training Summary
- **IoU Score:** 0.8943  
- **Epochs:** 30–50 (based on GPU)  
- **Batch Size:** 8–16  
- **Learning Rate:** 1e-4  

Includes:
- IoU curve  
- Loss curve  
- Sample mask predictions  

---

## ▶️ How to Run

### 1️⃣ Clone the repo

git clone https://github.com/Arbaz-hai/Offroad-Segmentation-Project
cd Offroad-Segmentation-Project

2️⃣ Install dependencies

pip install torch torchvision opencv-python albumentations matplotlib numpy

3️⃣ Train the model
python src/train.py

4️⃣ View predictions

Outputs are saved in:
results/predictions/

---
📦 Dataset

The dataset includes:
- Off-road desert environment images
- Pixel-wise annotated masks
-Generated using digital twin simulation

Supports multi-class segmentation:
- Sand
- Rock
- Ground clutter
- Vegetation
- Terrain obstacles

Future Improvements:

- Upgrade to DeepLabv3+, UNet++, or EfficientNet-based encoder
- Add mixed precision training (AMP)
- Use Dice Loss for imbalanced segmentation
- Deploy model with FastAPI

👤 Author: Arbaz
- GitHub: https://github.com/Arbaz-hai
- LinkedIn: https://www.linkedin.com/in/arbaz-sheikh-712408339

⭐ If you found this project helpful, please give the repository a star!

---

