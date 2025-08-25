# Customer-Lifetime-Value-Prediction
Understanding and predicting Customer Lifetime Value (CLV) is a key driver of strategic decision-making in retail, enabling organizations to identify high-value customers, tailor marketing campaigns, and optimize resource allocation. This project develops deep learning models to accurately estimate CLV for individual customers, defined as the total amount spent across all their transactions. The models leverage both demographic data and behavioral features aggregated at the customer level.

The dataset underwent rigorous preprocessing, including outlier detection, log-transformations for skewed variables, handling rare categories, and feature engineering to extract meaningful insights such as product category diversity and transaction history. Numerical and categorical features were prepared for model input using scaling, embedding, and grouping techniques as appropriate.

### Deep Learning Approaches
This project implements three advanced deep learning approaches for CLV prediction:

1. Tabular Neural Network with Embeddings
A traditional feedforward neural network that leverages learned embeddings for categorical features and direct processing of numerical features. The architecture includes multiple dense layers with dropout regularization, optimized through Bayesian hyperparameter tuning.

2. FTTransformer
An attention-based transformer model specifically tailored for tabular data. This model tokenizes both categorical and numerical features into embeddings and processes them through transformer blocks, capturing complex feature interactions through self-attention mechanisms.

3. Hybrid Residual Learning Model
A novel sequential ensemble approach that combines the strengths of both architectures through residual learning. The method works in two stages:

Stage 1: Train the FTTransformer to capture primary patterns and complex feature interactions
Stage 2: Train the Tabular Neural Network on the residuals (prediction errors) from the FTTransformer to capture systematic patterns that the transformer missed
This hybrid approach leverages the transformer's ability to model complex relationships while utilizing the tabular network's effectiveness at capturing local patterns and categorical embeddings.

### Model Performance (MAPE)
Tabular Neural Network: 8.38%
FTTransformer:	7.33%	
Hybrid Model:	2.29%	

This work demonstrates the power of deep learning for CLV prediction and underscores the value of data-driven strategies in enhancing customer management, retention, and targeted growth in the retail sector.
