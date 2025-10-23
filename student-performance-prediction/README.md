
# Student Performance Prediction

This project analyzes and predicts students’ **math scores** based on demographic and academic factors using **Machine Learning (Linear Regression)**.  
It demonstrates end-to-end data science workflow — from data cleaning and visualization to model training and evaluation.

---

##  Project Structure
```
student-performance-prediction/
│
├── data/
│   └── StudentsPerformance.csv
│
├── notebook/
│   └── analysis.ipynb
│
├── main.py
├── requirements.txt
└── README.md
```

---

##  Dataset
- **Source:** [Kaggle - Students Performance in Exams](https://www.kaggle.com/datasets/spscientist/students-performance-in-exams)
- **Description:**  
  Includes students’ gender, parental education, lunch type, test preparation course, and scores in math, reading, and writing.

---

##  Tools & Libraries
- **Python**
- **Pandas, NumPy**
- **Matplotlib, Seaborn**
- **Scikit-learn**

---

##  Steps Followed

### 1. Data Loading & Cleaning
Loaded dataset using Pandas, checked for missing values, and formatted column names.

### ️2. Exploratory Data Analysis (EDA)
Visualized distributions, correlations, and boxplots to identify patterns (e.g., impact of test preparation course on performance).

### 3. Feature Encoding
Converted categorical features (`gender`, `lunch`, `race/ethnicity`, etc.) into numerical values using LabelEncoder.

### 4. Model Training
Trained a **Linear Regression model** to predict math scores based on other academic and demographic factors.

### 5. Evaluation
Evaluated using **Mean Absolute Error (MAE)** and **R-squared (R²)** metrics.

**Example Results:**
```
Mean Absolute Error: 3.8
R-squared: 0.82
```

## Prediction Example
Predicted math score for a new student with given reading & writing scores.

```python
new_data = pd.DataFrame({
    'reading_score': [72],
    'writing_score': [78]
})
predicted_score = model.predict(new_data)
print(f"Predicted Math Score: {predicted_score[0]:.2f}")
```

---

## Key Insights
- Students who **completed test preparation courses** performed better in math.
- **Lunch type** and **parental education** showed moderate influence.
- **Gender differences** were minor in this dataset.

---

## Future Work
- Try other models (Random Forest, XGBoost)
- Build a web interface using **Streamlit**
- Include feature importance visualization

---

## How to Run
1. Clone the repo  
   ```bash
   git clone https://github.com/yourusername/student-performance-prediction.git
   cd student-performance-prediction
   ```
2. Install dependencies  
   ```bash
   pip install -r requirements.txt
   ```
3. Run the notebook or script  
   ```bash
   python main.py
   ```

---

## Author
**Thiri Swe Zin**  
💻 Software Engineering Student | Aspiring Data Scientist  
📫 [thiriszin129@gmail.com]  
🌐 [https://github.com/Thiri-SweZin](https://github.com/Thiri-SweZin)
````

