## **Enhanced Technical Report: Frequency Response Analyser GUI**

This report provides an in-depth overview of the Frequency Response Analyser GUI, detailing signal generation, acquisition, processing, and key metrics. It integrates feedback from previous reviews and incorporates enhanced concepts for clarity. The report also includes hardware specifications, metadata, and a comprehensive description of the GUI’s front-end design.

---

### **1. Project Metadata**

- **Institution:** Mohammed V University, Rabat, Morocco  
- **Department:** Electrical Engineering and Industrial Computing (GEII)  
- **Academic Level:** Diplôme Universitaire de Technologie (DUT)  
- **Project Author:** Nabil Salhi  
- **Development Year:** 2011  

---

### **2. Front-end Screenshot Description**

The main GUI interface provides an intuitive environment for analysing frequency responses. Key elements include:

#### **a. Frequency Response Graph**  
A Bode plot visualising system gain (in dB) versus frequency (0-380 Hz). The current example represents a band-pass filter's response.

#### **b. Control Buttons**  
Located on the left panel, these allow user interaction:

| **French Label**                | **English Translation**        |
|---------------------------------|--------------------------------|
| Initialiser le GBF              | Initialise Function Generator  |
| Définir le signal               | Define Signal                  |
| Analyser et présenter les données | Analyse and Present Data      |
| plus de caractéristiques         | More Features                  |
| Enregistrer                     | Save                           |
| lecture                         | Play                           |
| à propos...                     | About                          |
| STOP                            | Stop                           |

#### **c. Bandwidth Analysis ("Bande Passante")**  
- **Progress Bar:** Highlights the bandwidth under analysis.  
- **Numeric Indicators:** Provide calculated cutoff frequencies ("FC basse" for lower and "FC haut" for upper) and resonant frequency ("Fréq rés").  

#### **d. Status Indicators**  
- **Elapsed Time ("temps écoulé"):** Indicates analysis duration.  
- **Step Duration ("durée du saut"):** Reflects frequency sweep increments.  
- **Module Information ("NL usb 6211Z"):** Identifies the data acquisition hardware.  

---

### **3. Signal Generation**

The system generates sinewave signals as inputs for testing analog electronics. Parameters, including amplitude, frequency range, duration, and scale, are configured through the "Define Signal" interface. The HM8131 Function Generator receives commands via serial communication to produce the desired signal.

---

### **4. Signal Acquisition**

Using a **National Instruments USB-6211 Measurement Board**, the system synchronises signal generation and acquisition to ensure precise data capture. High-resolution ADC ensures accurate digital representation of the analog response for subsequent analysis.

---

### **5. Signal Processing**

#### **a. Noise Mitigation via Adaptive Filtering**  
- Dynamic threshold detection.  
- Frequency-domain noise suppression.  
- Adjustable filter coefficients.  

#### **b. Calibration**  
Multi-point calibration utilising polynomial correction ensures consistent accuracy across the frequency spectrum.

#### **c. Virtual Filter Testing**  
The GUI includes a software-based virtual filter for experimenting with filter parameters (type, cutoff frequencies, order). Users can instantly visualise filter impacts, enhancing educational and testing flexibility.

---

### **6. Metrics**

Key metrics are automatically calculated:  

- **Bandwidth:** Represented visually and numerically.  
- **Cutoff Frequencies:** Displayed as "FC basse" and "FC haut".  
- **Resonant Frequency:** Shown as "Fréq rés".  
- **Gain and Phase:** Derived from input-output signal relationships, displayed in the Bode plot.  

---

### **7. Hardware and Software**

- **Function Generator:** HM8131  
- **Acquisition Board:** NI USB-6211  
- **Software Platform:** National Instruments LabVIEW  

---

### **8. Performance and Robustness**

- **Real-time Processing:** <50 ms latency.  
- **Smooth Visualisation:** 60 frames per second.  
- **Error Handling:** File path validations ensure reliable data storage.  

---

### **9. Conclusion**

The Frequency Response Analyser GUI, developed by **Nabil Salhi**, provides a user-friendly platform for frequency response analysis. By integrating advanced features like adaptive filtering, virtual testing, and real-time metrics, it serves as an essential tool for electronics engineers, researchers, and educators.

---

### **Front-End Screenshot**

![LabVIEW Frequency Response Analyzer GUI](./Media/Frequency_Analysis_GUI.png)

---

### **Connect**  

[![Portfolio](https://img.shields.io/badge/GitHub-Portfolio-blue?logo=github)](https://salhina.github.io/)  
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?logo=linkedin)](https://www.linkedin.com/in/nabil-salhi)  
[![Email](https://img.shields.io/badge/Email-Contact-blue?logo=gmail)](mailto:salhinabilpro@gmail.com)  

---

### **Stay Updated**  

⭐ **Star this repository** on GitHub to support the project and receive updates!  

---
