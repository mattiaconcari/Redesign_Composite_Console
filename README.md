# Composite Naval Console: FEM Analysis & Weight Optimization ⛵📊

![Combined FEM Analysis](images/FEM_console.png)
*Figure 1: Side-by-side comparison of static stress verification (left, low failure risk) and modal frequency analysis (right, localized resonance at 70.4 Hz) performed on the composite console.*

## 📌 Project Overview
This repository outlines the configuration and evaluation of a structural Finite Element Analysis (FEA) performed on a composite naval console. The objective was to evaluate weight reduction strategies while respecting strict marine engineering standards.

**Design Constraints & Load Cases:**
* **Static Strength:** Maintained the composite failure index (Tsai-Hill criterion) below the critical threshold under maximum operational loads.
* **Global Stiffness:** Verified that maximum nodal displacement did not exceed the strict dimensional tolerances required for onboard instrumentation.
* **Modal Analysis:** Required to keep natural frequencies outside the critical engine excitation range (**2 - 13.2 Hz, 62.5 - 81.4 Hz**) to prevent resonance.

**Key Activities:**
* Configured a FEM environment in **Abaqus** to simulate composite material layups.
* Evaluated static load requirements, successfully achieving a **20% overall weight reduction** while satisfying both strength and displacement criteria.
* Performed modal analysis to extract natural frequencies and mode shapes, critically evaluating the trade-off between mass reduction and dynamic stiffness.

---

## 🛠️ Tech Stack & Tools
* **Simulation & FEA:** Abaqus
* **Materials:** Composite laminates (Layup configuration)
* **Analysis Types:** Static Structural, Modal (Frequency extraction)

---

## 💡 Engineering Evaluation & Trade-offs
The structural analysis highlighted a classic engineering trade-off. While the proposed **20% mass reduction** was statically viable and successfully optimized the console's weight, the modal analysis revealed the consequences of the reduced global stiffness. Specifically, one of the higher natural frequencies shifted and fell within the restricted **62.5-81.4 Hz excitation range** of the marine engine. 

Addressing this localized resonance in a physical prototype would require targeted layup re-orientation or adding specific ribbing on the resonating panel. This approach ensures the frequency is shifted out of the critical range by locally increasing stiffness, without compromising the overall 20% weight savings.
