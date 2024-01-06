### NASA Asteroids Classification 
### Overview
This case study focuses on the classification of asteroids using the NASA Asteroids dataset obtained from the Near Earth Object Web Service (NeoWs). The goal is to predict whether an asteroid is hazardous or not based on its characteristics. The study utilizes the XGBoost algorithm, Bayesian Optimization, and RandomizedSearchCV to achieve accurate classification.

### Dataset
The dataset comprises 4687 rows and 40 columns with various attributes of asteroids. The information includes details such as the closest approach date to Earth, NASA JPL small body ID, and features related to the asteroid's characteristics. The dataset link is here.

### Data Preprocessing
Correlation Heatmap
The initial step involves loading the dataset and examining the correlation between different features. A correlation heatmap is generated to visualize relationships among variables.

### Feature Selection
Certain irrelevant or highly correlated features are dropped to enhance the efficiency of the model. The 'Est Dia' and 'Miss Dist' columns, along with other unnecessary attributes, are removed.

### Data Scaling
The features are scaled using RobustScaler to ensure a standardized range for model training.

### Model Training
XGBoost Classification
The dataset is split into training and testing sets. An XGBoost classifier is trained on the scaled data to predict whether an asteroid is hazardous. The model's performance is evaluated using accuracy metrics.

### Hyperparameter Tuning - RandomizedSearchCV
RandomizedSearchCV is employed to fine-tune hyperparameters of the XGBoost model. The parameters considered include the learning rate, number of estimators, and maximum depth.

### Hyperparameter Tuning - Bayesian Optimization
Bayesian Optimization is used for further hyperparameter tuning. The algorithm explores the hyperparameter space to find the optimal combination that maximizes accuracy.

### Model Evaluation
The final models are evaluated on the test set, and classification reports are generated, providing insights into precision, recall, and accuracy. The results of RandomizedSearchCV and Bayesian Optimization are compared.

### Additional Libraries
The implementation uses scikit-optimize (skopt) for Bayesian Optimization and Optuna for another hyperparameter optimization approach.

### Results
The classification reports and accuracy scores are presented, showcasing the effectiveness of the XGBoost algorithm in asteroid classification. The impact of hyperparameter tuning on model performance is highlighted.

### Conclusion
This case study demonstrates the application of XGBoost, RandomizedSearchCV, and Bayesian Optimization for asteroid classification. The insights gained can contribute to identifying potential hazardous asteroids and improving our understanding of their characteristics.

Author
Ilaha Musayeva
09/09/23
