# Iris Flower Species Classification Using KNN

## Project overview
A small multi-class classification project that predicts Iris setosa, Iris versicolor, or Iris virginica from four flower measurements.

## Dataset
Scikit-learn's built-in Iris dataset: 150 observations, 4 features, 3 classes (50 observations per class). No separate CSV download is required.

## Model and workflow
- 80% training data and 20% testing data
- Stratified split with random_state=42
- StandardScaler for feature scaling
- K-Nearest Neighbors classifier with k=5
- Evaluation using accuracy, confusion matrix, precision, recall, and F1-score

## Results from the included run
- Test examples: 30
- Accuracy: 93.33%
- Confusion matrix (rows = actual classes; columns = predicted classes):
```text
[[10  0  0]
 [ 0 10  0]
 [ 0  2  8]]
```

## Run
Install dependencies:
```bash
pip install scikit-learn jupyter
```
Run the Python script:
```bash
python iris_knn.py
```
Or open `iris_knn_case_study.ipynb` in Jupyter or Google Colab and run all cells.

## Files
- `iris_knn.py` — executable Python code
- `iris_knn_case_study.ipynb` — notebook version
- `CLA3_Iris_KNN_Case_Study.docx` — report

## Reproducibility
The split seed, test size, scaling method, and KNN neighbour count are fixed in the code so the reported results can be reproduced in the same Scikit-learn environment.
