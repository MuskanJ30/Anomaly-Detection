
# Anomaly Detection in Time Series Data Using KMeans Scorer and Quantile Detector


### Project Description:

This project aims to develop and evaluate an anomaly detection system for time series data using advanced machine learning techniques. The focus is on detecting anomalies in industrial metrics represented by time series data from the ETTh2 dataset. This dataset includes various metrics related to machine performance and load usage, which are crucial for monitoring and maintaining industrial systems.


#### Data Preprocessing and Visualization:

Extracts relevant features from the ETTh2 dataset, specifically MUFL (Machine Utilization and Failure Level) and LULL (Load Usage Level). Visualizes the data to understand its structure and distribution, including training and validation subsets.

#### Anomaly Detection using KMeans Scorer:

The KMeans Scorer, from the Darts library, uses KMeans clustering to identify deviations from normal patterns in time series data. It clusters the data into k clusters and computes an anomaly score based on the distance of data points from the cluster centroids.

This method effectively identifies outliers by measuring how far data points deviate from normal clusters. It is well-suited for time series data where patterns and deviations are significant indicators of anomalies.

#### Quantile-Based Anomaly Detection:

The Quantile Detector converts computed anomaly scores into binary anomaly flags using quantile thresholds. It determines the threshold for anomalies based on the distribution of the scores.

By adjusting the quantile threshold, the detector can adapt to different levels of sensitivity. This allows for fine-tuning the detection system to balance between false positives and missed anomalies.

#### Visualization of Results:

Displays the original time series data, computed anomaly scores, and detected anomalies. Uses visualizations to highlight periods of anomalous behavior and validate the effectiveness of the detection methods.

#### Evaluation:

Assesses the performance of the anomaly detection methods by analyzing the detected anomalies and comparing them with known anomalies, if available. Adjusts parameters and thresholds to improve detection accuracy.

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
