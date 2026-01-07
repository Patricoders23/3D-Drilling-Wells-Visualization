# 3D Visualization of Drilling Wells - Campo Sacha

Interactive 3D trajectory analysis and visualization of three directional oil wells from Campo Sacha, Ecuador.


![Python](https://img.shields.io/badge/Python-3.11-blue)
![License](https://img.shields.io/badge/License-MIT-green)
![Status](https://img.shields.io/badge/Status-Production-success)
![Plotly](https://img.shields.io/badge/Plotly-5.18-orange)

---

## Project Overview

This project provides comprehensive 3D visualization and comparative analysis of three directional wells:

- **Well Alpha 1** : 147 survey points, TD = 11,386 ft
- **Well Alpha 2** : 114 survey points, TD = 10,770 ft  
- **Well Alpha 3** : 113 survey points, TD = 10,390 ft

### Features

- Complete 3D well trajectory visualization
- Casing point identification (13 3/8", 9 5/8", 7")
- Key reservoir formations (Hollin Superior and Inferior)
- Interactive exploration with Plotly
- Educational step-by-step Jupyter notebook

---

## Project Structure
```
3D_visualization_Drilling_Wells/
│
├── data/
│   ├── raw/                          # Original survey CSV files
│   │   ├── survey_alfa1_301D.csv
│   │   ├── survey_alfa2_308D.csv
│   │   └── survey_alfa3_200D.csv
│   │
│   └── processed/                    # Generated analysis files
│
├── outputs/
│   └── figures/                      # Generated visualizations
│
├── tres_pozos_3d_simple.ipynb        # Main analysis notebook
├── venv/                             # Virtual environment
├── requirements.txt                  # Python dependencies
└── README.md                         # This file
```

---

## Installation & Setup

### Prerequisites

- Python 3.11 or higher
- Visual Studio Code (recommended)
- Git (optional)

### Quick Start

1. **Clone or download this project**

2. **Open in VS Code**
```powershell
   cd 3D_visualization_Drilling_Wells
   code .
```

3. **Create virtual environment**
```powershell
   py -3.11 -m venv venv
   .\venv\Scripts\Activate.ps1
```

4. **Install dependencies**
```powershell
   python -m pip install --upgrade pip
   pip install -r requirements.txt
```

5. **Open the notebook**
   - Open `tres_pozos_3d_simple.ipynb` in VS Code
   - Select Python kernel (your venv)
   - Run cells sequentially with Shift+Enter

---

## Running the Analysis

### Main Notebook

The analysis is in `tres_pozos_3d_simple.ipynb`. This notebook includes:

- Step-by-step explanations in English and Spanish
- Clear, educational code with extensive comments
- No complex functions - easy to understand
- Interactive 3D visualization generation

Simply open the notebook and execute cells one by one. The notebook will:
1. Load the three well surveys from `data/raw/`
2. Process and validate the data
3. Generate an interactive 3D visualization
4. Save outputs to `outputs/figures/`

---

## What You'll See

### 3D Visualization Elements

**Well Trajectories (Lines):**
- Red: Well Alpha 1 (301D) - Deepest well
- Blue: Well Alpha 2 (308D) - Medium depth
- Green: Well Alpha 3 (200D) - Shallowest well

**Casing Points (Diamonds):**
- Orange: 13 3/8" Surface casing (~2,500 ft)
- Purple: 9 5/8" Intermediate casing (~8,500 ft)
- Brown: 7" Production casing (~10,300 ft)

**Reservoir Formations (Circles):**
- Lime green: Hollin Superior (~10,167 ft)
- Dark green: Hollin Inferior (~10,212 ft)

### Interactive Features

- **Rotate:** Left-click and drag
- **Zoom:** Mouse wheel
- **Pan:** Right-click and drag
- **Show/hide:** Click legend items
- **Details:** Hover over lines and points

---

## Key Results

### Well Statistics

| Well | Total Depth (MD) | TVD | Survey Points |
|------|-----------------|-----|---------------|
| Alpha 1 (301D) | 11,386 ft | 10,089 ft | 147 |
| Alpha 2 (308D) | 10,770 ft | 10,107 ft | 114 |
| Alpha 3 (200D) | 10,390 ft | 10,075 ft | 113 |

All three wells successfully reached the Hollin reservoir formation, demonstrating effective geological modeling and directional drilling execution.

---

## Technical Details

### Data Format

Each survey CSV contains:
- `MD`: Measured Depth (ft)
- `Inc`: Inclination (degrees)
- `Azim`: Azimuth (degrees)
- `TVD`: True Vertical Depth (ft)
- `NS`: North-South displacement (ft)
- `EW`: East-West displacement (ft)

### Coordinate System

- X-axis: North-South displacement
- Y-axis: East-West displacement  
- Z-axis: True Vertical Depth (negative, downward)

All measurements in feet (oilfield standard).

---

## Dependencies
```
pandas>=2.2.0
numpy>=1.26.0
plotly>=5.18.0
scipy>=1.11.0
matplotlib>=3.8.0
seaborn>=0.13.0
openpyxl>=3.1.0
```

---

## For Your Portfolio

This project demonstrates:

- **3D Geospatial Visualization:** Interactive plotting with Plotly
- **Domain Expertise:** Oil & Gas directional drilling knowledge
- **Data Processing:** Survey data cleaning and validation
- **Python Skills:** pandas, numpy, plotly, scipy
- **Documentation:** Clear, professional code and documentation
- **Jupyter Notebooks:** Educational, step-by-step analysis

### Skills Showcased

- Python programming (intermediate/advanced)
- 3D coordinate geometry
- Petroleum engineering fundamentals
- Data visualization best practices
- Technical writing and documentation
- Version control readiness


---

## Data Privacy

All data has been anonymized:
- Well names replaced with Alpha 1, 2, 3
- Operator information removed
- GPS coordinates normalized

Geological and directional data are authentic, providing real-world analysis examples while protecting proprietary information.

---

## Author

**Patricia Garcia**
- Petroleum Engineer → Data Scientist
- AWS Certified Cloud Practitioner
- Specialization: Oil & Gas Analytics


---

## License

MIT License - Educational and portfolio use.

---

## Acknowledgments

Data from directional drilling operations in Ecuador's Oriente Basin. Special thanks to the drilling and directional teams whose expertise made this analysis possible.

---

**Last Updated:** January 2026
**Python Version:** 3.11+
**Status:** Production Ready
