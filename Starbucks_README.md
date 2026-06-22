# ☕ Starbucks Customer Rewards Analytics Dashboard

An end-to-end data analytics project analyzing Starbucks customer rewards program data — covering customer behavior, offer performance, revenue trends, and global store distribution — culminating in an interactive Power BI dashboard.

![Dashboard Preview](outputs/dashboard.png)

---

## 👤 Author

**Thippavathi Hemanth Kumar**  
Aspiring Data Analyst | Python • SQL • Power BI  
[GitHub](https://github.com/hemanthmikkie/Mikkie)

---

## 📌 Objective

To analyze the Starbucks Customer Rewards Program dataset and extract actionable insights on:
- Customer demographics and spending patterns
- Offer type performance (BOGO, discount, informational)
- Revenue trends over time
- Global store and customer distribution
- Offer completion funnel metrics

---

## 📊 Dashboard KPIs

| Metric | Value |
|--------|-------|
| Total Customers | 17K |
| Total Revenue | 1.78M |
| Total Transactions | 139K |
| Offers Received | 76K |
| Offers Completed | 34K |
| Offer Completion Rate | 0.44 (44%) |

---

## 🗂️ Project Structure

```
Starbucks-Customer-Rewards-Analytics/
│
├── README.md
│
├── data/
│   ├── profile.csv          # 17,000 customer demographics
│   ├── portfolio.csv        # 10 offer types with details
│   ├── transcript.csv       # ⚠️ Not included — download from Kaggle (27MB)
│   ├── starbucks.csv        # Starbucks menu & beverage nutrition data
│   └── directory.csv        # Global Starbucks store locations
│
├── outputs/
│   └── dashboard.png        # Power BI dashboard screenshot
│
└── dashboard/
    └── Starbucks_Customer_Rewards_Analytics_Dashboard.pbix
```

---

## 📁 Datasets Used

### 1. `profile.csv` — Customer Demographics (17,000 rows)
| Column | Description |
|--------|-------------|
| `id` | Unique customer ID |
| `gender` | M / F / O |
| `age` | Customer age |
| `income` | Annual income |
| `became_member_on` | Membership start date |

### 2. `portfolio.csv` — Offer Details (10 offers)
| Column | Description |
|--------|-------------|
| `id` | Offer ID |
| `offer_type` | bogo / discount / informational |
| `reward` | Reward points |
| `difficulty` | Minimum spend to complete offer |
| `duration` | Offer validity in days |
| `channels` | email, mobile, social, web |

### 3. `transcript.csv` — Events Log (306,535 rows)
| Column | Description |
|--------|-------------|
| `person` | Customer ID |
| `event` | transaction / offer received / viewed / completed |
| `value` | Amount spent or offer ID |
| `time` | Hours since campaign start |

### 4. `starbucks.csv` — Menu Data (242 rows)
Beverage categories with nutrition details — calories, fat, sugar, caffeine, and more.

### 5. `directory.csv` — Store Locations (17,000+ rows)
Global store data with city, country, longitude, and latitude for map visualizations.

---

## 📈 Dashboard Visualizations

| Visual | Insight |
|--------|---------|
| **Offer Status Distribution** (donut chart) | Transactions dominate at 45.33%; offer completion at 10.95% |
| **Revenue by Offer Type** (bar chart) | BOGO, discount, and informational each generate ~1.8M revenue |
| **Revenue Trend** (bar chart) | Consistent revenue across all three offer types |
| **Total Revenue by Time** (line chart) | Revenue fluctuates between 10K–20K across 800 campaign hours |
| **Customer Distribution** (map) | Global customer base concentrated in North America and Europe |
| **Gender & Offer Type Slicers** | Dynamic filtering across all visuals |

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|------|---------|
| Python (Pandas, NumPy) | Data cleaning & wrangling |
| Power BI | Interactive dashboard & DAX measures |
| Power Query | Data transformation & merging |
| DAX | KPI calculations (completion rate, total revenue) |
| Git & GitHub | Version control & portfolio hosting |

---

## 💡 Key Insights

- **44% offer completion rate** — over half of received offers go uncompleted, indicating opportunity for better targeting.
- **All three offer types generate equal revenue (~1.8M each)** — suggesting informational offers are as effective as incentive-based ones.
- **Transactions make up 45% of all events** — showing strong organic purchase behavior independent of offers.
- **Revenue peaks across campaign hours** — time-based targeting could further optimize offer delivery.
- **Customer base is globally distributed** — heaviest concentration in North America with a strong European presence.

---

## 🚀 How to Use

1. Clone the repository:
   ```bash
   git clone https://github.com/hemanthmikkie/Mikkie.git
   ```

2. Open the Power BI dashboard:
   - Open `dashboard/Starbucks_Customer_Rewards_Analytics_Dashboard.pbix` in Power BI Desktop
   - Refresh data sources pointing to the `data/` folder

3. Use the **Gender** and **Offer Type** slicers to dynamically filter all visuals.

---

## 📂 Data Source

- **Kaggle:** [Starbucks App Customer Reward Program Data](https://www.kaggle.com/datasets/blacktile/starbucks-app-customer-reward-program-data)
- **Kaggle:** [Starbucks Store Locations](https://www.kaggle.com/datasets/starbucks/store-locations)

> ⚠️ **Note:** `transcript.csv` is not included in this repository due to file size (27MB). Please download it directly from the Kaggle link above and place it in the `data/` folder before running the project.
