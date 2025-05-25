# 🛣️ Road Damage Classification Using ResNet50, InceptionV3, and VGG16  
*A Deep Learning Approach for Multi-Label Road Damage Detection*

This project focuses on developing a robust multi-label classification system to identify and categorize various types of road damage. By leveraging pre-trained deep learning models—**ResNet50**, **InceptionV3**, and **VGG16**—we aim to automate the process of road damage detection from a dataset of 4,000 TIF images, each labeled with 26 different damage types. The system predicts severity on a scale of 0 to 5, aiding in road maintenance planning and resource allocation.

---

## 🎯 Objectives

- **Develop a Multi-Label Classification System**  
  Predict multiple road damage types simultaneously using transfer learning.

- **Model Comparison**  
  Evaluate ResNet50, InceptionV3, and VGG16 based on accuracy, precision, recall, and F2-score.

- **Insightful Visualizations**  
  Generate loss curves, confusion matrices, and training metrics to compare model performance.

---

## 🗂️ Dataset

- **Images**: 4,000 `.TIF` images of roads  
- **Labels**: 26 damage categories per image, each rated from 0 (none) to 5 (severe)

> 📩 For access to the dataset, please email: `25100147@lums.edu.pk`

---

## 🧠 Methodology

### 🔍 Data Preprocessing
- Read and process multi-label `.TIF` road images
- Resize and normalize input images
- Prepare label tensors for 26-class severity scores

### 🤖 Model Architectures

| Model       | Highlights                                                 |
|-------------|------------------------------------------------------------|
| **ResNet50**   | Deep residual architecture helps mitigate vanishing gradients |
| **InceptionV3** | Auxiliary classifiers improve gradient flow during training  |
| **VGG16**       | Simpler and deeper, but more resource-intensive              |

---

## 🏋️‍♂️ Training & Evaluation

- **Loss Function**: CrossEntropyLoss  
- **Optimizer**: Adam  
- **Validation** after each epoch  
- **Metrics Tracked**: Accuracy, Precision, Recall, F2-score

### 📊 Visualizations
- 📉 Loss Curves for training vs. validation
- 📋 Confusion Matrices for detailed error analysis
- 📈 Metric Trends across epochs for all models

---

## 🧪 Hyperparameter Tuning

- Tuned:
  - Learning Rates
  - Batch Sizes
  - Layer Freezing/Unfreezing  
- Goal: Maximize validation F2-score

---

## 🚀 Deployment Potential

- Application of best model in:
  - Automated road inspection systems
  - Government road maintenance scheduling
  - Scalable infrastructure monitoring

---

## 🏁 Results Summary

| Model        | Strengths                         | Notes                                     |
|--------------|-----------------------------------|-------------------------------------------|
| **ResNet50**   | Balanced across all metrics        | Efficient training and decent generalization |
| **InceptionV3**| Best **Precision** & **F2-score**  | Benefit from auxiliary classifiers         |
| **VGG16**      | High **Recall**                    | Computationally heavier than others        |

---

## 📌 Conclusions

- InceptionV3 shows the best performance in precision and F2-score.
- All models demonstrate the viability of deep learning for road damage detection.
- This approach is highly scalable and offers real-world impact in smart city initiatives.

---

## 🔮 Future Work

- 🔓 **Unfreeze More Layers** to fine-tune deeper representations
- 📈 **Expand Dataset** for better generalization
- 🌐 **Deploy** model to mobile/web for real-time road damage detection

---

## 👨‍💻 Author & Contact

Developed by **Muhammad Saad Haroon**  
For dataset or inquiries, contact: `25100147@lums.edu.pk`

---

> *Built with PyTorch and passion for practical AI.*
