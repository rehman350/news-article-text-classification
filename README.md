# News Article Classification using Machine Learning

## Project Overview
This project performs text **classification on news articles** and classifies them into two categories using Machine Learning. It involves:

- Exploratory Data Analysis (EDA)
- Text Preprocessing
- Feature Extraction (TF–IDF)
- Model Training (SVM Classifier)
- Evaluation & Results

This project was created as a Machine Learning assignment.

## Columns:
| Column | Description |
|--------|-------------|
| text   | News article text |
| label  | Class label (2 or 3) |

After preprocessing, a cleaned dataset is saved as:

Data/clean_data.csv

## Step-1: Exploratory Data Analysis (EDA)
`01_eda.ipynb`

### Performed Tasks
✔ Loaded dataset  
✔ Checked structure and summary  
✔ Calculated word count  
✔ Plotted:

- Word Count Distribution
- Word Count by Label

### Observation:

> Most articles contained 25–45 words before preprocessing.

## Step-2: Text Preprocessing
Notebook:  
`02_preprocessing.ipynb`

### Applied Techniques
✔ Lower-casing  
✔ Removing punctuation  
✔ Removing stopwords  
✔ Lemmatization  

A new cleaned column was created: clean_text

## Step-3: Feature Extraction  
`03_feature_extraction.ipynb`

Technique Used:

TF–IDF Vectorization

Data split:
80% Training
20% Testing

## 🤖 Model Used
Classifier:
Support Vector Machine (SVM)

## Model Performance

| Metric | Score |
|--------|------|
| Accuracy | **0.85 (85%)** |

### Classification Report

| Label | Precision | Recall | F1-Score |
|------|----------|-------|--------|
| 2 | 0.84 | 1.00 | 0.91 |
| 3 | 1.00 | 0.25 | 0.40 |

### Confusion Matrix

[[16 0]
[ 3 1]]

Interpretation

- Class-2 predicted very well
- Class-3 recall low because dataset is small & imbalanced


## Conclusion

Text preprocessing improved data quality and reduced noise.  
TF-IDF successfully converted text into numeric features.  
SVM achieved **85% accuracy**.

## Future Improvements
✔ Collect more data  
✔ Balance dataset  
✔ Try deep learning  
✔ Hyperparameter tuning  

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- NLTK
- Scikit-Learn

## Author
Abdul Rehman  
Machine Learning Student
