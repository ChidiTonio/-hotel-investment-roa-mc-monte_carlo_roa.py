# -hotel-investment-roa-mc-monte_carlo_roa.py
This repository implements the Monte Carlo + Real Options model from the journal article 'Phased Capital Allocation under Tight Budget–Time Constraints'. Designed for reproducibility and extension."
# Phased Capital Allocation under Tight Budget–Time Constraints  
### A Real Options and Monte Carlo Approach to Hospitality Investment Appraisal  

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)  
[![Python 3.8+](https://img.shields.io/badge/Python-3.8%2B-blue)](https://www.python.org)  

This repository contains the **reproducible computational model** supporting the academic article:  
> *“Phased Capital Allocation under Tight Budget–Time Constraints: A Real Options and Monte Carlo Approach to Hospitality Investment Appraisal”*  
> — submitted to *Research in International Business and Finance* (Q2, Scopus).

The model integrates **real options analysis (ROA)** and **Monte Carlo simulation** to value strategic flexibility in capital-constrained projects — demonstrated via a real-world case of a £1M, 24-week luxury hotel conversion in the Channel Islands.


## Purpose

To provide a transparent, open-source implementation of a hybrid finance methodology that:  
✅ Quantifies the value of *phased implementation* under hard budget/time limits  
✅ Moves beyond static DCF by embedding flexibility as a financial option  
✅ Uses only freely available tools (Python, NumPy, SciPy) — no proprietary software  
✅ Supports teaching, replication, and extension by researchers and practitioners  

This work aligns with open scholarship principles and the *FAIR data guidelines* (Findable, Accessible, Interoperable, Reusable).

---

## 📂 Repository Structure
├── monte_carlo_roa.py          # Main simulation script (fully commented)
├── README.md                   # This file
├── LICENSE                     # MIT License
└── figures/                    # (Optional) Output figures (e.g., histogram, tornado plot)

---

## ⚙️ How to Run

### Option 1: Google Colab (No installation needed)
1. Open [Google Colab](https://colab.research.google.com)  
2. `File → New notebook`  
3. Copy-paste the contents of [`monte_carlo_roa.py`](monte_carlo_roa.py)  
4. Click `Runtime → Run all`  
→ Output includes:  
   - Summary statistics (mean NPV, option value, success probability)  
   - Distribution histogram of total project value  
   - Tornado plot for sensitivity analysis  

### Option 2: Local Python Environment
```bash
# 1. Clone this repository
git clone https://github.com/your-username/hotel-investment-roa-mc.git
cd hotel-investment-roa-mc

# 2. Create and activate a virtual environment (recommended)
python -m venv venv
source venv/bin/activate   # Linux/Mac
# venv\Scripts\activate   # Windows

# 3. Install dependencies
pip install numpy pandas matplotlib scipy

# 4. Run the simulation
python monte_carlo_roa.py

Tested on: Python 3.8, 3.9, 3.10, 3.11
Runtime: ~45 seconds for 10,000 simulations (standard laptop) 
 How to Cite 

If you use this code in your research, please cite the associated article: 

    [Nzomiwu Anthony Chidi]. (2025). Phased Capital Allocation under Tight Budget–Time Constraints: A Real Options and Monte Carlo Approach to Hospitality Investment Appraisal. Research in International Business and Finance, under review. 
** BibTeX entry**: 
bibtex
@article{yourname2025phased,
  title={Phased Capital Allocation under Tight Budget--Time Constraints: A Real Options and Monte Carlo Approach to Hospitality Investment Appraisal},
  author={Nzomiwu A. C.},
  Target journal={Research in International Business and Finance},
  year={2025},
  note={Under review}
}
