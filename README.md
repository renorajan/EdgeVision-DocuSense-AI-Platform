# EdgeVision DocuSense AI Platform

## Overview
Enterprise-grade Edge AI platform combining 
real-time industrial equipment monitoring with 
intelligent document processing, powered by 
NVIDIA Jetson Nano and Microsoft Azure.

## Architecture
```
[ESP32 Sensors] → [Jetson Nano Edge AI]
                        ↓
                 [Azure IoT Hub]
                        ↓
              [Microsoft Fabric]
              [Medallion Lakehouse]
                        ↓
              [Azure Databricks]
              [Delta Live Tables]
              [MLflow + Model Serving]
                        ↓
                 [Snowflake DW]
                    ↓        ↓
             [Streamlit]  [Power BI]
```

## Tech Stack

### Edge Layer
- NVIDIA Jetson Nano (CUDA 10.2)
- ESP32 IoT Controller
- DHT22 Temperature/Humidity Sensor
- MPU6050 Vibration/Accelerometer
- EMEET C950 1080P Camera

### AI/ML Models
- YOLOv5: Real-time object detection
- EasyOCR: Document text extraction
- LSTM: Equipment anomaly detection
- BERT: Document classification

### Cloud Platform
- Azure IoT Hub: Edge data ingestion
- Microsoft Fabric: Unified analytics
- Azure Databricks: ML engineering
- Snowflake: Data warehouse

### Visualization
- Power BI: Executive dashboards
- Streamlit in Snowflake: Operations UI

## Use Cases

### Equipment Health Monitoring
- Real-time temperature anomaly detection
- Vibration pattern analysis
- Predictive maintenance alerts
- Equipment failure prediction

### Document Intelligence
- Automated document scanning
- OCR text extraction
- Document classification
- Key data field extraction

## Project Structure
```
EdgeVision-DocuSense-AI-Platform/
├── edge/
│   ├── jetson/
│   │   ├── yolov5_detect.py
│   │   ├── ocr_pipeline.py
│   │   └── lstm_anomaly.py
│   └── esp32/
│       ├── sensor_read.ino
│       └── wifi_send.ino
├── cloud/
│   ├── fabric/
│   │   ├── eventstream_config.json
│   │   └── lakehouse_setup.py
│   ├── databricks/
│   │   ├── delta_live_tables.py
│   │   └── mlflow_training.py
│   └── snowflake/
│       └── streamlit_app.py
├── dashboard/
│   └── powerbi/
└── README.md
```

## Author
Reno Rajan Christy
Sr Data Engineer | AI Solutions Architect
LinkedIn: linkedin.com/in/renochristy
```


2. Click "Commit changes"
3. Add message: "Initial README"
4. Click "Commit changes" green button# EdgeVision-DocuSense-AI-Platform
EdgeVision-DocuSense-AI-Platform
