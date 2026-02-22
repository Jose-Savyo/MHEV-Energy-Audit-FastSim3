# 🚗 Hybrid Vehicle Energy Audit Study (MHEV/HEV)

This repository contains a technical study on the energy efficiency of electrified vehicles using **FASTSim (Future Automotive Systems Technology Simulator)**, developed by the National Renewable Energy Laboratory (NREL).

## 📌 Project Objective
To analyze energy flow distribution and energy recovery potential (regenerative braking) of a hybrid vehicle during standardized driving cycles (EPA UDDS).

## 💎 The Digital Twin Concept in this Study
Unlike a simple statistical model, this project implements a **Digital Twin** of a Hybrid Electric Vehicle (HEV) using the FASTSim-3 engine.

### What makes this a Digital Twin?
* **High-Fidelity Physical Modeling**: The simulation doesn't just estimate consumption; it models the physical interaction between the powertrain, battery chemistry, and external road loads (drag and rolling resistance) in real-time steps.
* **Dynamic Feedback Loop**: It replicates the vehicle's "brain" (Control Logic), deciding when to use the electric motor or the internal combustion engine based on the State of Charge (SOC) and driver demand.
* **Predictive Power**: This virtual replica allows for "What-if" scenarios, such as testing the impact of a smaller battery or a different driving cycle, with engineering-grade precision before any physical prototype is built.
* **FastSim-3 (Rust Engine)**: The use of the f3 core allows the twin to run simulations thousands of times faster than real-time, enabling rapid optimization of energy management strategies.

## 🛠️ Technologies Used
* **FASTSim-3**: High-performance simulation engine powered by Rust and Python.
* **Google Colab**: Cloud environment for data analysis and simulation.
* **Matplotlib/Seaborn**: Visualization of power flows and battery State of Charge (SOC).

## 📊 Key Analysis Points
1. **Fuel Converter Efficiency**: Analysis of thermal losses and chemical energy consumption.
2. **Regenerative Braking System**: Quantification of energy returned to the battery during deceleration.
3. **Road Loads**: Impact of aerodynamic drag and tire rolling resistance on total energy demand.
4. **State of Charge (SOC)**: Monitoring battery behavior and energy buffering during urban driving.

## 🚀 How to Run the Study
You can run the full simulation directly in your browser:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/172hh0eWJTsfl8z_79xZAPO8WzonAvxYK?usp=sharing)

## 📈 Expected Results
The study demonstrates how electrification—even in Mild Hybrid (MHEV) systems—reduces energy waste at the brakes, optimizing overall fuel consumption in urban cycles by recovering kinetic energy.

---
**Author:** José Sávyo  
**Tool:** FASTSim (National Renewable Energy Laboratory - NREL)
