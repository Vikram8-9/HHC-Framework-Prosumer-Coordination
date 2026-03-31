# 🌩️ Hybrid Hierarchical Framework: Stochastic MPC & EGT Coordination

[![Status](https://img.shields.io/badge/Research-Official--Release-gold.svg)]()
[![Python](https://img.shields.io/badge/Python-3.9%2B-green.svg)]()
[![GPU](https://img.shields.io/badge/GPU-NVIDIA--RTX--4070-76b900.svg)]()
[![Institution](https://img.shields.io/badge/Southeast--University-Nanjing-blue.svg)]()
 
**"A Hybrid Hierarchical Framework Combining Stochastic MPC and Evolutionary Game Theory for Prosumer Coordination"**

---

## 🏛️ Authorship & Affiliation
* **Vikram Kumar** (Main Author) - `vk2391080@gmail.com`
* **Usama Aslam** - `usamaaslma465@gmail.com`
* **Muhammad Ahsan Niazi** - `ahsanniazi297@gmail.com`

---

## 🔬 Mathematical Architecture (HHC Framework)

### 1️⃣ Upper Layer: Stochastic MPC (VPP Coordination)
Minimization of system-wide costs under probabilistic scenarios $\omega$:
$$\min_{\omega} \mathbb{E} \left[ \sum_{k=t}^{t+T} (Cost_{loss}(k, \omega) + Cost_{deg,tx}(k, \omega) + Cost_{penalty}(k, \omega)) \right]$$

### 2️⃣ Lower Layer: Evolutionary Game Theory (Prosumer Strategy)
Strategies evolve according to the **Replicator Dynamics** principle:
$$x_s(t+1) = x_s(t) \cdot \frac{f(s)}{\sum_{s'} x_{s'}(t) \cdot f(s')}$$

---

## 🗺️ Data Repository Map (IoT Data Lake)
To maintain high-fidelity simulation standards, the data is organized into a **Spatio-Temporal Hierarchy**. This structure manages **268,800+ discrete files**.

```text
📂 Data_Repository/ [268,800 Total Files]
├── 🏠 Prosumer_001/
│   ├── 📅 Day_01/
│   │   ├── ☀️ PV_Generation/    --> [TS_00_00.csv ... TS_23_45.csv] (96 intervals)
│   │   ├── 🔌 Inelastic_Load/   --> [TS_00_00.csv ... TS_23_45.csv] (96 intervals)
│   │   ├── 🚗 EV_Demand/        --> [TS_00_00.csv ... TS_23_45.csv] (96 intervals)
│   │   └── 🔋 Battery_State/    --> [TS_00_00.csv ... TS_23_45.csv] (96 intervals)
│   ├── ... (Days 02 to 06)
│   └── 📅 Day_07/
├── ... (Prosumers 002 to 099)
└── 🏠 Prosumer_100/

Note: Each .csv file represents a discrete 15-minute sensor slice. This atomized architecture is designed for Privacy-Preserving Parallel Processing.

💻 Hardware Environment (HPC Specs)

Model: Dell G16 (7630)

CPU: Intel(R) Core(TM) i9-13900HX (24 Cores)

RAM: 32 GB DDR5 4800MHz

GPU: NVIDIA® GeForce RTX™ 4070 (8GB GDDR6)

Storage: 1 TB NVMe SSD Gen4

Software: Python 3.9, Gurobi 9.5, DEAP Library

🚀 Usage Guide
code
Python
download
content_copy
expand_less
from HHC_Core_Model import HybridHierarchicalControl
# Initialize agent for Prosumer 42
agent = HybridHierarchicalControl("Prosumer_042")
# Load a specific 15-minute interval
slice = agent.load_slice("Day_03", "PV_Generation", "12_00")
📜 Citation (BibTeX)
code
Bibtex
download
content_copy
expand_less
@article{kumar2024hhc,
  title={A Hybrid Hierarchical Framework Combining Stochastic MPC and Evolutionary Game Theory for Prosumer Coordination},
  author={Kumar, Vikram and Aslam, Usama and Niazi, Muhammad Ahsan},
  journal={Southeast University Research Archive},
  year={2024}
}

