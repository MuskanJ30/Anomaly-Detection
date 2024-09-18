
# Anomaly Detection in Time Series Data Using KMeans Scorer and Quantile Detector


### Project Description:

This project aims to develop and evaluate an anomaly detection system for time series data using advanced machine learning techniques. The focus is on detecting anomalies in industrial metrics represented by time series data from the ETTh2 dataset. This dataset includes various metrics related to machine performance and load usage, which are crucial for monitoring and maintaining industrial systems.


#### Data Preprocessing and Visualization:

Load and preprocess the ETTh2 dataset to extract relevant features, namely MUFL (Machine Utilization and Failure Level) and LULL (Load Usage Level).
Visualize the data to understand its structure and distribution, including training and validation subsets.

#### Anomaly Detection using KMeans Scorer:

Implement the KMeans Scorer from the Darts library to detect anomalies. This method uses KMeans clustering to identify deviations from normal patterns in the time series data.
Train the KMeans Scorer on the training subset and compute anomaly scores for the validation subset.

#### Quantile-Based Anomaly Detection:

Apply the Quantile Detector to convert the computed anomaly scores into binary anomaly flags. The detector uses quantile thresholds to distinguish between normal and anomalous data points.
Fine-tune the quantile threshold to optimize the detection performance.

#### Visualization of Results:

Plot the original time series data alongside the computed anomaly scores and detected anomalies. Use visualizations to highlight periods of anomalous behavior and validate the effectiveness of the detection methods.

#### Evaluation:

Assess the performance of the anomaly detection methods by analyzing the detected anomalies and comparing them with known anomalies, if available. Adjust parameters and thresholds to improve detection accuracy.

#### Tools and Libraries:

Python: Programming language used for implementation. 

Darts: A library for time series analysis and forecasting.

Matplotlib and Seaborn: Libraries for visualization of data and results.

Pandas: Library for data manipulation and analysis.


#### Outcome: 
The project will provide a robust anomaly detection framework for industrial time series data, showcasing the use of KMeans clustering and quantile-based methods. The results will be visualized to offer insights into the performance of the detection system and highlight potential areas for further improvement.

### Applications:

Industrial Monitoring: Detecting unusual patterns in machine utilization and load usage to preemptively address maintenance issues.
Quality Control: Identifying anomalies in manufacturing processes to ensure product quality.
Predictive Maintenance: Enhancing the reliability of industrial systems by forecasting potential failures based on historical data.
