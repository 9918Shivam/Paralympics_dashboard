# 🏅 Paralympics Dashboard — Power BI

![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Data](https://img.shields.io/badge/Data-1960–2018-blue?style=for-the-badge)
![Medals](https://img.shields.io/badge/Total%20Medals-15%2C645-orange?style=for-the-badge)
![Countries](https://img.shields.io/badge/Countries-73-green?style=for-the-badge)

An interactive **Power BI dashboard** that explores over five decades of Paralympic Games history — from Rome 1960 to PyeongChang 2018. It surfaces medal trends, country dominance, sport-level breakdowns, and seasonal patterns through rich, filterable visualizations.

---

## 📌 Problem Statement

The Paralympic Games have grown from a small gathering of 400 athletes in 1960 into one of the world's largest sporting events. Yet the depth of that journey — which nations led, which sports drove medals, and how participation evolved — is buried in raw records. This dashboard transforms that raw data into a clear, navigable story:

- **Which countries dominate** the medal table across eras?
- **How has medal volume changed** across Summer and Winter editions?
- **Which sports generate the most medals** and which are niche contributors?
- **How do gold, silver, and bronze** distribute across nations?

Analysts, sports historians, and enthusiasts can slice the data by year, season, country, sport, city, and continent to answer these questions instantly.

---

## 📊 Dashboard Overview

> Built in Power BI Desktop · Source: `Paralympics_Dataset_cleaned.xlsx` · 2,209 records × 18 fields

![Paralympics Dashboard](./screenshot/dashboard_preview.png)

---

## 🔢 Key Metrics (KPI Cards)

| Metric | Value |
|---|---|
| 🏆 Total Medals Awarded | **15,645** |
| 🥇 Gold Medals | **5,838** |
| 🥈 Silver Medals | **5,053** |
| 🥉 Bronze Medals | **4,754** |
| 🌍 Total Countries | **73** |
| ⚽ Total Sports | **35** |
| 📅 Games Editions | **22** |

These headline cards give an at-a-glance summary of the entire Paralympic record before any filters are applied.

---

## 📈 Charts & Visualizations

### 1. 🥧 Ratio of Bronze, Silver and Gold Medals *(Pie / Donut Chart)*
Displays the **proportional split** of medal types across all editions.
- Gold: **37.3%** (5.8K)
- Bronze: **32.3%** (5.1K)
- Silver: **30.4%** (4.8K)

**Insight:** Gold medals are slightly more awarded than Silver or Bronze, reflecting cases where ties or disqualifications cause asymmetric distributions.

---

### 2. 📊 Gold, Silver and Bronze Medals by Country *(Clustered Bar Chart)*
Stacked bars show each nation's **medal composition** — how much of their haul is gold versus silver versus bronze.

**Top performers:**
- 🇺🇸 United States — largest total, led by gold (1,487 golds)
- 🇩🇪 Germany — strong across all three medal types
- 🇬🇧 United Kingdom — historically dominant, especially in early editions
- 🇨🇳 China — rapid rise post-1984, now a top-4 nation
- 🇨🇦 Canada — consistent across Summer and Winter both

**Insight:** The US leads by a significant margin, but Germany and Great Britain challenge strongly, reflecting their long participation since the 1960s.

---

### 3. 📉 Total Medals by Games Year *(Line Chart)*
Tracks **medal volume edition by edition** from 1960 to 2018.

**Insight:** There is a clear upward trend from the 1960s through the early 1990s as more countries and sports were added. The line shows characteristic zigzag spikes — peaks at Summer editions and lower counts at Winter editions, which are smaller in scope. Medal counts stabilized post-2000 as the programme became more standardised.

---

### 4. 🌳 Total Medals by Sport *(Treemap)*
Each tile represents a sport; tile size reflects **total medals awarded** in that discipline.

**Dominant sports:**
- 🏃 **Athletics** — largest tile, the backbone of the Summer Games
- 🏊 **Swimming** — second biggest, consistent across all Summer editions
- 🚴 **Cycling**, **Powerlifting**, **Wheelchair sports** — mid-tier contributors
- ⛷️ **Alpine Skiing**, **Cross-country Skiing** — lead the Winter side
- 🏹 **Archery**, **Equestrian** — smaller, niche disciplines

**Insight:** Athletics and Swimming alone account for a disproportionate share of all medals, mirroring the Olympic programme structure.

---

### 5. 🗺️ Total Medals by Country *(Treemap)*
A country-level treemap where tile size maps to **total medal count**, giving an immediate visual sense of hierarchy.

The United States occupies the largest block, followed by Germany, United Kingdom, China, Canada, France, and Australia — all visible as large coloured tiles. Smaller nations appear as tiny slivers, highlighting the **concentration of medals among a handful of nations**.

---

## 🎛️ Interactive Filters (Slicers)

The right-hand panel provides full interactivity — all charts update simultaneously when any filter is changed.

| Slicer | Description |
|---|---|
| **Games Year** (1960–2018) | Drag the range slider to focus on a specific era |
| **Games Season** | Toggle between `Summer` and `Winter` editions |
| **NPC Name** (Country) | Filter all charts to one or more specific nations |
| **Sport** | Isolate a single sport across all time and countries |
| **Games City** | Focus on a specific host city edition |
| **Games Continent** | Regional comparison — e.g., Europe vs Asia |
| **Clear All Slicers** | One-click reset to return to the full dataset view |

---

## 🗂️ Dataset Structure

**File:** `Paralympics_Dataset_cleaned.xlsx`  
**Rows:** 2,209 &nbsp;|&nbsp; **Columns:** 18

| Column | Description |
|---|---|
| `games_code` | Unique edition identifier (e.g., PG1972) |
| `games_year` | Year of the Games (1960–2018) |
| `games_city` | Host city |
| `games_country` | Host country |
| `games_continent` | Host continent |
| `games_start / games_end` | Edition start and end dates |
| `games_season` | Summer or Winter |
| `npc` | National Paralympic Committee code |
| `npc_name` | Full country name |
| `npc_rank` | Overall medal rank for that edition |
| `npc_gold` | Gold medals won |
| `npc_silver` | Silver medals won |
| `npc_bronze` | Bronze medals won |
| `sport_code` | Sport identifier code |
| `sport` | Sport name |

---

## 💡 Key Insights

1. **US dominance is unmatched** — with 1,487 gold medals, the United States has more golds than the next two nations combined.
2. **Summer editions drive volume** — Summer Games award roughly 4–5× more medals than Winter editions due to programme size.
3. **China's rise** — virtually absent before 1984, China broke into the top 4 through rapid Paralympic investment from the 1990s onward.
4. **Athletics & Swimming = ~50% of all medals** — these two sports alone define the medal table for most nations.
5. **Participation expanded sharply post-1980** — the number of competing nations grew steeply after the IOC–IPC cooperation agreement.
6. **Medal distribution is highly concentrated** — a small group of ~10 nations consistently claims the majority of available medals across all editions.

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|---|---|
| **Power BI Desktop** | Dashboard design, DAX measures, interactive slicers |
| **Microsoft Excel** | Data cleaning and preparation |
| **DAX** | Calculated columns and aggregated KPI measures |

---

## 🤝 Contributing

Contributions are welcome! If you have suggestions for new visuals, additional data, or improved DAX measures, feel free to open an issue or submit a pull request.



*Data covers Paralympic Games editions from 1960 (Rome) through 2018 (PyeongChang) — 22 editions across both Summer and Winter Games.*
