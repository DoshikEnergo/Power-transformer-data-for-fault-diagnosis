# ⚡ Intelligent System for Predictive Diagnostics of Power Transformers based on DGA

An end-to-end Machine Learning pipeline developed to automate Dissolved Gas Analysis (DGA) and predict faults in power transformers. This project bridges physics-driven domain expertise with modern object-oriented Data Science practices, increasing diagnostic accuracy from a traditional **47% baseline to 92%**.

---

## 📋 Project Overview

In power engineering, monitoring dissolved gases in transformer oil is critical for preventing catastrophic failures and optimizing maintenance. Traditional analytical frameworks (like the Duval Triangle, Key Gas Method, or Rogers Ratios) face strict limitations on real-world, unbalanced data due to rigid geometric boundaries and ambiguous "gray zones".

This project implements a robust **Scikit-Learn Pipeline** combined with **CatBoost** to automatically generate physical features and classify 7 transformer states simultaneously:
*   **NF** (Normal Functioning / No Fault)
*   **PD** (Partial Discharges)
*   **D1** (Discharges of Low Energy)
*   **D2** (Discharges of High Energy)
*   **T1** (Thermal Fault, $T < 300^\circ\text{C}$)
*   **T2** (Thermal Fault, $300^\circ\text{C} < T < 700^\circ\text{C}$)
*   **T3** (Thermal Fault, $T > 700^\circ\text{C}$)

---

## 🛠 Project Architecture & Engineering Pipeline

Instead of flat model training, the solution is designed as an isolated, production-ready OOP pipeline. This structure fully prevents **Data Leakage** during cross-validation and simplifies commercial deployment.
