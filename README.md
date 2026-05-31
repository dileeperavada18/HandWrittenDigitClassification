

```markdown
# Handwritten Digit Classification using TensorFlow & MNIST

A simple yet highly efficient deep learning project that classifies handwritten digits (0-9) using the classic **MNIST dataset**. Built with **TensorFlow and Keras**, this project preprocesses pixel data and trains a Sequential Neural Network to recognize numerical digits with high accuracy.

---

## 🚀 Features
* **Built-in Dataset Loading:** Automatically fetches and loads the 60,000 training images and 10,000 testing images from the MNIST dataset.
* **Data Normalization:** Scales the pixel intensity values to a range between 0 and 1 using Keras utilities to speed up training convergence.
* **Sequential Deep Architecture:** Features a Multi-Layer Perceptron (MLP) built with Flattening, Dense layers, ReLU activation functions, and Softmax classification.
* **Visual Verification:** Includes custom plotting functions to visually display the digits along with their respective model predictions.

---

## 🛠️ Tech Stack & Libraries
* **Framework:** TensorFlow / Keras
* **Numerical Processing:** NumPy
* **Data Visualization:** Matplotlib

---

## 📋 Dataset
The **MNIST dataset** consists of $28 \times 28$ grayscale images of handwritten digits:
* **Training Set:** 60,000 images
* **Testing Set:** 10,000 images
* **Labels:** 0 through 9

---

## 💻 Installation & Usage

### 1. Clone the Repository
```bash
git clone [https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git](https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git)
cd YOUR_REPOSITORY_NAME

```

### 2. Install Dependencies

Make sure Python is installed, then run the following command to install the required libraries:

```bash
pip install tensorflow numpy matplotlib

```

### 3. Running the Project

Execute the script via your terminal:

```bash
python handwrittendigitclassification.py

```

*Note: If you are running this on **Google Colab**, you can simply copy-paste the cells or upload the `.py`/`.ipynb` file directly without needing manual installations.*

---

## 🧠 Model Architecture

The neural network utilizes a direct feedforward `Sequential` pipeline:

1. **Flatten Layer:** Reshapes the input data from a 2D matrix ($28 \times 28$ pixels) into a 1D array of 784 pixels.
2. **Hidden Layer 1:** Dense fully-connected layer with **128 neurons** using the **ReLU** activation function.
3. **Hidden Layer 2:** Dense fully-connected layer with **128 neurons** using the **ReLU** activation function.
4. **Output Layer:** Dense layer with **10 neurons** (one for each digit from 0 to 9) using the **Softmax** activation function to output class probabilities.

### Training Configuration:

* **Optimizer:** Adam
* **Loss Function:** Sparse Categorical Crossentropy
* **Metrics:** Accuracy
* **Epochs:** 3

---

## 📊 Results

Upon training, the script evaluates the model against the unseen test dataset and outputs:

* **Validation Loss**
* **Validation Accuracy**
* A sample prediction comparison alongside a rendered visualization of the test image.

```

```
