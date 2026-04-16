# 🚀 Interaction of Cohesive Lunar Regolith with Spacecraft Footpad

### A DEM-Based Study with Cohesion Modeling and DEM–FEA Coupling Exploration

---

## 📌 Overview

This project investigates the interaction between a spacecraft footpad and lunar regolith using the Discrete Element Method (DEM). The study goes beyond conventional granular simulations by incorporating **cohesive behavior of lunar soil**, which plays a critical role in low-gravity environments.

A key focus is placed on understanding how **particle-level interactions influence macroscopic response**, including stress distribution, void fraction evolution, and rotational stability of the lander during impact.

---

## 🎯 Objectives

* Analyze stress distribution and force transmission during lander impact
* Evaluate rotational torque and stability of the spacecraft footpad
* Model **cohesive lunar soil behavior** under vacuum conditions
* Reconstruct realistic regolith characteristics based on literature
* Explore **DEM–FEA coupling** for structural response analysis

---

## ⚙️ Methodology

### DEM Framework

* Simulations performed using **LIGGGHTS**
* Particle-based modeling of lunar regolith
* Hertzian contact model for normal and tangential interactions

### Cohesion Modeling

To replicate the unique behavior of lunar soil:

* Implemented **parallel bond model** between particles
* Simulated formation of **particle clusters (agglomerates)**
* Modeled cohesion arising from
  Van der Waals forces

This approach enables representation of bonded granular media, significantly improving realism compared to non-cohesive DEM simulations.

---

## 🌑 Significance of Cohesion in Lunar Regolith

Unlike terrestrial soils, lunar regolith exhibits strong cohesive effects due to:

* Absence of atmospheric moisture
* Fine particle size distribution
* Dominance of inter-particle attractive forces

The inclusion of bonding mechanics allows simulation of:

* Load-bearing particle clusters
* Resistance to particle separation
* Altered stress propagation pathways

---

## 🔗 DEM–FEA Coupling Exploration

To extend the study toward structural response:

* Initiated integration of DEM with
  Abaqus
* Objective: Capture interaction between regolith and **deformable spacecraft footpad**
* Developed partial workflow for data exchange between DEM and FEA domains

Due to computational resource constraints (restricted HPC access), full-scale coupling could not be completed.
However, this establishes a foundation for future **fully coupled DEM–FEA simulations**.

---

## 🛠️ Tools & Technologies

* **LIGGGHTS** — DEM simulations
* **Abaqus** — Finite Element Analysis (partial integration)
* **ParaView** — Visualization and post-processing
* **OpenFOAM** — (for potential CFD coupling)
* **Python** — Data analysis and scripting

---

## 📊 Simulation Details

### Material Properties

* Density: 3100 kg/m³
* Young’s Modulus: 20 MPa
* Poisson’s Ratio: 0.22
* Coefficient of Restitution: 0.35

### Particle Characteristics

* Size range: 1.5 mm – 10 mm
* Distribution based on lunar soil studies

---

## 📈 Key Insights

* Cohesion significantly alters **stress distribution patterns**
* Bonded particles form clusters that influence **load transfer mechanisms**
* Rotational torque is highly sensitive to soil structure and cohesion
* Void fraction evolves dynamically during impact and settling
* Inclusion of bonding leads to **more realistic representation of lunar regolith behavior**

---

## 🔮 Future Work

* Full-scale **DEM–FEA coupling** for structural deformation analysis
* Advanced cohesive contact models beyond parallel bonding
* Irregular particle modeling using multisphere approaches
* Validation with experimental or mission-based data
* Integration with CFD for dust and plume interaction studies

---

## 📂 Repository Structure

```

── MTP_Presentation.pdf
│
└── README.md
```

---

## 👨‍🔬 Author

**Somdeb Sar**
Dual Degree (B.Tech + M.Tech), Metallurgical Engineering
IIT Bhubaneswar

---

## 📎 Note

This repository currently contains the project presentation.
Code, simulation inputs, and post-processing scripts may be added in future updates.
