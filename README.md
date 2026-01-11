# 🌿 PlantVillage: Agricultural Disease Detection System

![Python](https://img.shields.io/badge/Python-3.9%2B-blue)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange)

## 📌 Project Overview
This project is a deep learning initiative designed to detect plant diseases from leaf images with high accuracy. By leveraging **Transfer Learning** with the **MobileNetV2** architecture, the system is optimized for efficiency, making it suitable for mobile and edge device applications.

Unlike standard "Black Box" models, this project integrates **Explainable AI (XAI)** using **Grad-CAM**, allowing us to visualize the specific regions of the leaf that the model focuses on to identify diseases.

## 🚀 Key Features
- **Efficient Architecture:** Uses MobileNetV2 (Pre-trained on ImageNet) for low latency.
- **Explainable AI (XAI):** Integrated **Grad-CAM** to generate heatmaps, visualizing the model's "Region of Interest" (ROI).
- **Robust Data Pipeline:** Implements physical data splitting (Train/Val/Test) to prevent data leakage.
- **Data Augmentation:** Real-time image augmentation to improve model generalization.
- **Wide Coverage:** Capable of identifying diseases across 38 different classes (14 crop species).

## 📂 Data Setup (Crucial Step)
The dataset is large and is **not included** in this repository. Please follow these steps to set up the data:

1.  **Download:** Go to [Kaggle - PlantVillage Dataset](https://www.kaggle.com/datasets/abdallahalidev/plantvillage-dataset) and download the archive.
2.  **Extract:** Unzip the downloaded file.
3.  **Organize:** Move the extracted `PlantVillage` folder into the `data/raw/` directory of this project.
    * **Target Path:** `YourProject/data/raw/PlantVillage/`
    * *Check:* Inside this folder, you should see subfolders like `Tomato___Bacterial_spot`, `Pepper__bell___healthy`, etc.

## 🛠 Installation & Usage

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/YOUR_USERNAME/PlantVillage-DeepLearning-System.git](https://github.com/YOUR_USERNAME/PlantVillage-DeepLearning-System.git)
    cd PlantVillage-DeepLearning-System
    ```

2.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

3.  **Run the Jupyter Notebook:**
    Navigate to the `notebooks/` directory and run the main notebook to train the model or test it.
    ```bash
    jupyter notebook notebooks/PlantDisease_Detection_MobileNetV2.ipynb
    ```

## 📊 Methodology
1.  **Data Engineering:** Using `split-folders` to partition data into Training (80%), Validation (10%), and Test (10%) sets.
2.  **Transfer Learning:** Freezing the base layers of MobileNetV2 to retain learned features and fine-tuning the classification head.
3.  **Visualization:** Generating Grad-CAM heatmaps to validate that the model is detecting biological features (e.g., lesions) rather than background noise.

## 🚀 Key Features
- **Lightweight Architecture:** Uses MobileNetV2 (Pre-trained on ImageNet) for low latency and small model size.
- **Explainable AI (XAI):** Integrated **Grad-CAM** to generate heatmaps, visualizing the model's "Region of Interest" (ROI).
- **Robust Data Pipeline:** Implements physical data splitting (Train/Val/Test) to prevent data leakage.
- **Data Augmentation:** Real-time image augmentation to improve model generalization.
- **38 Classes:** Capable of identifying diseases across 14 different crop species.

## 📂 Data Setup (Crucial Step)
The dataset is large and is **not included** in this repository to keep the repo lightweight. Please follow these steps to set up the environment:

1.  **Download:** Go to [Kaggle - PlantVillage Dataset](https://www.kaggle.com/datasets/abdallahalidev/plantvillage-dataset) and download the archive.
2.  **Extract:** Unzip the downloaded file.
3.  **Organize:** Move the extracted `PlantVillage` folder into the `data/raw/` directory of this project.
    * **Target Path:** `YourProject/data/raw/PlantVillage/`
    * *Check:* Inside this folder, you should see subfolders like `Tomato___Bacterial_spot`, `Pepper__bell___healthy`, etc.

## 🛠 Installation & Usage

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/YOUR_USERNAME/PlantVillage-DeepLearning-System.git](https://github.com/YOUR_USERNAME/PlantVillage-DeepLearning-System.git)
    cd PlantVillage-DeepLearning-System
    ```

2.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

3.  **Run the Jupyter Notebook:**
    Navigate to the `notebooks/` directory and launch the main notebook to train the model or run inference.
    ```bash
    jupyter notebook notebooks/PlantDisease_Detection_MobileNetV2.ipynb
    ```

## 📊 Methodology
The project follows a rigorous engineering pipeline:
1.  **Data Engineering:** Using the `split-folders` library to partition data into Training (80%), Validation (10%), and Test (10%) sets.
2.  **Transfer Learning:** Freezing the base layers of MobileNetV2 to retain learned features and fine-tuning the classification head.
3.  **Evaluation:** Using Confusion Matrices and Categorical Crossentropy Loss to measure performance.
4.  **Visualization:** Generating Grad-CAM heatmaps to validate biological features (e.g., detecting lesions vs. background noise).

## 📝 Technical Report (Turkish)
For a comprehensive technical breakdown and detailed report in Turkish, please refer to the [TECHNICAL_REPORT_TR.md](TECHNICAL_REPORT_TR.md) file included in this repository.

## 🤝 Contribution
This is an open-source project developed for educational and portfolio purposes. Feedback, issues, and pull requests are welcome.

## 📜 License
Distributed under the MIT License. See `LICENSE` for more information.

    cd PlantVillage-DeepLearning-System
    ```

2.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

3.  **Run the Jupyter Notebook:**
    Navigate to the `notebooks/` directory and launch the main notebook to train the model or run inference.
    ```bash
    jupyter notebook notebooks/PlantDisease_Detection_MobileNetV2.ipynb
    ```

## 📊 Methodology
The project follows a rigorous engineering pipeline:
1.  **Data Engineering:** Using the `split-folders` library to partition data into Training (80%), Validation (10%), and Test (10%) sets.
2.  **Transfer Learning:** Freezing the base layers of MobileNetV2 to retain learned features and fine-tuning the classification head.
3.  **Evaluation:** Using Confusion Matrices and Categorical Crossentropy Loss to measure performance.
4.  **Visualization:** Generating Grad-CAM heatmaps to validate biological features (e.g., detecting lesions vs. background noise).

## 📝 Technical Report (Turkish)
For a comprehensive technical breakdown and detailed report in Turkish, please refer to the [TECHNICAL_REPORT_TR.md](TECHNICAL_REPORT_TR.md) file included in this repository.

## 🤝 Contribution
This is an open-source project developed for educational and portfolio purposes. Feedback, issues, and pull requests are welcome.

## 📜 License
Distributed under the MIT License. See `LICENSE` for more information.

- **Architecture:** MobileNetV2 (Pre-trained on ImageNet) with custom classification head.
- **Data Engineering:** Robust data splitting (Train/Val/Test) to prevent data leakage.
- **Performance:** Optimized for inference speed (Low Latency) and high accuracy.
- **Reproducibility:** Structured according to strict Data Science standards.

### 📂 Data Setup (Crucial Step)
Since the dataset is large, it is not included in this repository. Please follow these steps to set up the data:

1.  **Download:** Go to [Kaggle PlantVillage Dataset](https://www.kaggle.com/datasets/abdallahalidev/plantvillage-dataset) and download the archive.
2.  **Extract:** Unzip the downloaded file.
3.  **Organize:** Move the extracted `PlantVillage` folder into the `data/raw/` directory of this project.
    * *Correct Path:* `YourProject/data/raw/PlantVillage/`
    * Inside this folder, you should see subfolders like `Tomato___Bacterial_spot`, `Pepper__bell___healthy`, etc.

## 🛠 Installation & Usage

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/YOUR_USERNAME/PlantVillage-DeepLearning-System.git](https://github.com/YOUR_USERNAME/PlantVillage-DeepLearning-System.git)
   cd PlantVillage-DeepLearning-System
