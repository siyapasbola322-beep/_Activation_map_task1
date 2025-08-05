---# Task 1: Activation Map Visualization for Age Detection

## 📌 Objective
The main goal of this task is to **visualize activation maps** to understand which parts of an image activate the filters of a Convolutional Neural Network (CNN) for **age detection**. This helps interpret what the model is learning and which image features are important.

---

## 📂 Folder Structure

## 📦 Dataset Used
- **UTKFace Dataset**
  - A large-scale face dataset with labels: age, gender, and ethnicity.
  - Used only for training the model for age detection.

---

## 🧠 Model Architecture
A custom CNN model built using Keras with TensorFlow backend. It includes:
- 3 Convolutional layers
- ReLU activation
- MaxPooling layers
- Fully connected Dense layers
- Final output layer with regression (age prediction)

---

## 🔥 Activation Map Visualization Approach
We used **Grad-CAM (Gradient-weighted Class Activation Mapping)** to visualize which image regions activate the CNN filters the most for age prediction.

Steps followed:
1. Load the trained CNN model (`age_model.h5`)
2. Pass a face image through the model
3. Extract gradients from the final convolutional layer
4. Generate a heatmap
5. Overlay the heatmap on the original image

---

## ▶️ How to Run

1. **Install Dependencies**
   ```bash
   pip install -r requirements.txt
