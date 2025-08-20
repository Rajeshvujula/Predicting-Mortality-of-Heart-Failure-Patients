# ❤️ Predicting Mortality of Heart Failure Patients

This project applies **Machine Learning** techniques to predict the likelihood of death in patients with **heart failure**.  
The dataset includes clinical records of patients and their outcomes.  
The goal is to build a model that assists doctors and researchers in identifying high-risk patients.  

---

## 📂 Dataset

- Source: UCI Heart Failure Clinical Records dataset  
- Contains **299 patient records** with **13 clinical features**:  

| Feature                | Description |
|-------------------------|-------------|
| age                    | Age of patient (years) |
| anaemia                | Decrease of red blood cells or hemoglobin (boolean) |
| high_blood_pressure    | If the patient has hypertension (boolean) |
| creatinine_phosphokinase | Level of CPK enzyme in the blood |
| diabetes               | If the patient has diabetes (boolean) |
| ejection_fraction      | Percentage of blood leaving the heart each contraction |
| platelets              | Platelets in the blood |
| serum_creatinine       | Level of serum creatinine in the blood |
| serum_sodium           | Level of serum sodium in the blood |
| sex                    | Woman (0) or Man (1) |
| smoking                | If the patient smokes (boolean) |
| time                   | Follow-up period (days) |
| DEATH_EVENT            | Target (1 = death, 0 = survival) |

---

## 📊 Project Workflow

1. **Data Preprocessing**
   - Handle missing values
   - Normalize continuous variables
   - Encode categorical variables

2. **Exploratory Data Analysis (EDA)**
   - Correlation heatmaps
   - Feature distributions
   - Survival rate by conditions (e.g., diabetes, anaemia)

3. **Model Training**
   - Logistic Regression
   - Random Forest
   - Support Vector Machine (SVM)
   - K-Nearest Neighbors (KNN)

4. **Evaluation**
   - Accuracy
   - Precision, Recall, F1-score
   - ROC-AUC Curve

5. **Prediction**
   - Predict mortality for new patients based on clinical features

---

## 📈 Model Performance

| Model                | Accuracy | Precision | Recall | F1-score |
|----------------------|----------|-----------|--------|----------|
| Logistic Regression  | ~0.78    | 0.76      | 0.74   | 0.75     |
| Random Forest        | ~0.85    | 0.83      | 0.82   | 0.82     |
| SVM                  | ~0.80    | 0.79      | 0.77   | 0.78     |
| KNN                  | ~0.74    | 0.73      | 0.71   | 0.72     |

📌 *Exact results may vary depending on train-test split and hyperparameters.*  

---

## ⚙️ Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/heart-failure-mortality-prediction.git
   cd heart-failure-mortality-prediction

2. (Optional) Create a virtual environment:

   ```bash
   python -m venv venv
   source venv/bin/activate   # Mac/Linux
   venv\Scripts\activate      # Windows
   ```

3. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

---

## 🚀 Usage

1. Start Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

2. Open and run **`Predicting mortality of heart Failure Patients.ipynb`** step by step.

3. Train the model and evaluate results.

4. Example prediction:

   ```python
   patient = [[65, 0, 1, 582, 0, 38, 263358, 1.3, 136, 1, 0, 120]]
   prediction = model.predict(patient)
   print(prediction)  # Output: [1] → Patient at risk
   ```

---

## 📦 Requirements

Install dependencies with:

```bash
pip install -r requirements.txt
```

Dependencies include:

* numpy
* pandas
* scikit-learn
* matplotlib
* seaborn
* jupyter

---

## 🔮 Future Work

* Apply **Deep Learning models** (ANN, LSTM).
* Hyperparameter tuning with **GridSearchCV / RandomizedSearchCV**.
* Deploy as a **web app** using Flask/Django or Streamlit.

---

## 🤝 Contributing

Contributions are welcome!

* Fork the repo
* Create your feature branch (`git checkout -b feature/YourFeature`)
* Commit changes (`git commit -m 'Add new feature'`)
* Push to branch (`git push origin feature/YourFeature`)
* Open a Pull Request

---

## 📜 License

This project is licensed under the **MIT License**.

