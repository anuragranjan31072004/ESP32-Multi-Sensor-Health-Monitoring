# Multi-Sensor Portable Health Monitoring System using ESP32

## Overview
This project presents a real-time biomedical health monitoring system using an ESP32 microcontroller. The system integrates multiple physiological sensors to continuously measure ECG, heart rate, oxygen saturation (SpO2), and body temperature with local signal processing and display.

The design focuses on compactness, low power consumption, and reliable vital-sign acquisition without relying on external networks.

---

## Sensors Used
- **AD8232 ECG Module**
  - Low-noise analog front-end for ECG acquisition
  - Enables visualization of PQRST waveform features
- **MAX30102**
  - Optical sensor for heart rate and SpO2 measurement
  - Uses photoplethysmography (PPG)
- **DS18B20**
  - Digital temperature sensor using 1-Wire protocol
  - High accuracy and noise immunity

---

## System Architecture
- ESP32 microcontroller
- Local signal acquisition and processing
- Serial plotter / local display output
- No cloud or IoT dependency

All physiological signals are processed locally on the ESP32.

---

## Signal Processing Workflow

### ECG Processing
- Analog signal acquisition from AD8232
- Filtering and amplification
- R-peak detection
- ECG waveform visualization

### Heart Rate & SpO2
- I²C communication with MAX30102
- AC/DC component extraction
- Ratio-of-ratios computation
- Heart rate estimation from PPG peaks

### Temperature Measurement
- Digital temperature acquisition via DS18B20
- Direct ESP32 interface using 1-Wire protocol

---

## Results
- Clear ECG waveform with identifiable P, QRS, and T components
- Stable heart rate and SpO2 values within physiological range
- Accurate body temperature readings
- Reliable real-time performance with low delay

---

## Applications
- Personal health monitoring
- Biomedical embedded systems
- Continuous vital-sign assessment
- Medical support and academic research

---

## Future Enhancements
- Machine-learning-based arrhythmia detection
- Advanced filtering techniques
- Alarm system for abnormal vitals
- Wearable enclosure design
- Battery-powered continuous operation
