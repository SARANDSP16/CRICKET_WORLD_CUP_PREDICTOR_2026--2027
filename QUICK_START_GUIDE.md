# 🏏 Cricket World Cup Predictor - Complete Unified Notebook

## ⚡ Quick Start Guide

### What You Have
✅ **Single Unified Notebook** - All 5 original notebooks merged into one  
✅ **Pre-configured API Keys** - Ready to use immediately  
✅ **Power BI Optimized** - Direct export to Power BI folder  
✅ **One-Click Execution** - Run all cells sequentially  

---

## 🚀 How to Use

### Option 1: Run in Jupyter (Recommended)

```bash
# 1. Navigate to your project folder
cd /path/to/your/project

# 2. Install dependencies
pip install -r requirements.txt

# 3. Launch Jupyter
jupyter notebook

# 4. Open: Cricket_Predictor_Complete.ipynb

# 5. Run all cells: Cell → Run All
```

### Option 2: Run in VS Code

```bash
# 1. Open VS Code
# 2. Install "Jupyter" extension
# 3. Open: Cricket_Predictor_Complete.ipynb
# 4. Click "Run All" button at top
```

### Option 3: Run in Google Colab

```bash
# 1. Upload Cricket_Predictor_Complete.ipynb to Google Drive
# 2. Open with Google Colab
# 3. Runtime → Run all
```

---

## 📊 What This Notebook Does

### 1️⃣ System Check (Section 1)
- Verifies Python version, RAM, CPU
- Creates project directories
- Sets up SQLite database

### 2️⃣ Data Collection (Section 2)
- Connects to **CricketData.org API** (your key: ``)
- Connects to **Cricbuzz RapidAPI** (your key: ``)
- Scrapes **ESPN Cricinfo** for rankings
- Tests all API connections

### 3️⃣ Database Setup (Section 3)
- Creates 5 tables (players, stats, matches, rankings, grounds)
- Loads 15 sample Indian players
- Inserts realistic ODI statistics

### 4️⃣ Feature Engineering (Section 4)
- Calculates 12+ advanced features:
  - Performance score (0-100)
  - Retirement risk (age-based)
  - Fitness score
  - Form (6-month & 12-month)
  - Experience factor

### 5️⃣ Machine Learning (Section 5)
- Trains **Random Forest** classifier
- Trains **XGBoost** classifier
- Shows feature importance
- Saves models to `models/` folder

### 6️⃣ Predictions (Section 6)
- **T20 World Cup 2026 Squad** (15 players)
- **ODI World Cup 2027 Squad** (15 players)
- **Veterans Analysis** (38+ age)
- **Tournament Win Probability** (Monte Carlo simulation - 10,000 runs)

### 7️⃣ Visualizations (Section 7)
- 6 comprehensive charts:
  - Selection probability distribution
  - Age vs Performance
  - Squad composition by role
  - Top 10 players
  - Retirement risk analysis
  - Win probability forecast

### 8️⃣ Power BI Export (Section 8)
- Exports ALL data to `powerbi/` folder
- Creates setup guide: `POWER_BI_SETUP_GUIDE.txt`
- Creates report template: `report_structure.json`
- Ready for immediate Power BI import

### 9️⃣ Summary (Section 9)
- Shows execution summary
- Displays key predictions
- Provides next steps

---

## 📂 Output Files Generated

After running the notebook, you'll have:

```
project/
├── data/
│   ├── cricket_predictor.db          ← SQLite database
│   ├── processed/
│   │   ├── complete_player_analysis.csv
│   │   ├── t20_squad_2026.csv
│   │   ├── odi_squad_2027.csv
│   │   ├── tournament_predictions.csv
│   │   └── comprehensive_analysis.png
│   └── raw/
├── models/
│   ├── random_forest_model.pkl
│   └── xgboost_model.pkl
└── powerbi/                           ← IMPORT THIS TO POWER BI
    ├── POWER_BI_SETUP_GUIDE.txt      ← READ THIS FIRST
    ├── report_structure.json
    ├── complete_player_analysis.csv   ← Main data file
    ├── t20_squad_2026.csv
    ├── odi_squad_2027.csv
    ├── tournament_predictions.csv
    ├── players.csv
    └── player_stats.csv
```

---

## 📊 Power BI Setup (Simple 5-Step Process)

### Step 1: Open Power BI Desktop
Download free: https://powerbi.microsoft.com/desktop/

### Step 2: Get Data
Click **"Get Data"** → **"Text/CSV"**

### Step 3: Import Files
Navigate to your **`powerbi/`** folder and import:
- ✅ `complete_player_analysis.csv` ← **MAIN FILE**
- ✅ `t20_squad_2026.csv`
- ✅ `odi_squad_2027.csv`
- ✅ `tournament_predictions.csv`

### Step 4: Create Visualizations
Open `POWER_BI_SETUP_GUIDE.txt` in the powerbi folder for:
- Recommended dashboard layouts
- DAX formulas (copy-paste ready)
- Color schemes (India team colors)

### Step 5: Design Your Dashboard

**Page 1: Overview**
- Card: Total Players
- Card: Avg Selection Probability
- Gauge: T20 Win Probability
- Gauge: ODI Win Probability
- Bar Chart: Top 15 Players

**Page 2: T20 World Cup 2026**
- Table: Full squad from `t20_squad_2026.csv`
- Treemap: Players by role
- Scatter: Age vs Performance

**Page 3: ODI World Cup 2027**
- Table: Full squad from `odi_squad_2027.csv`
- Bar Chart: Selection probabilities
- KPI: Squad strength

**Page 4: Veterans Analysis**
- Table: Players 38+ by 2027
- Scatter: Retirement risk vs Selection
- Card: High risk count

---

**Built with ❤️ for Cricket Analytics**

*Ready to predict the future of Indian cricket? Let's go! 🚀*

---

**Last Updated:** November 4, 2025  
**Version:** 1.0 - Complete Unified Edition
