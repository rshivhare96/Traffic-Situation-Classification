# 🚦 Traffic Situation Classification

This project analyzes traffic data collected over time, focusing on vehicle counts and categorizing the **traffic situation** (e.g., low, normal, high, jam). The goal is to develop a classification model that accurately predicts the traffic situation using vehicle and time-related features.

---

## 📂 Data

The dataset used is:

- `Traffic.csv`

It contains the following features:

- **Time**: Time of the day  
- **Date**: Day number of the month  
- **Day of the week**: Weekday name  
- **CarCount**, **BikeCount**, **BusCount**, **TruckCount**: Counts of different vehicle types  
- **Total**: Sum of all vehicle counts  
- **Traffic Situation**: Target label (low, normal, high, jam)

---

## 🔍 Analysis Workflow

The project includes the following steps:

- Initial data loading and inspection  
- Missing values and duplicate check  
- Exploratory Data Analysis (EDA) using **Seaborn** and **Matplotlib**  
- Label encoding of categorical features  
- Feature-target split and train-test split  
- Model training using multiple regression and classification models  
- Model performance evaluation using accuracy, precision, recall, and F1-score  
- Hyperparameter tuning of **SVM** using **GridSearchCV**

---

## 📊 Key Insights

- No missing or duplicate data entries  
- Clear trends in traffic based on **day of the week**, **vehicle count**, and **date**  
- Vehicle types like **CarCount** and **TruckCount** strongly influence traffic levels  
- The SVM model with `rbf` kernel and `C=100` showed the best performance with **95.4% accuracy**

---

## 📁 Scripts & Outputs

- `traffic_classification.ipynb`: Full analysis pipeline from loading to model evaluation  
- Visualization outputs include:
  - Count plots of traffic situation per weekday
  - Histogram distributions of vehicle types segmented by traffic situation

---

## 🛠️ Libraries Used

- **Data Processing**: `pandas`, `numpy`  
- **Visualization**: `matplotlib`, `seaborn`  
- **Modeling**: `sklearn`, `xgboost`, `yellowbrick`  
- **Evaluation**: `classification_report`, `accuracy_score`, `GridSearchCV`

---

## ✅ Usage

To run the project:

1. Clone this repository  
2. Place `Traffic.csv` in the root directory  
3. Run the Jupyter notebook `traffic_classification.ipynb`  
4. Review the model outputs and plots for insights

---

## 🚀 Future Improvements

- Incorporate **time features** more effectively (e.g., convert `Time` to hour bins)  
- Balance class distributions if imbalanced  
- Deploy the best model as a web API or visualization dashboard  
- Use time series or deep learning for sequential prediction

---

## 👤 Author

**Rohit Shivhare**  
[LinkedIn](https://www.linkedin.com/in/rohit-shivhare-a857a4233/)  
*MSc Data Science – Brunel University, London*
