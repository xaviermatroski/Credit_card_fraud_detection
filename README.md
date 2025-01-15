# Credit Card Fraud Detection

Welcome to the **Credit Card Fraud Detection** project! This repository presents an end-to-end solution for identifying fraudulent credit card transactions using the dataset from [Kaggle](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud). The project applies data preprocessing, feature engineering, and machine learning techniques to effectively classify fraudulent and non-fraudulent transactions.

## Dataset Overview 🔍
The dataset contains transactions made by European cardholders in September 2013. It includes a total of **284,807 transactions**, out of which only **492 are fraudulent** (representing **0.172% of all transactions**). Each transaction is characterized by:
- **Time**: Seconds elapsed between this transaction and the first transaction in the dataset.
- **Amount**: Transaction amount.
- **V1, V2, ..., V28**: Principal components obtained using PCA.
- **Class**: Target variable, where 1 represents fraud and 0 represents non-fraud.

## Key Features of This Project 🚀

1. **Exploratory Data Analysis (EDA):**
   - Visualized the class imbalance in the dataset.
   - Analyzed correlations between features and the target variable.

2. **Data Preprocessing:**
   - Handled class imbalance using oversampling techniques like SMOTE.
   - Scaled the features for better performance with machine learning algorithms.

3. **Machine Learning Models:**
   - Trained and evaluated multiple models, including:
     - Logistic Regression
     - Random Forest
     - Gradient Boosting
     - Support Vector Machine
   - Compared metrics such as accuracy, precision, recall, F1-score, and AUC-ROC.

4. **Evaluation Metrics:**
   - Prioritized metrics like **Precision**, **Recall**, and **F1-score** due to the highly imbalanced nature of the dataset.

## Results 🎯
### Undersampling

#### Logistic Regression
- **Accuracy**: 0.9526
- **Precision**: 1.0000
- **Recall**: 0.9118
- **F1 Score**: 0.9538

#### Decision Tree Classifier
- **Accuracy**: 0.8789
- **Precision**: 0.8835
- **Recall**: 0.8922
- **F1 Score**: 0.8878

### Oversampling

#### Logistic Regression
- **Accuracy**: 0.9446
- **Precision**: 0.9728
- **Recall**: 0.9148
- **F1 Score**: 0.9429

#### Decision Tree Classifier
- **Accuracy**: 0.9981
- **Precision**: 0.9973
- **Recall**: 0.9988
- **F1 Score**: 0.9981

### Base

#### Logistic Regression
- **Accuracy**: 0.9993
- **Precision**: 0.8906
- **Recall**: 0.6264
- **F1 Score**: 0.7355

#### Decision Tree Classifier
- **Accuracy**: 0.9989
- **Precision**: 0.6535
- **Recall**: 0.7253
- **F1 Score**: 0.6875

## How to Run the Project 🖥️

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/credit-card-fraud-detection.git
   cd credit-card-fraud-detection
   ```
2. Install required packages:
   ```bash
   pip install -r requirements.txt
   ```
3. Download the dataset from [Kaggle](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud) and place it in the `data/` directory.
4. Run the Jupyter Notebook:
   ```bash
   jupyter notebook Credit_card_fraud_detection_model.ipynb
   ```

## Next Steps 📈
- Experiment with additional ensemble models.
- Optimize hyperparameters using advanced techniques like Grid Search and Random Search.
- Deploy the model using Flask or Streamlit for real-world applications.

## Contributions 🌟
Feel free to fork this repository and create a pull request for any improvements or new ideas. Feedback and suggestions are always welcome!

## Acknowledgments 🙌
- Dataset by the [Machine Learning Group - ULB](https://www.ulb.ac.be/)
- Kaggle for providing an excellent platform for data science enthusiasts.

---

**Let’s detect and prevent fraud together!**

