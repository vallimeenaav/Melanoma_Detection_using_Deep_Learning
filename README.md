# 🩺 Melanoma Detection using Deep Learning  
**Early & Accurate Diagnosis of Skin Cancer with CNNs & Inception Networks**  

![Melanoma Detection](https://upload.wikimedia.org/wikipedia/commons/5/5f/Melanoma.jpg)  

## 🚀 Project Overview  
Melanoma is the deadliest form of skin cancer, and **early detection significantly improves survival rates**.  
This project implements **Deep Learning** models—including **Convolutional Neural Networks (CNNs)** and **Inception-based architectures**—to classify **dermoscopic images** as **benign or malignant** with **98.8% accuracy**.  

## 🏆 Key Achievements  
✔️ **98.8% classification accuracy** on **33,126** dermoscopic images  
✔️ **Precision & Recall of 0.95**, ensuring **low false negatives**  
✔️ **Extensive data augmentation** to combat class imbalance  
✔️ **Multi-model comparison**: CNN, DCNN, and Inception-based models  
✔️ **Patient-level metadata integration** for contextualized decision-making  

## 📂 Dataset  
- **Source**: [ISIC Skin Cancer Dataset](https://challenge.isic-archive.com/)  
- **Size**: 33,126 images (benign & malignant)  
- **Key Features**:  
  - Lesion Images 🖼️  
  - Patient Demographics (Age, Gender) 👤  
  - Anatomical Site of Lesion 📍  

## 🧠 Deep Learning Models  
| Model | Accuracy | Precision | Recall |  
|----------|------------|------------|------------|  
| **CNN** | 95.0% | 0.88 | 0.71 |  
| **DCNN** | 98.1% | 0.93 | 0.96 |  
| **Inception** | **98.8%** | **0.95** | **0.95** |  

> **🔬 Conclusion:** The **Inception model** emerged as the most **accurate & balanced** classifier, outperforming other architectures in melanoma detection.

## 🔄 Data Preprocessing  
✔ **Image Normalization** (Resized to 128x128)  
✔ **Data Augmentation** (Rotation, Flipping, Scaling)  
✔ **Feature Engineering** (Metadata Encoding)  
✔ **Handling Class Imbalance** (External dataset integration)  

## 📊 Exploratory Data Analysis (EDA)  
✔ **Body part impact analysis**: Most affected areas = torso, lower extremity  
✔ **Age Distribution**: Higher melanoma occurrence in **older patients**  
✔ **Gender Differences**: 57% of **malignant cases** were found in **males**  
✔ **Lesion Location**: Malignant lesions in **lower & upper extremities** more common in females  

## 🛠️ Model Architecture  
### **1️⃣ CNN Model**  
- 3 Convolutional Layers  
- Max-Pooling  
- Dense Layers  
- **Accuracy: 95%**  

### **2️⃣ Deep Convolutional Neural Network (DCNN)**  
- 7 Convolutional Layers  
- Batch Normalization  
- Fully Connected Layers  
- **Accuracy: 98.1%**  

### **3️⃣ Inception Model (Best Performance ✅)**  
- Multiple **Inception Modules**  
- Global Average Pooling  
- Dropout & Batch Normalization  
- **Accuracy: 98.8%**  

## 📌 How to Use  
### 1️⃣ Install Dependencies  
pip install -r requirements.txt
### 2️⃣ Train the Model
python train.py --model inception --epochs 50
### 3️⃣ Predict Melanoma
python predict.py --image sample.jpg

## 📈 Performance Metrics
<img width="594" alt="Screenshot 2025-02-02 at 4 39 36 PM" src="https://github.com/user-attachments/assets/f625ecb2-9b31-4703-8cb4-762854cd41b7" />

## 🚀 Future Work
- ✔ Explainable AI (XAI) for model interpretability
- ✔ Multi-class classification for different skin lesions
- ✔ Time-Series Analysis for disease progression monitoring

## 📜 References
- ISIC Melanoma Dataset
- Deep Learning in Skin Cancer Detection: [Nature Study](https://www.nature.com/articles/nature21056)

## 🤝 Contributing
Pull requests are welcome! If you'd like to contribute, feel free to fork this repository and submit a PR.
