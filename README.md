# **Customer Purchase Prediction in E-commerce**

## **Project Overview**
This project aims to predict future customer purchases on an e-commerce platform based on their browsing patterns, purchase history, and customer demographics. We leverage machine learning models, including **Logistic Regression** and **XGBoost Regression**, to predict whether a customer will make a purchase in the future.

The dataset used for this project is the [UCI Online Retail Dataset](https://archive.ics.uci.edu/ml/datasets/Online+Retail), which contains transactional data for an online retailer.

---

## **Table of Contents**

1. [Dataset](#dataset)
2. [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
3. [Modeling](#modeling)
    - Logistic Regression
    - XGBoost Regression
4. [Evaluation](#evaluation)
5. [How to Run](#how-to-run)
6. [Conclusion](#conclusion)

---

## **Dataset**
The dataset used in this project is the **UCI Online Retail Dataset**. It contains transactional data, including:
- **InvoiceNo**: Invoice number
- **StockCode**: Product code
- **Description**: Product description
- **Quantity**: Quantity of each product per transaction
- **InvoiceDate**: Transaction date and time
- **UnitPrice**: Product price per unit
- **CustomerID**: Unique customer identifier
- **Country**: Country of the customer

Dataset Source: [UCI Machine Learning Repository - Online Retail Dataset](https://archive.ics.uci.edu/ml/datasets/Online+Retail)

---

## **Exploratory Data Analysis (EDA)**

In the EDA, we analyzed the following:
1. **Data Cleaning**: Handled missing values and removed canceled orders (negative quantities).
2. **Time-based Trends**: Extracted and visualized trends in transactions across different months, days, and hours.
3. **Country-wise Transactions**: Visualized the top 10 countries based on transaction count.
4. **Top Purchased Products**: Identified the most popular products.
5. **Recency, Frequency, and Monetary (RFM) Analysis**: Analyzed customer behavior using RFM metrics to understand purchase patterns.
6. **Correlation Analysis**: Visualized the relationships between RFM features.

---

## **Modeling**

We built two models for predicting future customer purchases:
1. **Logistic Regression**: A basic classification algorithm that models the probability of a customer making a future purchase.
2. **XGBoost Regression**: A more advanced and powerful gradient boosting model that improves prediction accuracy by iteratively optimizing errors.

---

## **Evaluation**

The performance of both models was evaluated using the following metrics:
- **Accuracy**: Measures the overall correctness of the model.
- **Precision**: Measures the model's ability to correctly predict positive instances.
- **Recall**: Measures how many actual positive instances were correctly predicted.
- **F1-Score**: A harmonic mean of precision and recall.

We compare the results from **Logistic Regression** and **XGBoost Regression** to determine which model performs better for our prediction task.

---

## **How to Run**

### **Requirements**
- Python 3.x
- Libraries: 
  - pandas
  - numpy
  - matplotlib
  - seaborn
  - scikit-learn
  - xgboost

### **Steps to Run**
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/customer-purchase-prediction.git
   cd customer-purchase-prediction
   ```

2. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

3. Download the dataset from the [UCI repository](https://archive.ics.uci.edu/ml/datasets/Online+Retail), and place it in the root directory of the project.

4. Run the EDA and modeling scripts:
   ```bash
   python eda.py
   python model.py
   ```

5. Provide input to compare predictions from both models (Logistic Regression and XGBoost):
   ```bash
   python input_prediction.py
   ```

---

## **Conclusion**
This project demonstrates how customer browsing and transaction data can be leveraged to predict future purchases using machine learning models. We use both a basic **Logistic Regression** model and a more advanced **XGBoost** model to evaluate which provides better predictions for customer behavior.

---

## **License**
This project is licensed under the MIT License.

---

Feel free to modify the project and experiment with other machine learning algorithms, feature engineering techniques, or additional datasets to enhance the predictive power!

---

### **Contact**

For any queries or contributions, feel free to reach out via GitHub Issues or directly through email.

