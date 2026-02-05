# 🩺 ESP32 Multi-Sensor Portable Health Monitoring System

## 📌 Overview
This project presents a **real-time portable health monitoring system** using the **ESP32 microcontroller**.  
The system simultaneously acquires and processes multiple biomedical parameters including **ECG, heart rate, SpO₂, and body temperature**, making it suitable for educational, prototype, and non-clinical biomedical applications.

---

## 🎯 Objectives
- Design a multi-sensor biomedical data acquisition system  
- Capture and visualize real-time ECG signals  
- Measure heart rate, SpO₂, and body temperature  
- Validate signal quality and sensor reliability  
- Analyze results using waveform plots and serial data  

---

## 🧠 System Architecture

### Sensors Used
| Parameter | Sensor |
|---------|--------|
| ECG | AD8232 |
| Heart Rate & SpO₂ | MAX30102 |
| Temperature | DS18B20 |
| Controller | ESP32 |

### Functional Flow
1. Sensor signal acquisition  
2. Analog-to-digital conversion (ADC)  
3. Signal conditioning and filtering  
4. Real-time visualization  
5. Serial data monitoring  

---

## 🛠️ Hardware Setup
- ESP32 Development Board  
- AD8232 ECG module with electrodes  
- MAX30102 pulse oximeter sensor  
- DS18B20 digital temperature sensor  
- Breadboard, jumper wires, USB power  

Hardware connection diagrams and physical setup images are available in the **images** folder.

---

## 💻 Software Implementation
- **Platform:** Arduino IDE  
- **Programming Language:** C / C++  
- **Communication:** Serial interface  
- **Processing:** Handled directly on ESP32  

The source code and modular structure are available inside the **src** directory.

---

## 📁 Repository Structure
ESP32-Multi-Sensor-Health-Monitoring



├── docs/ → Project report and reference papers


├── images/ → System diagrams, waveforms, plots


├── results/ → Experimental observations and outcomes


├── src/ → Source code


├── README.md → Main project documentation


└── Reference_paper.pdf


---

## 🖼️ Visual Results & Outputs
All figures used in analysis are stored in the **images** folder.

### Included Images
- System block diagram  
- Hardware circuit diagram  
- Hardware setup  
- ECG waveform captured using AD8232  
- Wide-view ECG signal  
- Multi-channel real-time data stream  
- Temperature, SpO₂, and PPG plot  
- Serial monitor output  

Each image is described in `images/README.md`.

---

## 📊 Experimental Results
- Clear ECG waveform with identifiable peaks  
- Stable heart rate and SpO₂ readings  
- Accurate digital temperature measurement  
- Reliable multi-channel data handling  
- Minimal noise and distortion under normal conditions  

Detailed interpretation is provided in the project report.

---

## 📄 Documentation

### 📘 Project Report
**File:** `docs/Project_Report_BML.pdf`  
Contains complete academic documentation including methodology, design, testing, and result analysis.

### 📚 Reference Paper
**File:** `docs/Reference_paper.pdf`  
Provides theoretical background and literature support for biomedical signal acquisition.

---

## 📌 Applications
- Educational biomedical projects  
- Prototype health monitoring systems  
- Wearable device research  
- IoT-based healthcare solutions  
- Academic demonstrations  

---

## 🚀 Future Scope
- Cloud-based IoT dashboards  
- Mobile application integration  
- Data logging and analytics  
- AI-based health anomaly detection  
- Compact wearable enclosure design  

---

## 🔧 Tools & Technologies
- ESP32  
- Arduino IDE  
- Biomedical sensors  
- Embedded C/C++  
- Serial communication  
- Signal processing  

---

## 📜 License
This project is intended for **educational and non-commercial use only**.

---

## 🙌 Acknowledgements
This project was developed as part of an academic biomedical engineering initiative and inspired by real-world healthcare monitoring challenges.
