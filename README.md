# 🌿 Cotton Leaf Curl Virus Detection Using Deep Learning

### AI-Powered Cotton Disease Detection for Smart Agriculture

An Artificial Intelligence and Deep Learning based project designed to identify **Cotton Leaf Curl Virus (CLCuV)** from cotton leaf images. The proposed system aims to help identify potential disease symptoms through image classification and provide general disease-prevention guidance.

The project focuses on two classes:
- 🌱 **Healthy Cotton Leaf**
- 🦠 **Cotton Leaf Curl Virus (CLCuV)**

The planned solution combines deep learning with an Android mobile application to make image-based disease screening accessible and convenient.

---

## 📌 Table of Contents

- [Project Overview](#-project-overview)
- [Objectives](#-objectives)
- [Key Features](#-key-features)
- [How It Works](#-how-it-works)
- [Technologies Used](#-technologies-used)
- [Dataset](#-dataset)
- [Model Development](#-model-development)
- [Project Structure](#-project-structure)
- [Installation](#-installation)
- [Expected Results](#-expected-results)
- [Future Improvements](#-future-improvements)
- [Disclaimer](#-disclaimer)
- [Author](#-author)

---

## 🌱 Project Overview

Cotton is an important agricultural crop in Pakistan. Cotton Leaf Curl Virus is a significant disease that can affect cotton plants and reduce crop productivity.

This project proposes a deep learning-based approach to classify cotton leaf images as healthy or potentially affected by Cotton Leaf Curl Virus.

Users will be able to capture a cotton leaf image using a mobile camera or select an image from their gallery. The trained model will analyze the image and display a predicted class.

The long-term goal is to develop a user-friendly Android application that supports preliminary disease screening and provides general information about disease prevention.

## 🎯 Objectives

- Develop an image-classification model for Cotton Leaf Curl Virus screening.
- Distinguish healthy cotton leaves from leaves showing CLCuV-related symptoms.
- Explore EfficientNetB0 transfer learning for image classification.
- Integrate the trained model into an Android application.
- Provide general disease-awareness and prevention information.
- Evaluate model performance using standard machine-learning metrics.
- Explore how AI can support agricultural decision-making.

## ✨ Key Features

- 📷 **Camera Support:** Capture cotton leaf images using a mobile device.
- 🖼️ **Image Upload:** Select leaf images from the device gallery.
- 🧠 **AI-Based Classification:** Predict whether an image belongs to the healthy or CLCuV class.
- 📊 **Model Evaluation:** Measure performance using accuracy, precision, recall, and F1-score.
- 🌾 **Disease Awareness:** Display general information about Cotton Leaf Curl Virus.
- 📱 **Android Application:** Provide a simple and accessible mobile interface.
- 🔬 **Transfer Learning:** Explore EfficientNetB0 to build the image-classification model.

*These are planned features; their implementation and performance will be documented as development progresses.*

## ⚙️ How It Works

1. **Image Input:** The user captures or uploads a cotton leaf image.
2. **Preprocessing:** The image is resized and prepared for the trained model.
3. **Model Inference:** The deep learning model analyzes image features.
4. **Prediction:** The application displays the predicted class.
5. **Guidance:** The user receives general disease-awareness or prevention information.

```text
Cotton Leaf Image
        |
        v
Image Preprocessing
        |
        v
Deep Learning Model
   (EfficientNetB0)
        |
        v
  Classification
    /         \
   v           v
Healthy      Possible CLCuV
   \           /
    v         v
 Prediction and General Guidance
```

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Python | Model development |
| TensorFlow / Keras | Deep learning |
| EfficientNetB0 | Proposed image-classification architecture |
| OpenCV | Image processing |
| Scikit-learn | Model evaluation |
| Matplotlib | Visualizing training and evaluation results |
| Kotlin | Android application development |
| Android Studio | Mobile app development environment |
| FastAPI | Optional model-serving backend |
| Git & GitHub | Version control and project hosting |

## 📂 Dataset

The project requires a labelled cotton leaf image dataset containing these two classes:

1. Healthy Cotton Leaf
2. Cotton Leaf Curl Virus (CLCuV)

Before training, the dataset will be checked for:
- Correct image labels
- Image quality and readability
- Class distribution
- Duplicate or near-duplicate images
- Appropriate usage permissions and licensing

**Dataset note:** Add the verified dataset source and its licence here after checking the downloaded files. The dataset images are not included in this repository.

## 🧠 Model Development

The proposed model is **EfficientNetB0 with Transfer Learning**.

The development process will include:

1. Loading and inspecting the dataset.
2. Preprocessing and resizing images.
3. Splitting data into training, validation, and test sets.
4. Applying appropriate data augmentation to training images.
5. Training and tuning the model.
6. Evaluating performance on a held-out test set.
7. Exporting the trained model for application integration.

### Evaluation Metrics

The model will be evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion matrix

Actual scores will be added after training and testing. No model accuracy is claimed at this stage.

## 📁 Project Structure

```text
Cotton-Leaf-Curl-Virus-Detection/
│
├── README.md
├── requirements.txt
├── .gitignore
│
├── proposal/
│   ├── Cotton_Leaf_Curl_Virus_FYP_Proposal.pdf
│   └── Cotton_Leaf_Curl_Virus_FYP_Proposal.docx
│
├── dataset/
│   └── README.md
│
├── model/
│   └── README.md
│
├── android-app/
│   └── README.md
│
└── notebooks/
    └── README.md
```

*This structure represents the current starter repository. Training notebooks, model files, and Android source code can be added as they are developed.*

## 💻 Installation

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR-USERNAME/Cotton-Leaf-Curl-Virus-Detection.git
```

Replace `YOUR-USERNAME` with your GitHub username.

### 2. Open the Project Folder

```bash
cd Cotton-Leaf-Curl-Virus-Detection
```

### 3. Create a Virtual Environment

```bash
python -m venv .venv
```

Activate it on Windows:

```bash
.venv\Scripts\activate
```

### 4. Install Dependencies

```bash
pip install -r requirements.txt
```

**Note:** These steps prepare the Python environment. The complete training pipeline and Android application must be implemented before the full system can run.

## 📈 Expected Results

The expected outcome is a prototype capable of classifying cotton leaf images into healthy and possible Cotton Leaf Curl Virus categories.

The final report will document:
- Dataset details and class distribution
- Training configuration
- Measured evaluation metrics
- Confusion matrix
- Limitations and possible sources of error

Results will be reported only after the model has been trained and evaluated.

## 🚀 Future Improvements

- Improve performance using a larger, verified dataset.
- Convert the trained model to TensorFlow Lite for on-device inference.
- Complete Android application integration.
- Add offline prediction support if the selected model deployment approach allows it.
- Improve usability with multilingual guidance.
- Validate predictions using images collected under real field conditions.
- Collaborate with agricultural experts to review disease-management information.

## ⚠️ Disclaimer

This project is intended for educational and research purposes. Image-based predictions are preliminary and should not be treated as a definitive plant diagnosis. Similar symptoms may have different causes, and model performance depends on the quality and diversity of the training data.

Consult a qualified agricultural expert or local agricultural extension service before making disease-management or treatment decisions.

## 👨‍💻 Author

**Shakir Hussain**

Final Year Project: Cotton Leaf Curl Virus Detection Using Deep Learning


⭐ If you find this project interesting, consider starring the repository as it develops.
