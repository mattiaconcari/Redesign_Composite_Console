# Composite Naval Console: FEM Analysis & Weight Optimization ⛵📊

![FEM Simulation](images/abaqus_screenshot.png)
*Abaqus FEA setup: Static strength assessment and modal shape evaluation on the composite layup.*

## 📌 Project Overview
This repository outlines the configuration and evaluation of a structural Finite Element Analysis (FEA) performed on a composite naval console. The objective was to evaluate weight reduction strategies while respecting strict marine engineering standards.

**Design Constraints & Load Cases:**
* **Static Strength:** Maintained the composite failure index (Tsai-Hill criterion) below the critical threshold under maximum operational loads.
* **Global Stiffness:** Verified that maximum nodal displacement did not exceed the strict dimensional tolerances required for onboard instrumentation.
* **Modal Analysis:** Required to keep natural frequencies outside the critical engine excitation range (**2 - 13.2 Hz, 62.5 - 81.4 Hz**) to prevent resonance.

**Key Activities:**
* Configured a FEM environment in **Abaqus** to simulate composite material layups.
* Evaluated static load requirements, successfully identifying a lighter structural configuration that satisfied both strength and displacement criteria.
* Performed modal analysis to extract natural frequencies and mode shapes, critically evaluating the trade-off between mass reduction and dynamic stiffness.

---

## 🛠️ Tech Stack & Tools
* **Simulation & FEA:** Abaqus
* **Materials:** Composite laminates (Layup configuration)
* **Analysis Types:** Static Structural, Modal (Frequency extraction)

---

## 💡 Engineering Evaluation & Trade-offs
The structural analysis highlighted a classic engineering trade-off between mass and stiffness. While the proposed weight reduction was statically viable, the modal analysis revealed that the reduced global stiffness caused one of the higher natural frequencies to fall within the restricted **62.5-81.4 Hz excitation range**. 

Addressing this resonance in a physical prototype would require localized layup re-orientation or targeted ribbing on the specific resonating panel. This approach ensures the frequency is shifted out of the critical range by locally increasing stiffness, without adding unnecessary global weight to the structure.
