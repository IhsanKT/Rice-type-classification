# 🌾 Rice Type Classification using PyTorch

This project implements a binary classification model to distinguish between two types of rice grains using a fully connected neural network built with PyTorch. The dataset is sourced from Kaggle and includes features such as Area, Perimeter, Roundness, and others.

---

## 📂 Dataset

- **Source**: [Kaggle - Rice Type Classification](https://www.kaggle.com/datasets/mssmartypants/rice-type-classification)
- **Attributes**: 11 features per rice grain sample
- **Classes**:  
  - `0` - One type of rice  
  - `1` - Another type of rice

---

## 🔧 Setup Instructions

1. **Clone the repo and open in Colab**  
   Or upload your `.ipynb` file to Colab directly.

2. **Install Dependencies**
   ```bash
   !pip install opendatasets --quiet
   ```

3. **Download Dataset**
   - You'll need a Kaggle API key.
   - Upload your `kaggle.json` or enter credentials when prompted.

4. **Run All Cells**
   - Data will be downloaded and preprocessed.
   - A model will be trained and evaluated.

---

## 🧠 Model Architecture

- **Input Layer**: 10 features
- **Hidden Layer**: 10 neurons (ReLU)
- **Output Layer**: 1 neuron (Sigmoid for binary classification)
- **Loss Function**: Binary Cross Entropy (BCELoss)
- **Optimizer**: Adam (learning rate: 0.001)

---

## 📊 Results

- **Training Accuracy**: ~98.6%
- **Validation Accuracy**: ~98.5%
- **Test Accuracy**: ~98.5%

---

## 🧪 Inference

You can run predictions by entering the feature values in the final cell:

```
Area: 4537
Major Axis Length: 92
Minor Axis Length: 64
Eccentricity: 0.71
...
```

Output:
```
Class is: 0
```

---

## 📁 File Structure

```
rice-type-classification/
│
├── rice_classification.ipynb  # Notebook with full pipeline
├── README.md                  # This file
```

---

## ✅ To Do

- [ ] Add feature importance visualization
- [ ] Experiment with more complex architectures
- [ ] Convert model to ONNX or TorchScript for deployment
- [ ] Streamlit or Gradio web app interface

---

## 🙋‍♂️ Author

**Ihsan KT**  
For questions, feel free to open an issue or reach out!
