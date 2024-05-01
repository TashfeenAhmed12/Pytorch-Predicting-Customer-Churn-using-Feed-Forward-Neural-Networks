# Objective
The primary objective of this project is to develop a predictive model using feed-forward neural networks to accurately identify customer churn. This involves extensive data preprocessing, experimenting with various network architectures, activation functions, and learning rates to optimize model performance. Predicting customer churn is crucial for businesses as it enables them to identify at-risk customers and implement effective retention strategies. By understanding the factors that influence churn, businesses can tailor their customer engagement and retention efforts, thereby reducing turnover and enhancing customer loyalty. This not only helps in sustaining revenue but also reduces the costs associated with acquiring new customers, adding significant value to the business.

# Data Description
The dataset used in this project contains various features related to customer demographics, service usage, and account details, essential for analyzing customer churn. You can find the dataset and more details on [Kaggle](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)

# Data Preprocessing / Feature Engineering
The preprocessing steps included handling missing values, standardizing numerical features, encoding categorical variables, and addressing class imbalance. The data was split into training, validation, and testing sets to ensure robust evaluation. Key transformations such as One-Hot Encoding for categorical variables and StandardScaler for numerical data were applied to prepare the dataset for neural network training.

# Modeling: Approach and Architecture
Two feed-forward neural network models were developed:

Basic Model: A three-layer network designed for initial exploration, using ReLU activation and Xavier weight initialization.

Enhanced Model: A more complex five-layer network with He initialization and hinge loss function to explore deeper interactions and enhance model robustness.

Both models underwent extensive hyperparameter tuning using grid search methods to optimize performance metrics such as accuracy, precision, recall, and F1 score.

# Results for Best Model
The best performing model from these experiments was chosen based on its validation performance, particularly focusing on the F1 score due to its relevance in balancing precision and recall effectively. Here's a summary of the model's performance:

| Metric       | Validation Set | Test Set |
|--------------|----------------|----------|
| Accuracy (%) | 74.37          | 76.57    |
| Precision (%)| 69.52          | 73.75    |
| Recall (%)   | 86.96          | 82.62    |
| F1 Score (%) | 77.27          | 77.93    |

Interpretation: The selected model demonstrated a high ability to identify potential churn, as indicated by the high recall and F1 score. The results suggest that the model is particularly effective in recognizing most true positive cases without a large number of false positives, which is crucial for practical applications in customer relationship management.

# Conclusion
This project illustrates the application of feed-forward neural networks in a practical business scenario, emphasizing the importance of comprehensive data preprocessing, strategic model building, and rigorous evaluation to achieve reliable predictive performance.
