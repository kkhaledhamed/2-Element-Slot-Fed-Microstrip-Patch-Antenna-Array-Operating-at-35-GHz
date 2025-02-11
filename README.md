# 2-Element Slot-Fed Microstrip Patch Antenna Array at 35 GHz

## Project Overview
This project presents the design and simulation of a **2-element slot-fed microstrip patch antenna array** operating at **35 GHz** for millimeter-wave applications such as **5G communications, radar systems, and high-speed wireless networks**. The slot-coupled feeding mechanism enhances **bandwidth, impedance matching, and gain**, ensuring an optimized directional radiation pattern.

## Key Features
- **Frequency of Operation:** 35 GHz
- **Antenna Type:** 2-element slot-fed microstrip patch array
- **Substrate Material:** Rogers RT/duroid 5880 (εr = 2.2, tanδ = 0.0009)
- **Feeding Mechanism:** Slot-coupled feed

### **Performance Metrics:**
- **Return Loss (S11):** ≈ -12 dB at 35 GHz with 2 GHz bandwidth
- **Peak Gain:** 7.01 dBi
- **Radiation Pattern:** Unidirectional with minimal side lobes
- **Radiation Efficiency:** ~1.013 (excellent power conversion)
- **Front-to-Back Ratio:** 21.52 dB
- **VSWR:** 1.69 at 35 GHz
- **Input Impedance:** 41.51 + j22.55 Ω, requiring a matching network

---

## Design Procedure
The design process involves the following key steps:

### **1. Substrate Selection**
- **Material:** Rogers RT/duroid 5880 (εr = 2.2, tanδ = 0.0009)
- **Substrate heights:**
  - **h1:** 0.254 mm
  - **h2:** 0.4 mm

### **2. Patch Design**
- **Patch dimensions:**
  - **Width:** 2.37 mm
  - **Length:** 2 mm
- **Substrate dimensions:**
  - **Width:** 8 mm
  - **Length:** 5 mm

### **3. Slot Design**
- **Slot dimensions:**
  - **Width:** 1.98 mm
  - **Length:** 0.16 mm

### **4. Microstrip Feedline**
- **Microstrip dimensions:**
  - **Width:** 0.1604 mm
  - **Length:** 3.6 mm

### **5. Power Divider**
- **T-junction power divider** with **impedance matching** to ensure uniform power distribution.
- **Final impedance after optimization:** Zo = 41 Ω.
- **Width of lateral microstrip:** 2.9 mm.

---

## Simulation and Results
The antenna was simulated using **HFSS (High-Frequency Structure Simulator)**. Key findings:

### **Return Loss (S11)**
- Achieved **-12 dB at 35.17 GHz** with **≈2 GHz bandwidth**.
- Low reflection ensures high signal efficiency.

### **Radiation Pattern**
- **E-plane:** Cross-polarization of **-35.04 dB**.
- **H-plane:** Cross-polarization of **-37.81 dB**.

### **Gain and Efficiency**
- **Peak gain:** 7.01 dBi at 35 GHz.
- **Radiation efficiency:** ~1.013, indicating minimal power loss.

### **Additional Parameters**
- **Front-to-back ratio:** 21.52 dB.
- **VSWR:** 1.69 at 35 GHz (low signal loss due to reflection).

---

## Effect of Element Spacing
The distance between array elements affects **gain, mutual coupling, and compactness**:

### **High Distance**
- **Peak gain:** 5.24 dBi
- **Mutual coupling:** -17.58 dB
- **Advantages:** Improved gain & impedance matching.
- **Disadvantages:** Potential grating lobes, reduced compactness.

### **Low Distance**
- **Peak gain:** 4.41 dBi
- **Mutual coupling:** -14.45 dB
- **Advantages:** Compact size, reduced grating lobes.
- **Disadvantages:** Increased mutual coupling, reduced gain.

---

## Equivalent Circuit Model
An **equivalent circuit model** was developed in **ADS (Advanced Design System)** for validation.

### **Optimized Component Values**
- **R1:** 139.854 Ω, **R2:** 195.445 Ω
- **L1:** 3.9756 nH, **L2:** 236.781 pH
- **C1:** 4.46897 fF, **C2:** 85.66319 fF

The model was fine-tuned to closely match the **antenna's return loss (S11) performance**.

---

## Future Work
- **Beamforming Integration:** Extend the design for **dynamic beam steering**.
- **Multi-Band Operation:** Modify the design to support **multiple frequency bands**.
- **Advanced Feeding Networks:** Explore alternative feeding techniques for **better impedance matching and bandwidth enhancement**.

---

## References
1. **Rogers Corporation**, *Helping power, protect and connect our world*, [Rogerscorp.com](https://rogerscorp.com)
2. **Microstrip Patch Antenna Calculator**, *Pasternack*, [Link](https://www.pasternack.com/t-calculator-microstrip-ant.aspx)
3. **M. Alia, M. Z. Azmi, and M. N. M. Nasir**, *Design of Rectangular Microstrip Patch Antenna Using Aperture Coupled Fed for S-Band Application*, *ResearchGate*, [Link](https://www.researchgate.net/publication/338365982)
4. **Microstrip Width Calculator**, *everything RF*, [Link](https://www.everythingrf.com/rf-calculators/microstrip-width-calculator)

---

## Team Members
- **Khaled Ahmed Hamed**
- **Dalia Mohamed Soliman**
- **Zeyad Ashraf Abdelaziz**
- **Zeyad Antar Othman**
- **Sarah Abdelatty Ibrahem**
- **Ali Mohamed Mohamed Said**

### **Supervisor**
- **Prof. Eslam A. Eshrah**
