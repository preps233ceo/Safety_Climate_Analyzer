
# Business Analytics Model: Safety Observation Classification

This project applies business analytics and machine learning techniques to classify safety observations as **Safe** or **Unsafe** using a cleaned and balanced dataset.

## 🔍 Objective
Automatically classify text-based safety reports to support proactive risk management and enhance decision-making.

---

## 📊 Dataset
- Source: `cleaned_and_balanced.xlsx`
- 622 entries equally distributed between 'Safe' and 'Unsafe'
- Text-based observations + classification label

---

## 🧠 Model Development Steps

### 1. Problem Definition
Classify observations to streamline analysis of safety performance.

### 2. Import Libraries
Used `pandas`, `matplotlib`, `seaborn`, `scikit-learn`, and `re`.

### 3. Load and Explore Data
Explored structure, distribution of labels, and data quality.

### 4. Text Preprocessing
- Lowercase
- Remove punctuation
- Store in a new column: `Cleaned_Observation`

### 5. Train-Test Split
Used 80% for training and 20% for testing.

### 6. TF-IDF Vectorization
Converted text to numerical features using `TfidfVectorizer(stop_words='english')`.

### 7. Model Training
Evaluated multiple classifiers:
- Naive Bayes (88.8%)
- Linear SVM (89.6%)
- **Logistic Regression (90.4%)**
- **Random Forest (90.4%)**

### 8. Evaluation
Used:
- Accuracy
- Precision, Recall, F1-Score
- Confusion Matrix

### 9. Final Model
Selected **Logistic Regression** due to its top accuracy and balanced performance.

---

## 📁 Files
- `model_logistic_regression.ipynb` - Final model notebook
- `Model_Development_Plan.pptx` - Presentation
- `cleaned_and_balanced.xlsx` - Dataset
- `README.md` - This file

---

## 🚀 Optional Extensions
- Add hyperparameter tuning
- Deploy with Flask or Streamlit
- Serialize model with `joblib` or `pickle`

---

## 📬 Contact
For any inquiries or suggestions, please contact **John Shiburah** johnshiburah@gmail.com.
