# Techno-Commercial Feasibility of Climate-Isolated Solar BLDC Refrigeration Solutions

## 📌 Executive Summary
This project evaluates the technical viability and corporate financial feasibility of deploying decentralized, solar-powered Cold-Chain Solutions tailored to micro-climatic variances across developing markets (Baseline: Rural India). 

By integrating a **Google Colab Python Physical Simulation PoC** with an **Accrual-Based Corporate Financial Framework**, this study bridges the gap between hardware engineering constraints and macroeconomic investment feasibility ($NPV$, Payback, and Cash Flow liquidity).

---

## 🛠️ The Tech-Box Solution & Technical Architecture
Traditional AC-induction refrigeration solutions suffer from massive, destructive startup current surges (5x-6x running load), making off-grid solar scaling financially non-viable. 

This project simulates and validates a **Direct DC, Brushless DC (BLDC) Variable Speed Compressor** architecture running on a **500 Wp Solar Array** and a localized **Lithium Iron Phosphate ($LiFePO_4$) battery bank**, entirely eliminating inverter losses and starting surge penalties.

### Repository Folders:
* `/simulation`: Contains the core Python implementation simulating 24-hour battery State of Charge ($SoC$) dynamics under divergent environmental boundaries.
* `/financial_models`: Houses the dynamic 3-Segment financial accounting sheets (Standard, Arid, Rainforest).

---

## 📊 Solution-Based Market Segmentation & Year 1 Financial Matrix

Rather than scaling a single uniform product, our enterprise model utilizes **Climate-Based Solution Segmentation** to guarantee a 0% inventory spoilage rate globally:

| Financial Metrics (Year 1) | Segment 1: Standard | Segment 2: Arid (45°C) | Segment 3: Rainforest (Monsoon) |
| :--- | :--- | :--- | :--- |
| **Technical Pivot** | Base Configuration | Controller Thermal Proofing | Doubled Battery Autonomy (300Ah) |
| **Unit Manufacturing COGS** | ₹68,000 | ₹71,000 | ₹93,000 |
| **Wholesale Selling Price** | ₹85,000 | ₹92,000 | ₹1,15,000 |
| **Gross Margin Generated** | ₹85,00,000 | ₹1,05,00,000 | ₹1,10,00,000 |
| **Net Profit After Tax (PAT)**| ₹30,00,000 | ₹45,00,000 | ₹48,75,000 |
| **Projected Payback Period** | **1.14 Years** | **0.80 Years** | **0.74 Years** |

---

## 💻 Running the Technology PoC Simulation

The physical validation script evaluates the battery storage depletion curve over a 24-hour cycle. It accounts for **Negative Temperature Coefficients** (solar cell degradation at 45°C) and **Cloud-Attenuation Factors** (65% solar irradiance loss under tropical monsoons).

### Quick Start (Google Colab)
1. Open Google Colab.
2. Clone or upload the notebook file located in `/simulation/climate_sensitivity_poc.ipynb`.
3. Run all blocks to render the 24-Hour Battery Survival Curve across standard, desert, and tropical jungle matrices.

### Dependencies
```bash
pip install numpy matplotlib

# Important Notice

This repository contains code published for demonstration and testing purposes only. 
The underlying intellectual property (IP) — including inventions, processes, methods, 
algorithms, and research results — is proprietary and protected under Indian law and 
international treaties (Berne Convention, Paris Convention, TRIPS Agreement).

By accessing this repository, you agree:
- The code may be viewed and studied for non-commercial, educational, or research use only.
- Any reproduction, modification, distribution, or commercialization of the IP is strictly prohibited.
- Enforcement of rights will be pursued under Indian jurisdiction and applicable international treaties.

For licensing inquiries or commercial permissions, please contact:
Abhishek Singh  | UIDAI: 9414 9122 9013
Email: abhishek1033@gmail.com | abhishek.s@live.in
Location: Madhya Pradesh, India
