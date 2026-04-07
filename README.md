# Composite Naval Console: FEM Analysis & Weight Optimization ⛵📊

![FEM Simulation](images/abaqus_screenshot.png)
*Caption: Abaqus FEA setup: stress distribution and modal shape evaluation on the composite layup.*

## 📌 Project Overview
This repository outlines the configuration and evaluation of a structural Finite Element Analysis (FEA) performed on a composite naval console. The objective was to evaluate weight reduction strategies while maintaining static structural integrity and monitoring vibrational constraints.

**Key Activities:**
* Configured a FEM environment in **Abaqus** to simulate composite material layups under operational loads.
* Evaluated static load requirements, successfully identifying a lighter structural configuration.
* Performed modal analysis (NVH) to extract natural frequencies and mode shapes, comparing them against marine engine excitation ranges.

---

## 🛠️ Tech Stack & Tools
* **Simulation & FEA:** Abaqus
* **Materials:** Composite laminates (Layup configuration)
* **Analysis Types:** Static Structural, Modal (Frequency extraction)

---

## 💡 Engineering Evaluation & Trade-offs
The structural analysis highlighted a classic engineering trade-off between mass and stiffness. While the proposed weight reduction was statically viable, the modal analysis revealed that the reduced global stiffness caused one of the higher natural frequencies to fall within the restricted **70-85 Hz excitation range**. 

Addressing this resonance in a physical prototype would require localized layup re-orientation or targeted ribbing on the specific resonating panel. This approach ensures the frequency is shifted out of the critical range by locally increasing stiffness, without adding unnecessary global weight to the structure.
