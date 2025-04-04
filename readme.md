# Comparative Analysis of Pretrained ImageNet Models for Static Hand Gesture Recognition

## 📌 Overview
This repository contains a detailed comparative analysis conducted on **15 state-of-the-art CNN pretrained ImageNet models** for character-level static hand gesture recognition using the **Sign Language Gesture Images Dataset**.

## 🎯 Objectives
- Evaluate and compare the performance of pretrained ImageNet models.
- Identify the most accurate, efficient, and robust models for static hand gesture recognition.
- Provide insights to guide model selection for real-world Human-Computer Interaction (HCI) applications.

## 🚀 Models Evaluated

| EfficientNet Family     | ResNet Family       | VGG Family | MobileNet Family    | DenseNet Family | ConvNeXt Family |
|-------------------------|---------------------|------------|---------------------|-----------------|-----------------|
| EfficientNetV2L         | ResNet50            | VGG16      | MobileNetV2         | DenseNet121     | ConvNeXtBase    |
| EfficientNetB0          | ResNet101           | VGG19      | MobileNetV3Large    | DenseNet169     | ConvNeXtXLarge |
| EfficientNetV2S         | ResNet152           |            |                     | DenseNet201     |                 |

## 🗃️ Dataset
- **Name**: [Sign Language Gesture Images Dataset](https://www.kaggle.com/datasets/ahmedkhanak1995/sign-language-gesture-images-dataset)
- **Size**: 55,500 images (37 classes, including letters, numbers, and space)
- **Image Dimension**: 50×50 pixels

## 🛠️ Repository Structure
```
CAPIMSHGR/
├── code/                   # All model implementations
│   ├── [model]_[author].ipynb
│   └── ...
├── dataset/                # Dataset files
│   └── dataset.zip
├── docs/                   # Reports and documentation
│   └── readme.md
└── README.md               # Project overview (you are here)
```

## 🚧 Instructions for Contributors
- Download notebook from Kaggle.
- Rename the notebook to `[model]_[author].ipynb` format (e.g., `vgg19_adib.ipynb`).
- Place notebooks into the `code` folder.
- Commit each notebook separately for clarity and maintainability.

> ⚠️ **Please do not modify or delete other contributors' files.**

## 🔬 Methodology
- **Preprocessing**: Data normalization, augmentation, stratified data splitting (60%-20%-20%).
- **Training Strategy**: Transfer learning, fine-tuning final layers, and extensive model evaluation.
- **Evaluation Metrics**: Accuracy, Precision, Recall, F1-score.
- **Interpretability Techniques**: Grad-CAM, LIME, t-SNE visualization.

## 📈 Key Findings
- **Highest Accuracy**: `ConvNeXtXLarge` (99.63% Top-1 accuracy).
- **Balanced Choice**: `EfficientNetB0`, `MobileNetV2` (Optimal for resource-constrained environments).

| Recommended for                 | Model(s)                         |
|---------------------------------|----------------------------------|
| Highest Accuracy                | ConvNeXtXLarge, VGG19            |
| Best Efficiency (Edge Devices)  | EfficientNetB0, MobileNetV2      |
| Balanced Performance            | ResNet50, EfficientNetV2S        |

## 🎨 Visual Insights
- **Grad-CAM heatmaps**: Highlight crucial areas for gesture recognition.
- **t-SNE plots**: Demonstrate clear clustering between gesture classes.

## 📖 Full Report
- The detailed PDF report is available in the [`docs`](./docs) directory.

## 💬 Contributors
- **Adib Sakhawat** - 210042106
- **Md Hasibur Rahman** - 210042107
- **Minhajul Abedin** - 210042148
- **Nabila Islam** - 210042111
- **Nazifa Tasneem** - 210042114

## 🙌 Acknowledgments
Special thanks to the Kaggle platform for providing computational resources for the experiments.

---

✨ **Happy Exploring!**

_For any queries or further collaboration, please contact the contributors directly._
