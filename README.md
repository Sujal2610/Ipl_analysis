
# IPL Analytics Project

This project analyzes Indian Premier League (IPL) data from 2008 to 2024 using Python and Pandas. It extracts rich insights on team performance, player statistics, match trends, and much more.

#Dataset
The project uses two datasets:
- `matches.csv` – Match-level data from 2008–2024
- `deliveries.csv` – Ball-by-ball data for each match

# GitHub File Size Limit
The `deliveries.csv` file exceeds GitHub's 25MB file limit. Therefore, it is uploaded in compressed format:
Files included in this repository:
- `deliveries.csv.zip`
- `matches.csv`


#To load the zipped CSV in python ,use the following snippet in your notebook or script to read `deliveries.csv` from the zip:

```python
import pandas as pd
import zipfile

with zipfile.ZipFile('deliveries.csv.zip') as z:
    with z.open('deliveries.csv') as f:
        deliveries = pd.read_csv(f)
```

##  Features & Analyses

#Match & Team Insights
- Most successful teams by season and overall (2008–2024)
- Win margins by runs and wickets
- Toss decision impact

#Player Analytics
- Top batsmen by total runs and strike rate (min. 200 balls faced)
- Best bowlers by economy rate (min. 300 balls bowled)

#Strategy Trends
- Batting first vs chasing: season-wise win trends
- Venue popularity: top 10 most frequent stadiums

---

## Tech Stack
- Python 3
- Pandas
- Matplotlib & Seaborn (for visualizations)
- Jupyter Notebook


# Acknowledgment
Dataset sourced from [Kaggle – IPL Dataset](https://www.kaggle.com/datasets)
