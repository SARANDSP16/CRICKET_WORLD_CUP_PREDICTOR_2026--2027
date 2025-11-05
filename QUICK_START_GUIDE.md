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
- Connects to **CricketData.org API** (your key: `c1dde435-6493-44bb-bffc-443acf030eb0`)
- Connects to **Cricbuzz RapidAPI** (your key: `20bfa73fd3msh835e15064a3f2d2p19c716jsn57009bf1a217`)
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

## 🎯 Key Differences from Original Project

### ✅ What Changed

| Original | Unified Notebook |
|----------|------------------|
| 5 separate notebooks | 1 complete notebook |
| Manual API key entry | Pre-configured keys |
| Run notebooks sequentially | Run all at once |
| Cloudflare deployment | Power BI deployment |
| Complex setup | Simple execution |

### ✅ What's the Same

| Feature | Status |
|---------|--------|
| Data collection APIs | ✅ Identical |
| Machine learning models | ✅ Same algorithms |
| Feature engineering | ✅ All features included |
| Predictions accuracy | ✅ Same methodology |
| Database structure | ✅ Unchanged |

---

## 🔑 Your API Keys (Pre-configured)

### CricketData.org API
```
API Key: c1dde435-6493-44bb-bffc-443acf030eb0
Free Tier: 100 requests/day
Status: Already configured in notebook
```

### Cricbuzz RapidAPI
```
API Key: 20bfa73fd3msh835e15064a3f2d2p19c716jsn57009bf1a217
Free Tier: 100 requests/day
Status: Already configured in notebook
```

**You don't need to do anything - keys are hardcoded in Section 2!**

---

## 🐛 Troubleshooting

### Issue: "Module not found"
```bash
pip install -r requirements.txt
```

### Issue: "API key invalid"
Your keys are valid until the free tier limit is reached. The notebook will automatically fall back to web scraping.

### Issue: "Database locked"
Close any other programs accessing the database file.

### Issue: "Notebook won't run"
Ensure you have Python 3.8+ and at least 4GB RAM.

### Issue: "Power BI can't import CSV"
Check that the `powerbi/` folder exists and contains CSV files after running the notebook.

---

## 💡 Pro Tips

### 1. Customize Player List
Edit **Section 3** to add more players:
```python
sample_players = [
    ('Player Name', 'India', 'Role', 'Batting', 'Bowling', 'DOB'),
    # Add your players here
]
```

### 2. Adjust Prediction Weights
Edit **Section 4** to change feature importance:
```python
df['performance_score'] = (
    df['batting_avg'] * 0.3 +    # Change this
    df['strike_rate'] * 0.2 +    # And this
    # ...
)
```

### 3. Change Tournament Simulation
Edit **Section 6** to adjust Monte Carlo parameters:
```python
simulate_tournament(squad_strength, n_simulations=10000)  # Change count
```

### 4. Update Data Regularly
Re-run the notebook weekly/monthly to refresh predictions with latest stats.

---

## 📈 Expected Results

### Typical Output:
- **T20 Win Probability:** 30-45%
- **ODI Win Probability:** 35-50%
- **Squad Size:** 15 players each
- **Veterans (38+):** 2-4 players
- **High Retirement Risk:** 1-2 players

### Execution Time:
- **Fast:** 2-3 minutes (without downloading large datasets)
- **Slow:** 5-10 minutes (with full Cricsheet downloads)

---

## 🎓 Understanding the Predictions

### Selection Probability (0-1)
- **0.8-1.0:** Very likely to be selected
- **0.6-0.8:** Good chance
- **0.4-0.6:** Moderate chance
- **0.0-0.4:** Low chance

### Performance Score (0-100)
- **80-100:** World-class
- **60-80:** Very good
- **40-60:** Average
- **0-40:** Below average

### Retirement Risk (0-1)
- **0.0-0.3:** Low risk (young players)
- **0.3-0.6:** Moderate risk
- **0.6-0.8:** High risk (veterans)
- **0.8-1.0:** Very high risk (likely retirement)

---

## 🚀 Next Steps After Running

### Immediate (Today):
1. ✅ Run the complete notebook
2. ✅ Check `powerbi/` folder for exports
3. ✅ Open Power BI and import CSV files
4. ✅ Create your first dashboard

### Short-term (This Week):
1. 🔄 Customize player list
2. 🔄 Adjust prediction parameters
3. 🔄 Add more visualizations
4. 🔄 Share dashboard with friends

### Long-term (This Month):
1. 📊 Download full Cricsheet datasets
2. 📊 Add IPL data
3. 📊 Include injury news
4. 📊 Automate weekly updates

---

## 📞 Support

### If you encounter issues:
1. Read the error message carefully
2. Check the troubleshooting section above
3. Verify Python version and dependencies
4. Ensure API keys haven't exceeded free tier limits

### For Power BI help:
1. Open `POWER_BI_SETUP_GUIDE.txt` in powerbi folder
2. Follow step-by-step instructions
3. Use provided DAX formulas
4. Apply recommended color schemes

---

## 🎉 Summary

**What you have:**
- ✅ Single notebook with all functionality
- ✅ Pre-configured API keys
- ✅ Power BI export ready
- ✅ Comprehensive documentation

**What you need to do:**
1. Run the notebook (one click)
2. Import CSV files to Power BI
3. Create your dashboard
4. Done! 🎊

---

## 📄 Files Included

- `Cricket_Predictor_Complete.ipynb` ← **Main notebook (THIS ONE)**
- `requirements.txt` ← Dependencies
- `QUICK_START_GUIDE.md` ← This file
- Original project files (for reference)

---

## ⏱️ Time Estimates

| Task | Time Required |
|------|---------------|
| Install dependencies | 2-5 minutes |
| Run complete notebook | 3-5 minutes |
| Import to Power BI | 5-10 minutes |
| Create basic dashboard | 15-30 minutes |
| **Total** | **25-50 minutes** |

---

## 🏆 What You'll Get

**A fully functional cricket prediction system with:**
- 🎯 ML-powered squad predictions
- 📊 Tournament win probabilities
- 👴 Veterans retirement risk analysis
- 📈 Interactive Power BI dashboards
- 🔄 Automated data updates

---

**Built with ❤️ for Cricket Analytics**

*Ready to predict the future of Indian cricket? Let's go! 🚀*

---

**Last Updated:** November 4, 2025  
**Version:** 1.0 - Complete Unified Edition
