# MLB Weather Analysis
### How Much Does Weather Actually Affect a Baseball Game?

A 95°F afternoon in Houston. A 38°F night in Cleveland. Both count the same in the standings — but do they play the same? This project tests whether temperature, wind, and altitude actually move the scoreboard across five MLB seasons.

---

## Key Findings

All weather variables combined explain roughly **2% of game-to-game scoring variance**. The other 98% is pitching, lineups, and luck.

| Factor | Effect |
|---|---|
| Altitude — Coors Field | +2.34 runs/game |
| Temperature (+10°F) | +0.42 runs/game |
| Wind direction (out vs in) | +0.33 runs/game |
| Altitude — Excluding Coors | +0.032 runs/game |

Temperature's effect concentrates in **home runs** — the one outcome that depends entirely on whether the ball carries far enough to clear a fence. Two separate tests tried to isolate the temperature signal more cleanly. Neither strengthened it.

---

## What's Inside

- `mlb_weather_analysis.ipynb` — Full analysis with charts, regression, and an interactive over/under tool
- `mlb_2021_2025_weather_games.csv` — Cleaned game-level dataset (10,000+ outdoor games, 2021–2025)

---

## Interactive Widgets

The notebook includes an interactive over/under tool that estimates expected run scoring based on temperature, wind, and ballpark. Widgets require a live Python kernel — they will not display on GitHub.

---

## Data Source

MLB Stats API — Official MLB data, 2021–2025 Regular Seasons

---

## Built With

Python — numpy, pandas, statsmodels, matplotlib, seaborn, scipy, ipywidgets, requests, tqdm

## Here's a chart from this project showing individual contributions to total runs in an MLB game
<img width="1868" height="990" alt="image" src="https://github.com/user-attachments/assets/5b892dec-202c-4583-b9d1-2377fa4929a8" />

