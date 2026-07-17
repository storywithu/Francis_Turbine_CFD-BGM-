# Project: Performance Analysis of Francis Turbine (Steady-state RANS)

### A. System Geometry & Boundary Conditions ### 
![Geometry]<img width="1000" height="600" alt="image" src="https://github.com/user-attachments/assets/5b9000ba-162b-4141-a5d1-881439c7ec48" />
### B. Mesh Configuration & Quality (Overall Score: 0.670)### 
![Geometry]<img width="1000" height="600" alt="image" src="https://github.com/user-attachments/assets/eb0b88f2-280f-43e7-b781-e1eb1d6838c1" />
### C. Flow Dynamics Result ### 
![Geometry]<img width="1000" height="600" alt="image" src="https://github.com/user-attachments/assets/ca820a7f-db5a-4a70-8eb6-5ce149fe61c3" />

---

### 1. Project Overview
- **Objective**: Evaluation of hydraulic performance and internal flow characteristics (Runner efficiency, pressure distribution).
- **Methodology**: Steady-state RANS (Reynolds-Averaged Navier-Stokes) simulation using the MRF(Moving Reference Frame) approach to focus on power extraction efficiency and flow field visualization.
- **Project Period**: 2019.Aug ~ 2019.Aug
- **Repository Note**: This project documentation was archived in 2026.

---

### 2. Simulation Environment & Setup
- **Platform**: SimScale (Cloud-based CFD)
- **Analysis Type**: Incompressible, Steady-state (MRF approach)
- **Turbulence Model**: k-omega SST (Selected for superior prediction of adverse pressure gradients and flow separation)
- **Working Fluid**: Water (Liquid, 20°C)
- **Boundary Conditions**: 
  - Inlet: Velocity inlet (7.273 m/s, Design Point)
  - Outlet: Pressure outlet (0 Pa gauge)
- **Geometry Specs**: Runner Diameter = 0.108 m / Runner Cavity Volume Diameter = 0.132 m
- **Rotation Speed**: 250 rad/s (MRF Domain)
- **Mesh**: Automated mesh with local refinement at blade surfaces (Overall Mesh Quality Score: 0.670!)

---

### 3. Engineering Insights & Critical Reflection
- **Hydraulic Performance**: Successfully predicted the torque and power output characteristics under steady-state operating conditions.
- **Flow Visualization**: Pressure distribution on the runner blades identified potential cavitation zones and areas of flow separation.
- **Critical Reflection**:
  - **Methodological Limitation**: The current MRF (Moving Reference Frame) approach provides a time-averaged performance metric but inherently fails to capture transient Rotor-Stator Interaction (RSI).
  - **Future Advancement**: To analyze off-design performance and pressure pulsations, a transient Sliding Mesh simulation is required for higher-fidelity results.
