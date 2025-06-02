
# 📦 CIFAR-10 Image Classification with Transfer Learning

This project uses **transfer learning** on four popular pre-trained CNN models (`ResNet-18`, `AlexNet`, `EfficientNet-B0`, and `MobileNet-V2`) to classify images from the CIFAR-10 dataset.

In addition, the **Network In Network (NIN)** architecture is also implemented and used in this project.

---

## 🚀 Model Details

- For each pre-trained model, **two layers are unfrozen and fine-tuned**:
  - One deep/middle convolutional layer
  - The final classifier layer

- The final layer of each model is modified to output 10 classes (CIFAR-10).

- The **NIN model is fully trained from scratch** (no pre-trained weights).

---

## 📊 Data Augmentation

- Images resized to 224×224 pixels
- `AutoAugment` policy specific to CIFAR-10
- Augmented data merged with original training dataset to increase diversity

---

## 📈 Evaluation

For all models:

- Confusion Matrix for error analysis
- t-SNE visualization of learned feature embeddings
- Visualization of first convolutional layer filters

---

## 🛠 Training Setup

- Loss: CrossEntropyLoss
- Optimizer: Adam, lr=1e-4
- Epochs: 15 (adjustable)
- Training on GPU

---

## 💾 Model Saving

- Models saved after training for future use

---

## 🎯 Conclusion

This project demonstrates effective transfer learning strategies enhanced with data augmentation for CIFAR-10 classification using multiple architectures. It also includes training and evaluation of a from-scratch Network In Network (NIN) model for comparison.

