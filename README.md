# Task5-Decision Trees and Random Forests
# Heart Disease Prediction with Decision Trees and Random Forests

This project was completed as part of the AI & ML Internship Task 5. The goal is to build and evaluate machine learning models, specifically Decision Trees and Random Forests, to predict heart disease using a preprocessed dataset.

---

## Objective
Learn how to:
- Implement Decision Tree and Random Forest classifiers
- Visualize decision trees
- Evaluate model performance using accuracy, classification reports, and cross-validation
- Preprocess data for machine learning models

---

## Dataset
I used the [Heart Disease Dataset](https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset).

---

## Tools & Libraries
- **Python**: Programming language
- **Pandas**: Data manipulation
- **NumPy**: Numerical operations
- **Matplotlib**: Data visualization
- **Scikit-learn**: Machine learning models, preprocessing, and evaluation
- **Graphviz**: Decision tree visualization

---

## Project Structure
The project is implemented in a Google Colab Notebook (`Task_5_Decision_Trees_and_Random_Forests.ipynb`). Below are the key steps performed:

### 1. Data Loading
- Loaded the heart disease dataset using `pandas`.
- Displayed basic information (`df.info()`) and the first few rows (`df.head()`) to understand the dataset structure.

### 2. Data Preprocessing
- **Separated Features and Target**: Extracted features (`X`) and target (`y`) variables, with `target` indicating heart disease presence.
- **Train-Test Split**: Split the data into training (70%) and testing (30%) sets using `train_test_split` with a random state of 42 for reproducibility.
- **Feature Scaling**: Standardized numerical features using `StandardScaler` to ensure consistent scales across features.

### 3. Decision Tree Classifier
- Trained a `DecisionTreeClassifier` with a random state of 42.
- Evaluated performance using accuracy score and classification report.
- Visualized the decision tree using `graphviz` and `sklearn.tree.plot_tree`, saving the output as `decision_tree.pdf`.

### 4. Random Forest Classifier
- Trained a `RandomForestClassifier` (code not shown in the provided snippet but referenced in cross-validation).
- Evaluated performance using accuracy and classification metrics.

### 5. Cross-Validation
- Performed 5-fold cross-validation on both models:
  - **Decision Tree**: Achieved an accuracy of 1.0000 (±0.0000).
  - **Random Forest**: Achieved an accuracy of 0.9971 (±0.0059).

---

## Results
- **Decision Tree**:
  - Test Accuracy: 0.9708
  - Classification Report: High precision, recall, and F1-scores for both classes (0: No Disease, 1: Disease).
  - Cross-Validation Accuracy: 1.0000 (±0.0000)
- **Random Forest**:
  - Cross-Validation Accuracy: 0.9971 (±0.0059)
- The Decision Tree achieved perfect cross-validation accuracy, while the Random Forest showed slightly lower but robust performance.
