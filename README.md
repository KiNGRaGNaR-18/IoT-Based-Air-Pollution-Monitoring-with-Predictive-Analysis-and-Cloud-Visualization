# IoT-Based Air Pollution Monitoring with Predictive Analysis and Cloud Visualization
 A real-time IoT-based air pollution monitoring system using ESP32, AWS, and Machine Learning for predictive analysis and cloud visualization.

# Features
 - ESP32-based Sensor Integration – Reads air pollution data in real-time.
 - Cloud Storage (AWS) – Stores data on an AWS EC2 instance with a database.
 - Machine Learning Predictions – Forecasts pollution levels using AI models.
 - Live AQI API Integration – Compares sensor data with official AQI sources.
 - Grafana Dashboard – Displays real-time & predicted pollution levels.
 - Alerts & Notifications – Sends warnings for high pollution levels (optional).

# Technologies Used
 - Hardware: ESP32, PM2.5/PM10 Sensors, MQ-7 (CO), MQ-135 (NO2, VOCs)
 - Software: C++ (Arduino), Python (Flask/FastAPI)
 - Cloud: AWS EC2, PostgreSQL/InfluxDB
 - Machine Learning: Scikit-learn, TensorFlow (LSTM, Random Forest)
 - Visualization: Grafana, Plotly

# System Architecture
  ![Screenshot 2025-03-18 191754](https://github.com/user-attachments/assets/f136105d-8f36-4ec1-8d6f-f49e8af87c43)

# Installation & Setup
 - Hardware Setup
    - Connect ESP32 with sensors (PM2.5, CO, NO2, etc.).
    - Upload ESP32 code (/esp32-code) to the board using Arduino IDE.
      
 - Backend Setup (AWS & API)
    - Set up AWS EC2 instance (Ubuntu).
    - Clone this repository:
        - git clone https://github.com/your-username/IoT-Based-Air-Pollution-Monitoring-with-Predictive-Analysis-and-Cloud-Visualization.git
        - cd IoT-Based-Air-Pollution-Monitoring-with-Predictive-Analysis-and-Cloud-Visualization
    - Install required dependencies:
        - pip install flask influxdb pandas numpy
    - Run the API Server:
        - python server.py
      
 - Machine Learning Model
    - Train ML model (/ml-model/train_model.py) with historical AQI data.
    - Deploy the model to make predictions on new sensor data.
    
 - Grafana Dashboard Setup
    - Install & configure Grafana.
    - Connect it to InfluxDB/PostgreSQL.
    - Create graphs, trends, and alerts based on sensor & predicted data.

#  How It Works
 - ESP32 reads air quality data from connected sensors.
 - Sends data to AWS cloud for processing & storage.
 - Backend API stores & retrieves data for real-time access.
 - Machine Learning model predicts future pollution levels.
 - Grafana Dashboard displays real-time & forecasted data.

# Project Screenshots

 
# Contributors
 - 1
 - 2
 - 3
