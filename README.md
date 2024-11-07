Predicting_Network_Congestion_in_Cloud_Systems
This project is the final step of my training program on Python and data science. It applies regression analysis on the Diabetes dataset to predict network traffic, demonstrating end-to-end data science workflows, including data preprocessing, handling missing data, model training, evaluation, and visualization.

Project Workflow
1. Data Preparation and Cleaning
Data Loading: Load cs448b_ipasn.csv and check for missing or anomalous values.
Preprocessing: Clean the data by handling any missing values, normalizing traffic metrics, and creating derived features that capture temporal or network-specific patterns.
2. Exploratory Data Analysis (EDA)
Traffic Patterns: Analyze traffic patterns over time to identify peak periods and congestion correlations.
IP and ASN Analysis: Examine which IPs and ASNs are most associated with congestion, and check for any patterns that could help in feature engineering.
Visualizations: Use matplotlib and seaborn to create visualizations that depict the relationships between network load metrics and congestion.
3. Feature Engineering
Traffic Trend Metrics: Calculate trends and summary statistics from the traffic metrics to capture key congestion indicators.
Time-based Features: Create features that reflect traffic peaks during different times or days, which might impact congestion.
Network-related Metrics: Derive additional metrics such as IP density per ASN and network utilization metrics.
4. Model Development
Model Selection: Test several regression models (such as Linear Regression, Decision Tree Regressor, and Random Forest Regressor) to determine the best-performing model.
Training: Train the selected model(s) on the processed data, using cross-validation to ensure reliability.
Hyperparameter Tuning: Optimize model parameters for better performance, using techniques like Grid Search or Randomized Search.
5. Evaluation
Performance Metrics: Assess model performance using Mean Absolute Error (MAE), Mean Squared Error (MSE), and R-squared metrics.
Analysis: Interpret model results to understand which features contribute most to congestion predictions and identify potential model limitations.
Visualization of Predictions: Compare predicted congestion levels with actual data to visualize the model’s effectiveness.
6. Optional: Deployment
Web Integration: (Optional) Use Flask to create a simple API for real-time congestion prediction, where users can input network parameters to get immediate predictions.
Example Usage
To run the analysis and model development steps, open the Jupyter Notebook and execute the cells in sequence. Each section is labeled for easy navigation, from data preprocessing to model evaluation.

For example:

Clone the repository and navigate to the directory.

Run the following command to open Jupyter Notebook:

bash
Copy code
jupyter notebook Predicting_Network_Congestion_in_Cloud_Systems.ipynb
Follow the cells in the notebook for each step in data preparation, analysis, and model training.

Results and Discussion
The project demonstrates that by analyzing IP and network data, it's possible to predict congestion trends with reasonable accuracy. The final model, after tuning, achieves the following performance:

MAE: 47.035556504400944
MSE: 40847.46250997291
R-squared: 0.19372219837727
These results suggest that certain features like traffic volume, ASN density, and peak time traffic patterns are key predictors of network congestion.

Future Improvements
Additional Data: Integrating more data from other sources could improve model accuracy.
Real-Time Prediction: Developing a real-time congestion prediction system with streaming data could make the model more applicable to real-world cloud systems.
Feature Expansion: Additional feature engineering could further capture nuances in congestion patterns.
License
This project is licensed under the MIT License. See the LICENSE file for more details.

Authors
[Tahmid Ahmed Habib]

Acknowledgments
This project was developed as part of a regression analysis and machine learning study. Special thanks to the data providers and my teacher for his contribution.
