Indian Tourism Dashboard | Power BI

Interactive Power BI dashboard summarizing tourism in India across 110 rows  with KPI cards, region/state/category views and airport and railway connectivity.

## 📖 Overview

Built on `Expanded_Indian_Travel_Dataset` (**110 records**, 8 columns: Destination Name, State, Region, Category, Popular Attraction, Accessibility, Nearest Airport, Nearest Railway Station).

## 📊 KPI Cards (Executive Overview)

| KPI | Value | DAX Measure |
|---|---|---|
| Total Destinations | **110** | `COUNT(Dataset[Destination Name])` |
| Total States | **14** | `DISTINCTCOUNT(Dataset[State])` |
| Total Regions | **4** | `DISTINCTCOUNT(Dataset[Region])` |
| Total Categories | **5** | `DISTINCTCOUNT(Dataset[Category])` |
| Total Airports | **19** | `DISTINCTCOUNT(Dataset[Nearest Airport])` |
| Total Railway Stations | **20** | `DISTINCTCOUNT(Dataset[Nearest Railway Station])` |

Other measures: `total attraction` (distinct Popular Attractions) and `Destination %` (share of all destination records).

## 📈 Charts

| Visual | What it shows |
|---|---|
| **Clustered column chart** | Destinations by State / Region / Category, switched by the **"Explore by"** slicer (field parameter) |
| **Donut chart** | Destination share by Region |
| **Treemap** | Destination distribution by Category |
| **Navigation buttons** | Executive Overview • Connectivity Analysis • Deep Dive & Insights • Destination Explorer |

## 💡 Key Insights

- **Regions:** West and East lead with 32 records each (29.1%), then North (24) and South (22).
- **Categories:** Nature (52) and Heritage (43) make up most records; Adventure has 11, while Beach and Religious have only 2 each.
- **States:** Rajasthan has the most records (21), followed by Kerala, Himachal Pradesh and West Bengal (11 each).
- **Accessibility:** 53 records are Moderate, 35 Easy and 22 Difficult. All Adventure records are Difficult.
- **Connectivity:** 19 distinct airports and 20 distinct railway stations serve the destinations.

> **Data note:** the 110 records cover only **20 unique destinations**. Ten destinations (Jaisalmer, Udaipur, Shimla, Munnar, Mysore, Darjeeling, Rishikesh, Cherrapunji, Kaziranga, Ajanta and Ellora) appear 10 times each and the other ten appear once. Counts above are record counts, as the dashboard shows them.

## 🧰 Tools
Power BI Desktop • DAX • Field parameters • Custom visual (Advance Card) • Custom theme and action buttons

## 🚀 How to Use
Download `power-bi/India_Tourism_Dashboard.pbix`, open it in **Power BI Desktop** and use the **Explore by** slicer to switch the chart between State, Region and Category.

## 👩‍💻 Author

**Kashish Tripathi** • 📫 www.linkedin.com/in/kashish-tripathi-1a604525b / kashishtripathi1635@gmail.com
