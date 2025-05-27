# Classifying-Waste-Products
Classifying the Waste Products using the Transfer Learning

# ♻️ Waste Classification Using Transfer Learning (VGG16)

This project classifies waste images into **Recyclable** and **Organic** using transfer learning with a pre-trained VGG16 model.

## 📁 Dataset

The dataset is structured with two categories:
- `O` - Organic waste
- `R` - Recyclable waste

Download link: [Waste Classification Dataset](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/kd6057VPpABQ2FqCbgu9YQ/o-vs-r-split-reduced-1200.zip)

## 🧠 Model Summary

Two models were trained:
1. **Feature Extraction Model** (frozen base)
2. **Fine-Tuned Model** (last convolutional block trainable)

Both models use the pre-trained **VGG16** from Keras with custom dense layers on top.

## 📊 Evaluation

- Training and validation loss and accuracy plotted
- Test accuracy and classification report generated
- Visual inspection using prediction visualization on test images

## 📈 Results

- The model performs well on binary classification tasks.
- Fine-tuning improved accuracy compared to feature extraction alone.

## 🧪 Technologies Used

- Python
- TensorFlow / Keras
- Matplotlib
- scikit-learn

## 🔁 Transfer Learning Process

1. Load pre-trained VGG16 model (ImageNet weights)
2. Freeze early layers
3. Add custom dense layers on top
4. Train on waste classification dataset
5. Fine-tune selected layers
6. Evaluate performance

## 📸 Sample Output

### 🔍 Extract Features Model  
- **Loss & Accuracy Curves**  
  ![Extract Features Model - Loss Curve](extract_feat_loss_curve.png)  
  ![Extract Features Model - Accuracy Curve](extract_feat_accuracy_curve.png)

---

### 🧪 Fine-Tuned Model  
- **Loss & Accuracy Curves**  
  ![Fine-Tuned Model - Loss Curve](finetune_loss_curve.png)  
  ![Fine-Tuned Model - Accuracy Curve](finetune_accuracy_curve.png)






