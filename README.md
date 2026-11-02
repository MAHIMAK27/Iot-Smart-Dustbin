# ♻️ Smart Waste Identification System

## 📌 Project Overview

The **Smart Waste Identification System** is an Arduino-based project designed to identify and classify waste into two categories: **Wet Waste and Dry Waste** using a soil moisture sensor.

The system measures the moisture level of the waste material and uses a predefined threshold value to determine its category. Multiple sensor readings are collected and averaged to improve measurement stability and classification.

## 🎯 Objectives

- Identify wet and dry waste using a moisture sensor.
- Measure moisture levels in waste materials.
- Automatically classify waste based on sensor readings.
- Reduce manual effort in basic waste identification.
- Promote smart waste management and segregation.

## 🛠️ Components Required

| Component | Quantity |
|---|---:|
| Arduino Uno | 1 |
| Soil Moisture Sensor | 1 |
| Jumper Wires | As required |
| USB Cable | 1 |
| Computer with Arduino IDE | 1 |

## 🔌 Circuit Connections

| Soil Moisture Sensor | Arduino Uno |
|---|---|
| VCC | 5V |
| GND | GND |
| AO | A0 |

**Note:** The sensor's analog output (AO) is connected to pin A0 to measure moisture levels.

## ⚙️ Working Principle

1. The soil moisture sensor detects the moisture level of the waste material.
2. Arduino Uno reads the analog sensor values through pin A0.
3. The system collects 10 sensor readings with a 50 ms delay between readings.
4. The average sensor value is calculated.
5. The calculated value is compared with the predefined threshold of 800.
6. The waste is classified based on the following conditions:

   - **Wet Waste:** Sensor value below 800.
   - **Dry Waste:** Sensor value greater than or equal to 800.

7. The classification result is displayed in the Serial Monitor.

## 💻 Software Requirements

- Arduino IDE
- Arduino Uno Board Package
- USB Driver (if required)

```

## 🚀 How to Run the Project

1. Connect the soil moisture sensor to the Arduino Uno.
2. Open Arduino IDE on your computer.
3. Copy and paste the Arduino code.
4. Select **Arduino Uno** under Tools → Board.
5. Select the correct COM port under Tools → Port.
6. Click the Upload button.
7. Open Serial Monitor.
8. Set the baud rate to **9600**.
9. Place the sensor in contact with the waste material and observe the classification output.

## 📊 Sample Output

```text
SMART WASTE IDENTIFICATION SYSTEM

Sensor Value: 450 ==> WET WASTE
Sensor Value: 620 ==> WET WASTE
Sensor Value: 850 ==> DRY WASTE
Sensor Value: 920 ==> DRY WASTE
```

*Note: These are illustrative readings. Actual values depend on the sensor, material, and testing conditions.*

## 🔍 Classification Logic

| Sensor Reading | Classification |
|---|---|
| Below 800 | Wet Waste |
| 800 and above | Dry Waste |

The threshold value can be adjusted based on experimental sensor readings.

## 🌱 Applications

- Smart waste segregation systems.
- Automated waste management.
- Educational IoT and Arduino projects.
- Basic moisture-based waste identification.
- Sustainable environmental management.

## 🔮 Future Enhancements

- Integration of a servo motor for automatic waste separation.
- Addition of ultrasonic sensors for waste detection.
- Integration of IoT for real-time waste monitoring.
- Development of a smart dustbin with separate wet and dry compartments.
- Addition of advanced sensors for improved waste classification.

## 👩‍💻 Technologies Used

- Arduino Uno
- Embedded C/C++
- Soil Moisture Sensor
- Arduino IDE

## 📌 Conclusion

The Smart Waste Identification System demonstrates a basic approach to automated waste classification using Arduino Uno and a soil moisture sensor. By measuring moisture levels and comparing them against a predefined threshold, the system identifies wet and dry waste, supporting the development of smarter and more sustainable waste management solutions.

---

**Project Name:** Smart Waste Identification System  
**Controller:** Arduino Uno  
**Sensor:** Soil Moisture Sensor  
**Classification:** Wet Waste / Dry Waste
