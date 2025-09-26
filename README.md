# Fashion_MNIST_Metric_Calculation
A deep learning model built with TensorFlow to classify Fashion MNIST images into 10 clothing categories, evaluated using accuracy, confusion matrix, and classification metrics.

# Fashion MNIST Classification with TensorFlow  

## 📌 Project Overview  
This project demonstrates how a deep learning model built using **TensorFlow & Keras** can classify images from the **Fashion MNIST dataset**. The dataset consists of grayscale images of clothing and accessories, and the task is to predict the correct class out of 10 categories.  

The model is trained on the dataset, evaluated using multiple metrics, and visualized through plots and a confusion matrix to understand its strengths and weaknesses.  

---

## 🛠 Dataset: Fashion MNIST  
- **Size:** 70,000 images (60,000 training + 10,000 testing)  
- **Image Dimensions:** 28 × 28 pixels, grayscale  
- **Classes (10 categories):**  
  - 0️⃣ T-shirt/top  
  - 1️⃣ Trouser  
  - 2️⃣ Pullover  
  - 3️⃣ Dress  
  - 4️⃣ Coat  
  - 5️⃣ Sandal  
  - 6️⃣ Shirt  
  - 7️⃣ Sneaker  
  - 8️⃣ Bag  
  - 9️⃣ Ankle boot  

Each label is mapped to a fashion item to make the predictions more interpretable.  

---

## 🧠 Model Architecture  
The model is a **Sequential Neural Network** with the following layers:  

1. **Input Layer:** Accepts 28x28 images  
2. **Flatten Layer:** Converts 2D images into a 1D vector  
3. **Dense (512 units, ReLU):** Fully connected hidden layer  
4. **Dense (128 units, ReLU):** Second hidden layer  
5. **Dense (10 units, Softmax):** Output layer with probability distribution across 10 classes  

**Optimizer:** Stochastic Gradient Descent (SGD)  
**Loss Function:** Categorical Crossentropy  
**Metrics:** Accuracy  

---

## 📊 Metrics & Evaluation  
The model was trained for **20 epochs** with a **90/10 train-validation split**.  

Evaluation methods included:  
- 📉 **Loss & Validation Loss Plots:** To track training and validation progress  
- ✅ **Accuracy Score:** Overall model performance on unseen test data  
- 🔢 **Confusion Matrix:** To visualize per-class performance and misclassifications  
- 📑 **Classification Report:** Precision, recall, and F1-score for all 10 classes  

---

## 🔍 Key Insights  
- The model can successfully identify fashion items, but some classes (like **Shirt vs T-shirt/top** or **Coat vs Pullover**) are prone to misclassification due to visual similarities.  
- Normalization of pixel values (0–1 scaling) significantly improves performance.  
- Evaluating with both **accuracy** and **confusion matrix** helps in understanding where the model struggles.  

---

## ✅ Conclusion  
This project highlights how deep learning models can classify clothing items using **Fashion MNIST**. While overall accuracy is high, the misclassification cases reveal areas where the model can be improved (e.g., **CNNs, data augmentation, or advanced optimizers**).  
