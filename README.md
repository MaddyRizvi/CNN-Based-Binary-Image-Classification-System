
# Binary Image Classification with Convolutional Neural Networks (CNN)

## 📌 Summary

This project implements a Convolutional Neural Network (CNN) for binary image classification using a dataset of **10,000** animal images (dogs vs. cats). The goal is to train a deep learning model that can accurately classify images into one of two categories using supervised learning techniques in computer vision. This model can be trained on any other big size dataset.

---

## Model Performance
   Given below is how model performed
- **Training Accuracy:** 89.7%
- **Validation Accuracy:** 79.1%

## 📁 Dataset

- The dataset used consists of labeled images of **dogs** and **cats**.
- Each image is resized to a fixed shape for input consistency (e.g., 128x128).
- Data is split into **training**, **validation**, and **testing** sets.
- Dataset source: [Kaggle Dogs vs. Cats Dataset](https://www.kaggle.com/c/dogs-vs-cats/data) or a custom binary image dataset.

---

## 📂 Project Structure

```
├── data/
│   ├── train/
│   ├── test/
│   └── val/
├── models/
│   └── cnn_model.h5
├── notebooks/
│   └── convolutional_neural_network.ipynb
├── utils/
│   └── image_preprocessing.py
├── README.md
├── requirements.txt
└── run.py
```

---

## ⚙️ Requirements

To run this project, install the following dependencies (via `requirements.txt`):

```
tensorflow
keras
numpy
pandas
matplotlib
opencv-python
scikit-learn
```

Install them using:

```bash
pip install -r requirements.txt
```

---

## ▶️ How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/MaddyRizvi/CNN-Based-Binary-Image-Classification-System
   cd CNN-Based-Binary-Image-Classification-System
   ```

2. Prepare your dataset:
   - Place your images in `data/train/` and `data/test/` directories with subfolders `/dog` and `/cat`.

3. Run the training notebook:
   ```bash
   jupyter notebook notebooks/convolutional_neural_network.ipynb
   ```

4. Or run the script:
   ```bash
   python run.py
   ```

---

## 📈 Output

- Trained CNN model saved as `models/cnn_model.h5`.
- Training and validation accuracy/loss plots.
- Classification report and confusion matrix on test data.
- Example predictions with labeled images.

---

## 🔍 Details

**Algorithm Used:** Convolutional Neural Network (CNN)  
**Model Layers:** Conv2D → MaxPooling → Conv2D → MaxPooling → Flatten → Dense  
**Activation Functions:** ReLU (hidden layers), Sigmoid (output)  
**Loss Function:** Binary Cross-Entropy  
**Optimizer:** Adam  
**Distance Metric:** N/A (since this is a classification problem, not clustering)  
**Evaluation Metrics:** Accuracy, Precision, Recall, F1-Score

---

## 🧠 Understanding

The CNN learns to extract features like edges, textures, and shapes through convolutional layers, which are then used by dense layers to classify images. This project demonstrates how deep learning can be used for simple vision tasks like binary image classification and can be extended to more complex datasets or multi-class problems.

---

## 🤝 Contributing

Feel free to fork this repository and submit a pull request if you want to:
- Improve model architecture
- Add image augmentation or regularization
- Convert to multi-class classification
- Integrate with a web app for live demo

---

## 📜 License

This project is licensed under the MIT License – see the [LICENSE](LICENSE) file for details.

---
