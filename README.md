# 🥍 SU Women’s Lacrosse Stats Analysis Using LLMs

This Task-05 analyzes SU Women’s Lacrosse statistics from 2020 to 2025 using data scraping, transformation, feature engineering, large language models (LLMs), and validation with Python.

---

---

## 🧾 Step-by-Step Workflow

### 📥 1. Scrape XML Data (2020–2025)

- **Source**: [Syracuse Women's Lacrosse](https://cuse.com/sports/2013/1/16/WLAX_0116134638)
- **Saved Files**:  
  - `xml_data/2020.xml`  
  - `xml_data/2021.xml`  
  - `...`  
  - `xml_data/2025.xml`

---

### 🔄 2. Convert XML to CSV

- Parsed player stats tables from XML.
- Cleaned and standardized data.
- Saved as:
  - `xml_data/player_stats_2020_from_html.csv`, etc.

---

### 📊 3. Combine CSV Files

- Added a `Year` column to each CSV.
- Merged all into one file:
  - `all_years_combined_player_stats.csv`

---

### 🧠 4. Feature Engineering in `stats.ipynb`

- Cleaned and standardized data types.
- Created derived features:
  - `Total Points = Goals + Assists`
  - `Efficiency = Goals / Shots` (based on SOG%)
- Output:
  - `summary_player_stats.csv`

---

### 🤖 5. LLM Prompt Generation

- Crafted natural language prompts for analysis.
- Examples:
  - "Who had the most assists in 2023?"
  - "Which player had the highest shooting accuracy overall?"
- Saved prompts in:
  - `LLM_Prompts/llm_prompts.txt`



## 🔐 GitHub Privacy Controls

Sensitive files are ignored via `.gitignore`:
```gitignore


```


---

# 📊 Detailed Summary & Insights (2020–2025)

This report summarizes player performance from SU Women’s Lacrosse across six seasons, with insights into scoring, assists, accuracy, efficiency, and improvement. It also includes validation and observations based on LLM-driven analysis.

---

## 🗂️ Dataset Overview

| Years Covered | 2020–2025 |
|---------------|-----------|
| Total Players | ~60–80 per year |
| Key Metrics   | `Goals`, `Assists`, `Turnovers`, `Game Winning Goals`, `SOG%`, `Value Score`, `Total Points` (G + A) |

---

## 📈 Yearly Highlights

### 🟠 2020
- **Top Scorer**: Emily Hawryschuk (39 Goals)
- **Most Efficient**: Molly Carter, Ella Simkins (SOG% = 1.0)
- **Top Playmaker**: Megan Carney (11 Assists)
- **Insight**: Limited offensive activity; few players crossed 10 goals.

### 🟠 2021
- **Top Goal Scorer**: Meaghan Tyrrell (68 Goals)
- **Top Assists**: Meaghan Tyrrell (44 Assists)
- **Top SOG% (Min 10 G)**: Maddy Baxter (0.895)
- **Total Points Leader**: Meaghan Tyrrell (112 Points)
- **Insight**: Tyrrell's breakout season; dominant offense overall.

### 🟠 2022
- **Top Goal Scorer**: Meaghan Tyrrell (78 Goals)
- **Top Assists**: Meaghan Tyrrell (33 Assists)
- **Efficient Finishers**: Rowley, Payton (SOG% = 0.857)
- **Insight**: Continued offensive excellence from Tyrrell.

### 🟠 2023
- **Top Goal Scorer**: Megan Carney (59 Goals)
- **Top Assists**: Emma Ward (56 Assists)
- **Top Accuracy**: Rehder, Caroline & Rowley, Payton (SOG% = 1.0)
- **Insight**: Ward emerges as elite playmaker; efficient finishers underutilized.

### 🟠 2024
- **Top Goal Scorer**: Emma Tyrrell (70 Goals)
- **Top Assists**: Emma Ward (37 Assists)
- **Best All-Rounder**: Olivia Adamson (58G, 25A, SOG% = 0.706)
- **Insight**: Strong year for balanced offense and depth scoring.

### 🟠 2025
- **Top Goal Scorer**: Emma Muchnick (34 Goals)
- **Top Assists**: Emma Ward (46 Assists)
- **Most Efficient Scorer**: Sam DeVito (SOG% = 0.917)
- **Insight**: Ward remains key facilitator; opportunity to increase DeVito’s volume.

---

## 🏆 Overall Top Performers (2020–2025)

| Category               | Player               | Value             |
|------------------------|----------------------|-------------------|
| 🎯 Most Goals (1 Season) | Meaghan Tyrrell (2022) | 78 Goals          |
| 🧠 Most Assists        | Emma Ward (2023)     | 56 Assists        |
| 🔥 Best SOG%           | Sam DeVito (2025)     | 0.917             |
| 📈 Most Improved       | Emma Ward (2020→2025) | +71 Points        |
| 🥇 Highest Total Points| Meaghan Tyrrell (2021)| 112 Points        |
| 💡 Top GameChanger Score | Meaghan Tyrrell (2022) | 206.66            |

---

## 📌 Strategic Insights

### ⚔ Offensive Tactics
- **Emma Ward** is the core playmaker — led assists 3 years.
- **Sam DeVito** has elite efficiency (0.917 SOG%) but needs more attempts.
- **Pairing suggestion**: Ward + DeVito or Muchnick.

### 🛡 Defensive Focus
- High turnover players (e.g., Emma Ward: 41 in 2025) need handling drills.
- Defense improvement = more possessions, fewer costly errors.

### 🌱 Talent Development
- **Olivia Adamson**, **Gracie Britton**, and **Emma Muchnick** show consistent growth.
- **Emma Tyrrell's** peak (70 goals in 2024) needs sustained momentum.

---

## 🤖 LLM Integration

- Prompts generated from `summary_player_stats.csv` using natural language.
- Examples:
  - "Who had the most assists in 2023?"
  - "Which player had the highest shooting accuracy overall?"
- LLM (e.g., ChatGPT) responses validated in `validation.ipynb`.

### ✅ LLM Performance
- Accuracy rate: **>80%**
- Validated via Python code against ground truth.
- ✅ = Match, ❌ = Incorrect year/column/logic

---


```


```
## Author

Lakshmi Peram\
[lperam@syr.edu](mailto\:lperam@syr.edu)

```

