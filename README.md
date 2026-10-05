# IPL_Predivcitive_Analysis

# IPL Match Outcome & Exploratory Data Analysis

A comprehensive exploratory data analysis (EDA) project analyzing Indian Premier League (IPL) match statistics, toss impacts, team performances, and match-winning factors across multiple seasons.

---

## 📌 Project Overview
This project performs in-depth data cleaning, transformation, and exploratory visualization on historical IPL datasets (`matches.csv` and `deliveries.csv`). It uncovers trends regarding toss decisions, venue statistics, team win-loss records, scoring milestones, and boundaries across seasons.

---

## ⚙️ Dataset & Preprocessing

- **Datasets Used**:
  - `matches.csv`: Contains match-level information (teams, toss, venue, winner, player of match, umpires).
  - `deliveries.csv`: Contains ball-by-ball records (batsman, bowler, runs, dismissals).
- **Data Cleaning & Transformations**:
  - Removed sparse columns with excessive null values (e.g., `umpire3`).
  - Imputed missing numerical delivery data with `0` and missing string values with empty strings.
  - Standardized all franchise names across seasons to standard abbreviations (e.g., `Rising Pune Supergiant` & `Rising Pune Supergiants` → `RPS`, `Delhi Daredevils` → `DD`, `Sunrisers Hyderabad` → `SRH`, `Royal Challengers Bangalore` → `RCB`).

---

## 📊 Key Highlights & Findings

1. **Total Matches & Reach**:
   - Total matches analyzed: **636 matches** across **30 venues** and **13 franchises**.
2. **Most Successful Individuals & Teams**:
   - **Chris Gayle (`CH Gayle`)** holds the highest number of *Player of the Match* awards.
   - **Mumbai Indians (`MI`)** leads with the highest number of match wins (92 wins out of 157 matches).
3. **Record Victories**:
   - **Largest win by runs**: **146 runs** (Mumbai Indians vs. Delhi Daredevils, 2017).
   - **Largest win by wickets**: **10 wickets** (Kolkata Knight Riders vs. Gujarat Lions, 2017).
4. **Toss Tendencies**:
   - Overall, teams chose to **field first in 57.08%** of matches, compared to **42.92% choosing to bat first**.
   - **Mumbai Indians** won the highest number of tosses across the tournament's history.
   - Approximately **51% of matches** were won by the team that won the toss.

---


## 📸 Visualizations

### 1. Toss Decisions Across Seasons
Teams increasingly preferred fielding first in later seasons (2016–2017) compared to the initial seasons.

```text
Season-wise breakdown showing the shift from electing to bat first towards chasing/fielding.
```


### 2. Toss Wins per Team
Distribution of toss wins across all IPL franchises:
- **MI**: Highest toss wins (85+)
- **KKR & CSK**: Close contenders following MI



### 3. Total Matches vs. Matches Won
Comparison of overall participation versus actual victories:
- **MI**: 157 matches, 92 wins (Win Rate: ~58.6%)
- **CSK**: 131 matches, 79 wins (Win Rate: ~60.3%)
- **KKR**: 148 matches, 77 wins (Win Rate: ~52.0%)
- **RCB**: 152 matches, 73 wins (Win Rate: ~48.0%)


### 4. Toss Impact on Match Outcome
- **Toss Winner Won Match**: ~50.6%
- **Toss Winner Lost Match**: ~49.4%

Winning the toss provides a slight edge, but execution during the match remains the decisive factor.

---

## 🛠️ Tech Stack & Libraries
- **Language**: Python 3
- **Data Manipulation**: `pandas`, `numpy`
- **Visualization**: `matplotlib`, `seaborn`, `plotly`

---

## 🚀 How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/ipl-predictive-analysis.git
   cd ipl-predictive-analysis
   ```
2. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn plotly
   ```
3. Open and run the Jupyter Notebook:
   ```bash
   jupyter notebook "IPL Project.ipynb"
   ```
