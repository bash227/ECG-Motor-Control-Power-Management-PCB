# ECG-Integrated Motor Control PCB  
**Final Project for BME405 - Introduction to Design of Medical Electronic Devices**  
*Ankara University, Department of Biomedical Engineering*  

---

## Project Overview  
A multi-functional PCB combining:  
- **ECG Signal Acquisition** (INA188 instrumentation amplifier, 0.5Hz-100Hz bandwidth)  
- **Power Management** (3.6V Li-ion charging, ±5V/12V regulation)  
- **Motor/Actuator Control** (BD6220F-E2 driver, relay circuits)  

![PCB 3D Render](https://github.com/bash227/ECG-Motor-Control-Power-Management-PCB/blob/main/Documentation/Images/real.jpg?raw=true)


---

## Team Members  
| Name              | Role                                  |  
|-------------------|---------------------------------------|  
| [bash227](https://github.com/bash227)| PCB Layout              |  
| [UmutAygun](https://github.com/UmutAygun)| Schematic Design          |  

---

## Repository Structure  
```plaintext
ECG_Motor_PCB/
├── Hardware/ 
│   │   
│   ├── Outputs/
│   └── 3D models/
├── Documentation/
└── README.md
```

## Key Features
### Power managment
- MCP73831 Li-ion charger (0.5A)
- TLV61070A boost converter (3.6V→5V)
- LMC7660 voltage inverter (+5V→-5V)

### ECG Frontend
- INA188 instrumentation amplifier (G=1000)
- 0.5Hz high-pass filter
- 50Hz notch filter

### Motor Control
- BD6220F-E2 DC motor driver
- AP8803WTG-7 LED driver
- Optoisolated relay control
---
##  Setup Guide
1. Clone the repository:
```bash
git clone https://github.com/yourusername/ECG-Motor-Control-PCB.git
```
2. Open in KiCad:
```bash
PCB_FINAL_UPDATED.kicad_pro
```
3. Set 3D model path in KiCad:
```bash
KICAD8_3DMODEL_DIR = ${KIPRJMOD}/Hardware/3D_Models
```
## Academic Information
- Course: BME405 - Introduction to Medical Electronics Design
- Institution: Ankara University


## License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

