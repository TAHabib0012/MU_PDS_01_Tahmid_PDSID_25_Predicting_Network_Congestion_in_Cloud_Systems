# Predicting Network Congestion in Cloud_Systems

This project is the final step of my training program on Python and data science. It applies regression analysis on the IP Network and  Autonomous System Number dataset to predict network traffic, demonstrating end-to-end data science workflows, including data preprocessing, handling missing data, model training, evaluation, and visualization.

**Project Workflow**

1. **Data Preparation and Cleaning**
<br>**Data Loading:** Load cs448b_ipasn.csv and check for missing or anomalous values.
<br>**Preprocessing:** Clean the data by handling any missing values, normalizing traffic metrics, and creating derived features that capture temporal or network-specific patterns.

2. **Exploratory Data Analysis (EDA)**
<br>**Traffic Patterns:** Analyze traffic patterns over time to identify peak periods and congestion correlations.
<br>**IP and ASN Analysis:** Examine which IPs and ASNs are most associated with congestion, and check for any patterns that could help in feature engineering.
<br>**Visualizations:** Use matplotlib and seaborn to create visualizations that depict the relationships between network load metrics and congestion.

3. **Feature Engineering**
<br>**Traffic Trend Metrics:** Calculate trends and summary statistics from the traffic metrics to capture key congestion indicators.
<br>**Time-based Features:** Create features that reflect traffic peaks during different times or days, which might impact congestion.
<br>**Network-related Metrics:** Derive additional metrics such as IP density per ASN and network utilization metrics.

4. **Model Development**
<br>**Model Selection:** Test several regression models (such as Linear Regression, Decision Tree Regressor, and Random Forest Regressor) to determine the best-performing model.
<br>**Training:** Train the selected model(s) on the processed data, using cross-validation to ensure reliability.
<br>**Hyperparameter Tuning:** Optimize model parameters for better performance, using techniques like Grid Search or Randomized Search.

5. **Evaluation**
<br>**Performance Metrics:** Assess model performance using Mean Absolute Error (MAE), Mean Squared Error (MSE), and R-squared metrics.
<br>**Analysis:** Interpret model results to understand which features contribute most to congestion predictions and identify potential model limitations.
<br>**Visualization of Predictions:** Compare predicted congestion levels with actual data to visualize the model’s effectiveness.

6. **Optional: Deployment**
<br>**Web Integration:** (Optional) Use Flask to create a simple API for real-time congestion prediction, where users can input network parameters to get immediate predictions.
<br>**Example Usage**
To run the analysis and model development steps, open the Jupyter Notebook and execute the cells in sequence. Each section is labeled for easy navigation, from data preprocessing to model evaluation.

## Requirements

To run the code, you'll need:

- Python 3.x
- Libraries:
  - `numpy`
  - `pandas`
  - `scikit-learn`
  - `matplotlib`
  - `seaborn`
  - `Flask`(if applicable)

Install these libraries using:

```bash
pip install numpy pandas scikit-learn matplotlib seaborn
```

## Project Notebook

All code for the project is contained in a Google Colab notebook. [Download the notebook](link-to-notebook) and open it in Google Colab to view and execute the code directly.

**For example:**

1. Clone the repository and navigate to the directory.


      ```bash
      git clone https://github.com/TAHabib0012/MU_PDS_01_Tahmid_PDSID_25_Predicting_Network_Congestion_in_Cloud_Systems.git
      cd Predicting-Network-Congestion-in-Cloud-System
      ```

2. **Open the Colab Notebook**:

   Upload the notebook to your Google Drive and open it in Google Colab to run the code and explore the project in detail.

**Results and Discussion**

<br>The project demonstrates that by analyzing IP and network data, it's possible to predict congestion trends with reasonable accuracy. The final model, after tuning, achieves the following performance:

**MAE:** 47.035556504400944
<br>**MSE:** 40847.46250997291
<br>**R-squared:** 0.19372219837727
<br><br>These results suggest that certain features like traffic volume, ASN density, and peak time traffic patterns are key predictors of network congestion.

**Future Improvements**

<br>**Additional Data:** Integrating more data from other sources could improve model accuracy.
<br>**Real-Time Prediction:** Developing a real-time congestion prediction system with streaming data could make the model more applicable to real-world cloud systems.
<br>**Feature Expansion:** Additional feature engineering could further capture nuances in congestion patterns.

**License**

<br>This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

**Authors**
<br>**[Tahmid Ahmed Habib]**

**Acknowledgments**

<br>This project was developed as part of a regression analysis and machine learning study. Special thanks to the data providers and any contributors involved.

