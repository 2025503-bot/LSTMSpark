# A Hybrid LSTM Autoencoder and SMOTE-Balanced Classifier for Scalable Time Series Anomaly Detection on Apache Spark

**Dataset Sources:**
- NYC TLC: https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page
- NAB NYC Taxi: https://github.com/numenta/NAB/blob/master/data/realKnownCause/nyc_taxi.csv

Overview of the Project

This is a distributed project that implements an anomaly detection pipeline using Apache Spark (for large-scale processing of time-series data) with a deep LSTM Autoencoder and SMOTE-balanceed Random Forest for detecting anomalies in NYC taxi demand data.

This project contains two assignments:
- **Big Data Storage & Processing**: Apache Spark processed approximately 35M NYC taxi trip records (~792MB) across 12 monthly Parquet files using distributed window functions. 
- **Advanced Data Analytics:** A deep LSTM Autoencoder was trained to recognize normal demand patterns, SMOTE was used to address the 7.1:1 class imbalance, and a Random Forest was used to make the final predictions of anomalies.

Some of the notable anomaly events that we detected include: NYC Marathon (November 2nd), Thanksgiving (November 27th), Christmas (December 25th), New Years' Day (January 1st), Blizzard (January 27th).

