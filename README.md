# 🖥️ CIFAR-10 Image Classifier

A deep-learning project for classifying images from the **CIFAR-10 dataset** using multiple pre-trained models and a custom network built from scratch with PyTorch.  
The project demonstrates the performance of modern architectures, fine-tuning, and advanced data visualization techniques.

---

## 📦 Models Used
The project evaluates and compares the performance of the following architectures:

- **ResNet18**  
- **ResNet50**  
- **MobileNet**  
- **EfficientNet**  
- **Custom Network-in-Network (from scratch)**  

> Pre-trained models were fine-tuned on CIFAR-10 for improved performance.

---

## 🧪 Techniques & Methods

### ✔ Data Handling
- Dataset divided into:
  - **Training set**  
  - **Validation set**  
  - **Test set**

### ✔ Data Preprocessing & Analysis
- Visualizing sample images from dataset  
- Class distribution analysis  
- Outlier detection  
- Dimensionality reduction (for visualization and analysis)  
- Confusion matrix analysis  
- **Visualizing first convolutional layer filters** (`visualize_first_conv_filters`)  

### ✔ Model Training
- Fine-tuning pre-trained models  
- Training from scratch (Network-in-Network) using PyTorch  

---

## 🗂 Dataset

- **CIFAR-10**: 60,000 32x32 color images in 10 classes (airplane, automobile, bird, cat, deer, dog, frog, horse, ship, truck)  
- Dataset link: [CIFAR-10](https://www.cs.toronto.edu/~kriz/cifar.html)

---

## 📊 Results & Summary

> These models, despite some of them hiding input images and having a large number of parameters, were able to classify the data quite well because CIFAR-10 is a well-known dataset.  
> MobileNet and EfficientNet achieved higher accuracy due to their complex architectures, allowing the model to engage more deeply with the data.  
> ResNet-18, with residual connections, outperformed AlexNet in handling vanishing gradients.  
> Challenges were observed in distinguishing dogs and cats due to visual similarity, which can be mitigated by deeper networks and longer training.  

- EfficientNet and MobileNet achieved the highest accuracy  
- ResNet-18 showed strong performance among residual networks  
- Custom Network-in-Network demonstrates PyTorch implementation from scratch  

---

## 🔧 Installation & Usage

### 1️⃣ Clone the repository
```bash
git clone https://github.com/USERNAME/cifar10-classifier.git
cd cifar10-classifier
