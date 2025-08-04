# Fraud Detection Project

This project analyzes and detects fraudulent transactions using a dataset of financial transactions. The workflow includes data exploration, visualization, feature engineering, and building a machine learning model to classify transactions as fraudulent or not. The trained model is deployed using Streamlit for interactive visualization and prediction.

## Dataset

- The dataset is loaded from an Excel file (`Fraud.xlsx`).
- Key columns include transaction type, amount, balances, and fraud indicators.

## Steps Performed

1. **Data Exploration & Cleaning**
   - Checked for missing values and data types.
   - Explored class distribution for `isFraud` and `isFlaggedFraud`.
   - Visualized transaction types and fraud rates.

2. **Feature Engineering**
   - Created new features such as balance differences.
   - Filtered and analyzed suspicious patterns (e.g., zero balances after transfer).

3. **Visualization**
   - Plotted distributions of transaction amounts.
   - Visualized fraud rates by transaction type and over time.
   - Correlation heatmaps for key features.

4. **Model Building**
   - Selected features and split data into training and test sets.
   - Preprocessed data using scaling and one-hot encoding.
   - Built a pipeline with logistic regression (class weight balanced).
   - Evaluated model with classification report and confusion matrix.

5. **Model Saving**
   - Saved the trained pipeline using `joblib` for future use.

6. **Deployment with Streamlit**
   - Developed a Streamlit app for interactive visualization and prediction.
   - Users can upload transaction data and get real-time fraud predictions.
   - Visualizations of transaction patterns and model results are available in the app.

## Model Performance

- **Accuracy:** ~`your_accuracy_score`%
- **Precision (Fraud class):** ~`your_precision_score`

*(Replace the above with your actual scores, e.g., Accuracy: ~99.7%, Precision: ~76.5)*

## Requirements

- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- joblib
- streamlit

Install dependencies with:
```powershell
pip install pandas numpy matplotlib seaborn scikit-learn joblib streamlit
```

## Usage

1. Place `Fraud.xlsx` in the specified directory.
2. Run the notebook `Fraud_Detection.ipynb` step by step to train and save the model.
3. Start the Streamlit app:
   ```powershell
   streamlit run app.py
   ```
4. Use the web interface to visualize data and make predictions.

## Results

- The model provides classification metrics and a confusion matrix for fraud detection.
- Visualizations help understand transaction patterns and fraud distribution.
- The Streamlit app allows for interactive exploration and prediction.

## License

This project is for educational purposes.
