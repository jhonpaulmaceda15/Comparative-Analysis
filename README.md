# Comparative-Analysis
# https://colab.research.google.com/drive/1tSeorvt6pEUmYjpiWEg8mqkPS8oxS1_K?usp=sharing

# GUIDE QUESTIONS (FINAL REFLECTION)

## A. Model Performance

### 1. Which pre-trained model achieved the highest accuracy? Why?

Among the three models, MobileNetV2 achieved the highest accuracy because it was able to extract image features more effectively while remaining lightweight and efficient. Its architecture helped improve generalization on the custom dataset.

---

### 2. Which model had the lowest performance? What could be the reason?

VGG16 had the lowest performance among the models tested. One possible reason is that it is a heavier and older architecture, which may not adapt as efficiently to the dataset compared to newer models.

---

### 3. How did loss values compare across models?

The model with the best accuracy also had the lowest loss values. Lower loss indicates that the model made fewer prediction errors during training and validation.

---

# B. Evaluation Metrics

### 4. Why is accuracy not enough to evaluate a model?

Accuracy alone does not show how well the model performs for each class. A model may have high accuracy but still perform poorly on certain classes. Metrics such as Precision, Recall, and F1-score provide a more detailed evaluation.

---

### 5. Which model had the best F1-score? What does it indicate?

ResNet50 achieved the best F1-score. This indicates that the model had a good balance between Precision and Recall, meaning it correctly identified images while minimizing false predictions.

---

### 6. How did Precision and Recall differ across models?

Some models achieved higher Precision but lower Recall, meaning they made fewer wrong predictions but missed some correct images. Other models had higher Recall but slightly lower Precision, meaning they detected more images but also produced more false predictions.

---

# C. Confusion Matrix Analysis

### 7. Which classes were frequently misclassified?

Classes with similar visual features were more likely to be misclassified. For example, categories with similar colors, shapes, or textures were sometimes confused by the models.

---

### 8. What patterns did you observe in the confusion matrix?

Most correct predictions appeared along the diagonal of the confusion matrix, which indicates good classification performance. Misclassifications mainly occurred between visually similar classes.

---

# D. ROC and AUC

### 9. Which model had the highest AUC score?

MobileNetV2 achieved the highest AUC score, showing strong classification capability across all classes.

---

### 10. What does AUC tell us about model performance?

AUC measures how well the model can distinguish between classes. A higher AUC score means the model performs better at separating correct and incorrect predictions.

---

# E. Explainability (Grad-CAM)

### 11. What did Grad-CAM reveal about model decision-making?

Grad-CAM showed which regions of the image influenced the model’s predictions. It helped visualize whether the model focused on the important object features.

---

### 12. Did the model focus on relevant image regions?

Yes, the improved models mainly focused on the correct object regions instead of the background, indicating that the models learned meaningful features.

---

### 13. Which model produced the most meaningful heatmaps?

ResNet50 produced the clearest and most focused heatmaps, showing stronger feature extraction and better interpretability.

---

# F. Model Comparison & Improvement

### 14. Which model would you recommend for deployment? Why?

MobileNetV2 is recommended for deployment because it achieved high accuracy while remaining lightweight and fast, making it suitable for real-world applications and mobile devices.

---

### 15. How can you further improve your best-performing model?

The model can be improved further by:

* Adding more training images
* Applying stronger data augmentation
* Fine-tuning deeper layers
* Increasing training epochs
* Using better image preprocessing techniques

---

# G. Real-World Application

### 16. How can your model be applied in real-world scenarios?

The model can be used in applications such as:

* Object recognition
* Medical image analysis
* Plant disease detection
* Security and surveillance systems
* Mobile image classification apps

---

### 17. What are the risks of deploying an inaccurate model?

An inaccurate model may produce wrong predictions, which can lead to incorrect decisions, reduced reliability, and poor user trust. In critical applications like healthcare or security, inaccurate predictions may cause serious problems.

---

### 18. How can this system be integrated into a mobile/web app?

The trained model can be deployed using frameworks such as:

* TensorFlow Lite for mobile applications
* TensorFlow.js for web applications
* APIs and backend servers for real-time image prediction systems
