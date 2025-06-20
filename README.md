# Face-Recognition-using-KNN
# 🧑‍🏫 Face Recognition using K-NN, SVM, and GaussianNB

This project implements a face recognition system using a simplified CMU PIE dataset. It includes a custom-built **K-Nearest Neighbors (K-NN)** classifier, alongside **SVM** and **Gaussian Naive Bayes** classifiers using `scikit-learn`.

---


## ✅ Project Tasks

### Task 1: Preprocessing
- Normalized each face vector to unit length
- Used:
  - **150 training + 20 test samples** per subject (main setup)
  - **100 training + 70 test samples** per subject (alternate setup)

---

### Task 2: Custom K-NN Implementation
- Implemented **K-NN from scratch** (no libraries)
- Distance Metrics:
  - Euclidean Distance ✅
  - Cosine Similarity ❌ (performed poorly on this dataset)
- Evaluated with K values: **2, 5, 7, 11**

---

### Task 3: SVM and Naive Bayes

| Classifier       | Accuracy |
|------------------|----------|
| **SVM (Linear)** | **100%** |
| GaussianNB       | 85.0%    |

---

### Task 4: PCA Visualization

Applied **Principal Component Analysis (PCA)** to reduce data to 3D for visualization of class separability.

> Visualization was done using Matplotlib’s `Axes3D` scatter plot and color-coded by subject ID.

---

## 🚀 How to Run

### 1. Install dependencies

```bash
pip install numpy pandas scikit-learn matplotlib
2. Prepare dataset
Place dataset.csv in the root directory.

3. Run the main script

python main.py
This will:

Train and evaluate K-NN with multiple configurations

Compare with SVM and Naive Bayes

Generate a PCA 3D scatter plot

📂 Project Structure

📦face-recognition-knn
 ┣ 📜 main.py               # Main implementation script
 ┣ 📜 dataset.csv           # Input face dataset (CSV format)
 ┣ 📜 README.md             # Project documentation
