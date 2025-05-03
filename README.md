# DATA-ANALYST-TASK-8
Create a basic interactive dashboard that shows sales performance by product, region, and month

# Sales Performance Dashboard

A lightweight Power BI / Tableau‑style dashboard that tracks company‑wide
sales by **product category, region, and time**.  
This repository contains:

| Path | Description |
|------|-------------|
| `/data/` | Raw and cleaned CSV files (not included here – see _Data Source_). |
| `/reports/` | The dashboard file (`sales_performance.pbix` or `.twb`). |
| `/img/` | Static images used in the README. |
| `README.md` | You are here. |

---

## 1. Quick Start

```bash
# Clone the repo
git clone https://github.com/your‑org/sales‑performance.git
cd sales‑performance

# (Optional) create a Python env for data prep
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt

