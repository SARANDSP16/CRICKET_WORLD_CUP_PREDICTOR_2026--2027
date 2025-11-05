# Cricket Predictor 🏏

A comprehensive cricket analytics and prediction system that collects, analyzes, and visualizes cricket match data from multiple sources.

## Features 🌟

- **Multi-Source Data Collection** 
  - Cricbuzz API (live matches)
  - CricketData.org API (historical data)
  - ESPN Cricinfo (rankings & statistics)
  - Cricsheet (ball-by-ball historical data)

- **Data Processing**
  - Match data normalization
  - Player statistics aggregation
  - Team performance analysis
  - SQLite database storage

- **Analysis & Predictions**
  - Match outcome predictions
  - Player performance analysis
  - Team rankings and trends
  - Tournament simulations

## Quick Start 🚀

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/cricket-predictor.git
   cd cricket-predictor
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Set up API keys**
   - Get your RapidAPI key from [Cricbuzz API](https://rapidapi.com/cricketapilive/api/cricbuzz-cricket)
   - Set the environment variable:
     ```bash
     # Windows
     set RAPID_API_KEY=your_key_here
     
     # Unix/Linux/macOS
     export RAPID_API_KEY=your_key_here
     ```

4. **Run the notebooks**
   - Start with `01_Data_Collection_APIs.ipynb`
   - Follow the analysis notebooks in sequence

## Project Structure 📁

```
cricket-predictor/
├── notebooks/              # Jupyter notebooks for analysis
├── data/                   # Data directory
│   ├── raw/               # Raw data downloads
│   └── processed/         # Processed datasets
├── models/                # Trained models
├── powerbi/               # Power BI reports
└── README.md             # Project documentation
```

## Data Sources 📊

1. **Cricbuzz API** (via RapidAPI)
   - Live match scores
   - Recent match data
   - Player statistics

2. **CricketData.org API**
   - Historical match data
   - Player profiles
   - Team statistics

3. **ESPN Cricinfo**
   - Team rankings
   - Tournament data
   - Player rankings

4. **Cricsheet**
   - Ball-by-ball match data
   - Historical ODI/T20/Test matches
   - Detailed match statistics

## Analysis Pipeline 🔄

1. **Data Collection**
   - API integration
   - Web scraping
   - Data validation

2. **Data Processing**
   - Cleaning and normalization
   - Feature engineering
   - Statistics calculation

3. **Analysis & Modeling**
   - Exploratory data analysis
   - Statistical modeling
   - Machine learning predictions

4. **Visualization**
   - Interactive dashboards
   - Performance charts
   - Trend analysis

## Dependencies 📚

- pandas
- numpy
- requests
- beautifulsoup4
- sqlite3
- jupyter

## Contributing 🤝

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License 📝

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments 👏

- Cricket data providers
- Open-source community
- Contributors and users
