# Machine Learning Classification Analysis

This project explores several machine learning models for a binary classification task using the Breast Cancer Wisconsin dataset from the UCI Machine Learning Repository.

The goal is to compare different algorithms, evaluate their performance, and determine the most suitable model for identifying malignant cases.

---

## Dataset

The dataset contains **699 samples** with cytological features extracted from breast mass images.  
Each instance is classified as:

- **Benign (0)**
- **Malignant (1)**

Features describe characteristics of cell nuclei such as clump thickness, cell size uniformity, and mitoses.

Dataset source:  
UCI Machine Learning Repository – Breast Cancer Wisconsin Dataset.

---

## Project Workflow

The project follows a standard machine learning pipeline:

1. **Exploratory Data Analysis (EDA)**
   - Dataset structure inspection
   - Class distribution analysis
   - Feature distributions
   - Correlation heatmap

2. **Data Preprocessing**
   - Handling missing values
   - Feature scaling
   - Train–test split using stratification

3. **Model Training**
   - Logistic Regression (baseline)
   - k-Nearest Neighbours
   - Support Vector Machine (RBF kernel)
   - Random Forest

4. **Model Evaluation**
   - Accuracy
   - Confusion matrix
   - Classification report
   - ROC AUC

5. **Hyperparameter Exploration**
   - GridSearchCV used to explore SVM parameters.

---

## Model Comparison

The following models were evaluated on the test dataset:

| Model | Accuracy | Recall (Malignant) |
|------|------|------|
| Logistic Regression | ~0.95 | 0.92 |
| k-Nearest Neighbours | ~0.95 | 0.92 |
| Support Vector Machine | ~0.96 | 0.94 |
| Random Forest | **~0.96** | **0.96** |

Random Forest achieved the best overall performance with the highest recall for malignant cases and the fewest false negatives.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## Project Structure
```
ml-classification-analysis/
│
├── notebook/
│ └── classification-analysis.ipynb
│
├── data/
│
├── README.md
└── requirements.txt
```
---

## How to Run

1. Clone the repository
```
git clone https://github.com/EnitaH/ml-classification-analysis.git
```
2. Install dependencies
```
pip install -r requirements.txt
```
3. Open the notebook
4. Run all cells to reproduce the analysis.

---

## Author

**Enita Hashemi**  
BSc (Hons) Computer Science  
Robert Gordon University

---

## License

This project is for educational and portfolio purposes.

