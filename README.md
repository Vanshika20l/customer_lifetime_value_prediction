# customer_lifetime_value_prediction

# Customer Segmentation and LTV Prediction

## Overview
This project focuses on customer segmentation and predicting Customer Lifetime Value (LTV) using historical transaction data. The analysis is performed using Python, leveraging libraries such as Pandas, NumPy, Scikit-learn, XGBoost, Matplotlib, and Seaborn.

## Project Structure
- **customer_segment.ipynb**: Jupyter Notebook containing the complete analysis, including data loading, preprocessing, feature engineering, model training, evaluation, and visualization.
- **customer_segmentation.csv**: The dataset used for analysis, containing transaction records.

## Dataset Description
The dataset consists of transaction records with the following columns:
- **InvoiceNo**: Unique identifier for each transaction.
- **StockCode**: Unique identifier for each product.
- **Description**: Description of the product.
- **Quantity**: Number of items purchased.
- **InvoiceDate**: Date and time of the transaction.
- **UnitPrice**: Price per unit of the product.
- **CustomerID**: Unique identifier for each customer.
- **Country**: Country of the customer.

## Key Steps in the Analysis
1. **Data Loading**: The dataset is loaded using Pandas.
2. **Data Preprocessing**:
   - Handling missing values.
   - Cleaning column names.
   - Converting date columns to datetime format.
3. **Feature Engineering**:
   - Calculating Recency, Frequency, and Average Order Value (AOV) for each customer.
   - Simulating Customer LTV based on frequency and AOV.
4. **Model Training**:
   - Splitting the data into training and testing sets.
   - Training a Random Forest Regressor and an XGBoost Regressor to predict Customer LTV.
5. **Model Evaluation**: Evaluating model performance using Mean Absolute Error (MAE) and Root Mean Squared Error (RMSE).
6. **Customer Segmentation**: Segmenting customers based on predicted LTV into four categories: Low, Mid-Low, Mid-High, and High.
7. **Visualization**: Plotting the distribution of predicted Customer LTV.

## Requirements
To run this project, you will need:
- Python 3.x
- Libraries: Pandas, NumPy, Scikit-learn, XGBoost, Matplotlib, Seaborn

You can install the required libraries using pip:
```bash
pip install pandas numpy scikit-learn xgboost matplotlib seaborn
```

## How to Run
1. Clone the repository:
   ```bash
   git clone <repository-url>
   ```
2. Navigate to the project directory:
   ```bash
   cd <project-directory>
   ```
3. Open the Jupyter Notebook:
   ```bash
   jupyter notebook customer_segment.ipynb
   ```
4. Run the cells in the notebook to perform the analysis.

## Conclusion
This project provides insights into customer behavior and helps businesses understand their customer base better through segmentation and LTV prediction. The models can be further refined and optimized for better accuracy.

