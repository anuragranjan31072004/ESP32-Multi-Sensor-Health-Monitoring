# Experimental Results

This section presents the experimental results obtained from the implementation
of the ESP32-based Multi-Sensor Health Monitoring System. The system was tested
under real-time operating conditions to validate signal acquisition, sensor
integration, and data transmission reliability.

---

## 1. Real-Time ECG Signal Acquisition

The ECG signal was captured using the AD8232 analog front-end sensor interfaced
with the ESP32 ADC. The obtained waveform shows clear periodic peaks and troughs,
corresponding to normal cardiac activity. The morphology of the ECG signal
confirms correct electrode placement, proper signal conditioning, and sufficient
sampling rate of the ESP32.

The waveform maintains its structure despite minor baseline fluctuations, which
are attributed to motion artifacts and electrode contact variation.

**Related images:**
- `images/ecg_waveform_esp32_ad8232.png`
- `images/wide_view_ecg_signal.png`

---

## 2. Multi-Channel Real-Time Data Stream

The ESP32 successfully acquired and processed multiple physiological signals
simultaneously, including ECG, heart rate, SpO₂, and body temperature. The
multi-channel data stream confirms that the system can handle parallel sensor
inputs without data loss or cross-channel interference.

The stable operation of all channels validates the robustness of the system
architecture and efficient task handling by the ESP32 microcontroller.

**Related image:**
- `images/multi_channel_data_stream.png`

---

## 3. Temperature, SpO₂, and PPG Output Plot

A combined plot of body temperature, SpO₂, and PPG signals was generated to
visualize sensor stability and measurement consistency. The temperature values
remain steady over time, demonstrating the reliability of the DS18B20 digital
temperature sensor.

The PPG waveform and SpO₂ readings obtained from the MAX30102 sensor show smooth
variations, indicating accurate optical sensing and proper signal processing.

**Related image:**
- `images/temp_spo2_ppg_plot.png`

---

## 4. Serial Monitor Output

The ESP32 transmits real-time sensor readings to the serial monitor in a
comma-separated format. The output includes heart rate, SpO₂ percentage, and
body temperature values. The continuous and error-free data stream confirms
stable UART communication and correct sensor polling intervals.

This output format allows easy integration with external visualization tools
or cloud-based health monitoring platforms.

**Related image:**
- `images/serial_monitor_output.png`

---

## Summary of Results

The experimental evaluation confirms that the proposed system:
- Accurately captures real-time ECG signals
- Reliably measures heart rate, SpO₂, and body temperature
- Supports simultaneous multi-sensor data acquisition
- Provides stable real-time data transmission and visualization

Overall, the results validate the effectiveness of the ESP32-based multi-sensor
health monitoring system for portable biomedical applications, educational use,
and prototype-level healthcare monitoring solutions.

