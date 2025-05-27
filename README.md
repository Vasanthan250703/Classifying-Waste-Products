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

**Loss Curve:**  
![Extract_Features_Model_Loss_Curve](https://github.com/user-attachments/assets/c6091c65-69a6-410e-b346-4d1dff5b723d)

**Accuracy Curve:**  
![Extract_Features_Model_Accuracy_Curve](https://github.com/user-attachments/assets/733c5d74-732f-49af-ac3a-d7349110eabe)

**Sample Prediction:**  
![extract_features_model](https://github.com/user-attachments/assets/b3bdd9a6-83dd-4247-bb1b-dd48406cbfb0)

---

### 🧪 Fine-Tuned Model

**Loss Curve:**  
![Fine_Tuned_Model_Loss_Curve](https://github.com/user-attachments/assets/900990f4-aa7b-4374-8b26-c5568a43c78d)

**Accuracy Curve:**  
![Fine_Tuned_Model_Accuracy_Curve](https://github.com/user-attachments/assets/55f4097d-707b-423d-9965-147bf8266f29)

**Sample Prediction:**  
![fine_tuned_model](https://github.com/user-attachments/assets/01032901-36dd-4e66-b68a-c3337b50fb7f)







