# Anomaly Detection
This repository contains a Python code snippet for performing anomaly detection using the Isolation Forest algorithm on a dataset of salaries in the data science field. Additionally, it includes the code for creating a dispersion plot to visualize the relationship between salary and years of work experience.

## Dataset
The code assumes that the salary data is stored in a CSV file named ds_salaries.csv. Adjust the file name or path accordingly.

The dataset should include two columns: work_year representing the years of work experience and salary_in_usd representing the corresponding salary in USD.

## Anomaly Detection
The code utilizes the Isolation Forest algorithm, a popular unsupervised learning algorithm, to detect anomalies in the salary data. It fits the Isolation Forest model to the extracted features and predicts the anomalies. The predictions are stored in a new column named 'Anomaly' in the dataframe.

## Dispersion Plot
The code also generates a dispersion plot to visualize the relationship between salary and years of work experience. It uses the scatter() function from the matplotlib library to create the plot. The x-axis represents the salary, and the y-axis represents the years of work experience.

Feel free to customize the code and adapt it to your specific dataset or requirements.

## License
This project is licensed under the MIT License.

## Acknowledgments
scikit-learn - Library for machine learning in Python.
matplotlib - Visualization library for Python.
Please feel free to contribute or provide any feedback.
