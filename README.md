# Crop_Disease_Classification

#  Crop Disease Classification using Traditional ML & Deep Learning

This project compares traditional Machine Learning (SVM with HOG + PCA) and Deep Learning Sequential CNN and MobileNetV2 Transfer Learning for classifying crop diseases using leaf images from the PlantVillage dataset.

###  Project Goal
To evaluate which approach generalizes better for real-world plant disease detection and recommend a scalable, resource efficient solution for deployment in agricultural settings.

###  Models Implemented
- **Traditional ML**: Histogram of Oriented Gradients HOG + PCA + SVM  
- **Deep Learning**:
  - Custom Sequential CNN  
  - Functional API CNN  
  - MobileNetV2 Transfer Learning with ImageNet weights

###  Dataset
- Source: [PlantVillage – Kaggle](https://www.kaggle.com/datasets/emmarex/plantdisease)  
- ~54,000 images across multiple classes (e.g., Tomato Early Blight, Potato Late Blight, Healthy, etc.)  
- Preprocessed (128x128 resizing, normalization, augmentation)

### Results Summary
| Model            | Accuracy | Notes                                      |
|------------------|----------|--------------------------------------------|
| HOG + PCA + SVM  | ~76%     | Fast but poor generalization               |
| Sequential CNN   | ~88%     | Better learning from raw pixels            |
| MobileNetV2      | ~94%     | Best performance, deployable on mobile     |

### Highlights
- MobileNetV2 achieved highest test accuracy and minimal overfitting.
- Data augmentation (flip, zoom, rotate, shear) was critical for generalization.
- Full pipeline includes preprocessing, modeling, evaluation, and visualization.



### 📚 Author & Info
-  **Wengelawit Ayalew Solomon**
-  **October 10/19/2025**
-  Project for the course: *Machine Learning

###  Future Directions
- Real world testing on noisy leaf images
- Model deployment on Raspberry Pi  Android
- Integration with early warning systems for smallholder farmers
