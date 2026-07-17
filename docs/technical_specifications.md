# ⚙️ Hardware Bills of Materials (BOM) & Engineering Schematics

This document maps out the specific hardware profiles that change dynamically across our three solution segments to maintain a 100% cold-chain reliability guarantee.

## 📋 Comprehensive Bill of Materials Matrix

| Component Head | Segment 1: Standard System | Segment 2: Arid System | Segment 3: Rainforest System |
| :--- | :--- | :--- | :--- |
| **Solar PV Array** | 500 Wp Monocrystalline | 500 Wp Monocrystalline | 500 Wp Monocrystalline |
| **Compressor Technology** | 12V/24V Variable Speed BLDC | 12V/24V Variable Speed BLDC | 12V/24V Variable Speed BLDC |
| **Battery Storage** | 1800 Wh ($LiFePO_4$) | 1800 Wh ($LiFePO_4$) | **3600 Wh ($LiFePO_4$ Double Bank)** |
| **Thermal Insulation** | 60mm Cyclopentane Foam | **80mm High-Density Vacuum Panels** | 60mm Cyclopentane Foam |
| **Ingress & Protection** | IP54 Sheet Enclosure | IP54 Ventilation Guarded | **IP65 Moisture Sealed Junctions** |
| **Thermal Controller** | Standard Duty Fins | **Active Cooling Dual-Fan Heatsink** | Standard Duty Fins |

## 🔌 System Layout & Circuit Logic
Because our setup operates as a **Direct DC Architecture**, we completely eliminate the inverter stage.
[Solar PV Array] ──> [MPPT Charge Controller] ──> [LiFePO4 Battery Bank] ──> [Fuzzy-Logic BLDC Driver] ──> [Compressor Motor]

This direct-current topology eliminates the standard 12% to 15% DC-to-AC conversion loss and prevents high thermal-surge feedback loop failures inside the electronics.
