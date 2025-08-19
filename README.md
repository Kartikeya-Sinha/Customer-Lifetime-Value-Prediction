# Customer-Lifetime-Value-Prediction
Understanding and predicting Customer Lifetime Value (CLV) is a key driver of strategic decision-making in retail, enabling organizations to identify high-value customers, tailor marketing campaigns, and optimize resource allocation. This project develops deep learning models to accurately estimate CLV for individual customers, defined as the total amount spent across all their transactions. The models leverage both demographic data and behavioral features aggregated at the customer level.

The dataset underwent rigorous preprocessing, including outlier detection, log-transformations for skewed variables, handling rare categories, and feature engineering to extract meaningful insights such as product category diversity and transaction history. Numerical and categorical features were prepared for model input using scaling, embedding, and grouping techniques as appropriate.

For predictive modeling, two deep learning approaches have been used: a Tabular Neural Network with Embeddings, and the FTTransformer—an attention-based transformer model tailored for tabular data. Model hyperparameters were optimized through Bayesian optimization, with early stopping used to prevent overfitting. Performance was evaluated using the metric Mean Absolute Percentage Error (MAPE), with the FTTransformer achieving the best predictive accuracy.

This work demonstrates the power of deep learning for CLV prediction and underscores the value of data-driven strategies in enhancing customer management, retention, and targeted growth in the retail sector.
