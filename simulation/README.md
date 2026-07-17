# 🔬 Technology Proof-of-Concept (PoC) & Thermodynamic Simulation

This directory contains the computational engine used to validate the physical survival of the off-grid solar refrigeration unit before committing capital expenditure (CapEx).

## 📊 Core Engineering Equations Modeled

### 1. Temperature-Induced Solar Degradation
Solar PV panels lose efficiency as their cell operating temperature rises. This script implements a linear power degradation coefficient:

$$P_{actual} = P_{Wp} \times \left[1 - \gamma \times (T_{cell} - 25^\circ\text{C})\right]$$

Where:
* $P_{Wp}$ = Peak Rated Watts (500 Wp)
* $\gamma$ = Temperature coefficient of crystalline silicon (modeled at $0.4\%/^\circ\text{C}$)
* $T_{cell}$ = Core cell temperature (exceeds $70^\circ\text{C}$ in Arid regions)

### 2. Micro-Climatic Cloud Attenuation
To model rainforest monsoons, a multi-scattering diffuse light factor ($\alpha$) is applied directly to the historical clear-sky solar irradiance vector ($G$):

$$G_{attenuated} = G_{baseline} \times \alpha$$

## 🚀 How to Run the Notebook
1. Open [Google Colab](https://colab.research.google.com).
2. Click `Upload` and select `climate_sensitivity_poc.ipynb`.
3. Execute all code blocks (`Ctrl + F9`) to view the interactive 24-hour battery State-of-Charge (SoC) profiles.
