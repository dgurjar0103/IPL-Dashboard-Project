# 🏏 IPL 2024 Analytics Dashboard — Microsoft Excel

An interactive, data-driven Excel dashboard analyzing IPL 2024 season performance across all 8 teams and 33 top players. Built using Pivot Tables, slicers, and advanced Excel formulas to surface team standings, player stats, match outcomes, and more — all within a single workbook.

---

## 📊 Dashboard Pages

### 1. Team Performance Dashboard
- Total Matches Played, Total Wins, Total Runs Scored, Total Wickets Taken
- Team-wise win comparison (bar chart)
- Runs distribution across teams (pie/bar chart)
- Win type breakdown — **Win by Runs** vs **Win by Wickets**

### 2. Player Performance Dashboard
- Average Strike Rate and Average Economy across all players
- Top run-scorers and wicket-takers (ranked visual)
- Player-level breakdown: Runs, Balls Faced, Strike Rate, Wickets, Economy

---

## 🗂️ Data Model

The workbook follows a **star schema** structure with clearly separated fact and dimension tables:

| Table | Description |
|---|---|
| `fact_match` | Match-level data — teams, venue, winner, win margin, win type |
| `fact_player` | Player-level performance — runs, balls, fours, sixes, wickets, economy |
| `dim_team` | Team IDs and names for all 8 IPL franchises |
| `dim_player` | Player metadata — name, role, team |
| `dim_venue` | Venue names and cities |

---

## 🔑 Key Metrics Tracked

**Batting**
- Total Runs, Balls Faced, Strike Rate
- Fours and Sixes

**Bowling**
- Wickets Taken, Overs Bowled, Runs Conceded, Economy Rate

**Team**
- Matches Played, Wins, Total Runs, Total Wickets
- Win method distribution (by Runs / by Wickets)

---

## ⚙️ Excel Features Used

- **Pivot Tables** — dynamic aggregation across all sheets
- **Pivot Charts** — bar, pie, and column charts linked to pivot data
- **Slicers** — interactive filters for Team, Player, Venue, and Role
- **GETPIVOTDATA** — live formula references from summary tables
- **Conditional Formatting** — highlight top performers and outliers
- **Named Ranges** — clean formula referencing across sheets
- **Data Model** — relational table linking via Power Pivot

---

## 📁 File Structure

```
Project1.xlsx
├── Team Performance Dashboard    # Main visual dashboard (Team)
├── Player Performance Dashboard  # Main visual dashboard (Player)
├── Team Summary                  # Pivot tables: team stats
├── Player Summary                # Pivot tables: player stats
├── fact_match                    # Raw match data
├── fact_player                   # Raw player performance data
├── dim_team                      # Team dimension table
├── dim_player                    # Player dimension table
└── dim_venue                     # Venue dimension table
```

---

## 📌 Teams Covered

| Team | Code |
|---|---|
| Chennai Super Kings | CSK |
| Delhi Capitals | DC |
| Kolkata Knight Riders | KKR |
| Mumbai Indians | MI |
| Punjab Kings | PBKS |
| Rajasthan Royals | RR |
| Royal Challengers Bengaluru | RCB |
| Sunrisers Hyderabad | SRH |

---

## 🚀 How to Use

1. Download and open `Project1.xlsx` in **Microsoft Excel 2016 or later**
2. Navigate to the **Team Performance Dashboard** or **Player Performance Dashboard** tab
3. Use the **slicers** to filter by team, player, or venue
4. All charts and summary cards update dynamically with your selection

> ⚠️ Enable **Editing** and **Content** if prompted when opening the file.

---

## 🛠️ Tools & Technologies

- Microsoft Excel (Pivot Tables, Pivot Charts, Slicers)
- Power Pivot (Data Model & Relationships)
- DAX-style calculated fields

---

## 👤 Author

**Dushyant Gurjar**
B.Tech Computer Science & Engineering — BIT Mesra
📧 dgurjar0103@gmail.com
🔗 [LinkedIn](https://linkedin.com/in/) | [GitHub](https://github.com/)

---

## 📄 License

This project is for educational and portfolio purposes. IPL data used is publicly available.