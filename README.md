# Industrial-Combustion-Control-TIA-Portal
PLC-based industrial combustion control system designed in Siemens TIA Portal with integrated WinCC HMI visualization.
# Industrial Combustion Control System (TIA Portal + WinCC)

This project is the final assignment for the *Industrial Automation* course at the University of Tehran.  
It demonstrates the design and simulation of an **industrial combustion control system** for molten salt heating, using **Siemens TIA Portal** and **WinCC HMI**.

---

##  System Overview

The system simulates and controls an **industrial burner** that manages air and methane gas ratios to maintain proper combustion conditions for molten salt heating.  
It includes both **digital** and **analog** inputs/outputs, as well as a **Human–Machine Interface (HMI)** for monitoring and manual control.

### Main Functional Components
- **Digital Inputs/Outputs:** Start/Stop buttons, burner activation, emergency stop  
- **Analog Inputs:** Temperature sensors (2 thermocouples), air flow transmitter, gas flow transducer  
- **Analog Outputs:** Blower speed control (via inverter), gas valve position  
- **Burner & Ignition Control:** Safe startup (Pre-purge), ignition, and stable combustion sequence  
- **Temperature Control:** Maintain molten salt within desired limits (using setpoints)

---

##  Control Logic (PLC)

The control logic is implemented in **Ladder Logic (LAD)** and **SCL** within TIA Portal.

### Key Operations
1. **Pre-Purge Sequence:** Ensures system safety before ignition  
2. **Air–Fuel Ratio Control:** Dynamically adjusts gas and air flow to maintain proper combustion  
3. **Temperature Feedback Loop:** Monitors dual thermocouples and controls burner activation  
4. **Emergency Handling:** Implements safe shutdown on abnormal readings

---

##  HMI Design (WinCC)

The WinCC HMI provides real-time monitoring and control of:
- System states (Burner ON/OFF, Pre-Purge, Alarms)
- Analog sensor readings (Temperature, Flow rates)
- Manual adjustment of setpoints
- Visualization of process equipment (burner, blower, coils, valves)

> Example screens: Main Control Panel, Setpoint Configuration, Process Visualization

---

##  Simulation Environment

Developed and tested using:
- **Siemens TIA Portal V17**
- **PLCSIM Advanced**
- **WinCC Runtime**
- Simulated analog sliders and digital buttons for input testing

---

## 🧩Hardware (Simulated)

- Siemens PLC (S7-300/400 series)
- Inverter for blower motor control
- Solenoid valves for gas and air flow
- Thermocouples (for molten salt coils)

---

##  Setpoints & Timing

| Parameter | Description | Default |
|------------|--------------|----------|
| Setpoint1 | Air-to-fuel ratio | 10 |
| Setpoint2 | Temperature target (°C) | 1000 |
| T1 | Pre-purge duration (s) | 10 |
| T2 | Delay after ignition (s) | 20 |
| T3 | Burner ON duration (s) | 15 |
| T4 | Burner OFF duration (s) | 5 |

---


## Author

**Negar Shamaie**  
B.Sc. Electrical Engineering (Control Systems)  
University of Tehran  
 negar.shamaie83@gmail.com  
[GitHub](https://github.com/Negar-shamaie)


