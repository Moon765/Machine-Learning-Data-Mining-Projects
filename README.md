# Wildfire Detection Using Deep Learning  

## 📌 Project Overview  
Wildfires are a growing global concern, causing severe ecological damage, air pollution, and economic losses.  
This project explores **deep learning-based image classification** for wildfire detection, leveraging both **transfer learning** with pretrained models and a **custom CNN**.  

We compare the performance of **ResNet18, ResNet50, VGG16**, and a **custom CNN** on a wildfire image dataset, aiming to contribute to the development of **real-time wildfire monitoring and early warning systems**.  

---

## 🚀 Features  
- Binary classification: **Fire 🔥** vs **No Fire 🌲**  
- Implementation of **transfer learning** with pretrained CNNs  
- Custom-built CNN model for comparative analysis  
- **Data preprocessing & augmentation** (rotation, flips, color jitter, affine transforms)  
- **Early stopping** to mitigate overfitting  
- Evaluation metrics: **Accuracy, Precision, Recall, F1-score**  
- Visualization: training curves, confusion matrices, performance comparison  

---

## 📂 Dataset  
- Source: [Kaggle - The Wildfire Dataset](https://www.kaggle.com/datasets/elmadafri/the-wildfire-dataset)  
- Two classes: **Fire** and **No Fire**  
- Preprocessing steps:
  - Resize images → 256px (shorter side)  
  - Normalize using ImageNet mean/std  
  - Data augmentation (random rotations, flips, jitter, affine transforms)  

---

## 🏗️ Model Architectures  
1. **ResNet18** – best-performing pretrained model in this study  
2. **ResNet50** – deeper architecture for feature extraction  
3. **VGG16** – classical deep CNN with strong baseline performance  
4. **Custom CNN** – 3 convolutional blocks + fully connected classifier  

---

## ⚙️ Training Setup  
- **Optimizer:** Adam  
- **Loss Function:** Cross-Entropy Loss  
- **Batch Size:** 32  
- **Learning Rate Scheduler:** StepLR  
- **Max Epochs:** 40 (with early stopping patience = 5)  

---

## 📊 Results  
| Model      | Accuracy | Precision | Recall | F1-Score |
|------------|----------|-----------|--------|----------|
| ResNet18   | 70.15%   | 72.0%     | 68.5%  | 70.2%    |
| ResNet50   | 68.90%   | 70.5%     | 67.0%  | 68.7%    |
| VGG16      | 69.50%   | 71.0%     | 68.0%  | 69.5%    |
| Custom CNN | 65.30%   | 66.5%     | 64.0%  | 65.2%    |

✅ **ResNet18 achieved the best overall performance.**  
⚠️ Dataset biases and overfitting reduced generalization on unseen test data.  

---

## 📈 Visualizations  
- Training & validation loss curves  
- Confusion matrices for each model  
- Comparative accuracy charts  

---

## 🔮 Future Work  
- Advanced augmentation & synthetic data generation  
- Ensemble methods for higher robustness  
- Integration of **geo-spatial & temporal data**  
- Deployment in **real-time monitoring systems**  

---

## 📂 Folder Structure  
