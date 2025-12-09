# IoT-based Chlorine Detection System
An Arduino-based water quality monitoring project that measures Total Dissolved Solids (TDS), estimates chlorine levels, and reads turbidity values using analog sensors. This system is designed for real-time monitoring and can be extended into a fully functional IoT dashboard.

## Features
- Reads TDS levels (ppm) using an analog TDS sensor  
- Estimates chlorine levels based on TDS  
- Measures turbidity voltage through a turbidity sensor  
- Provides real-time output through Serial Monitor  
- Simple and extendable codebase for IoT applications  

## Hardware Requirements
| Component | Purpose |
|----------|----------|
| Arduino Uno / ESP32 / NodeMCU | Microcontroller board |
| TDS Sensor | Measures dissolved solids in water |
| Turbidity Sensor | Measures clarity of water |
| Jumper Wires | Wiring |
| 5V Power Supply | Sensor + board power |

## Pin Connections
| Sensor | Arduino Pin |
|--------|-------------|
| TDS Sensor | A1 |
| Turbidity Sensor | A0 |

## How It Works
### 1. TDS Measurement
- Reads analog value from sensor  
- Converts value into voltage  
- Converts voltage into TDS (ppm) using a linear relationship  

### 2. Chlorine Estimation
A basic linear model is used:

This can be calibrated more accurately using real sensor lab data.

### 3. Turbidity Measurement
- Reads analog input  
- Converts to voltage  
- Can be later mapped to NTU values with calibration  

![image](https://github.com/harshith7422/IoT-based-chlorine-detection-System/assets/89782073/37ebe2fc-ce71-4ee6-92ca-a3c18cf895b8)

![image](https://github.com/harshith7422/IoT-based-chlorine-detection-System/assets/89782073/f8bee905-768d-4b48-ab34-a15b2a7992dc)
