# 🔥 California Wildfire & Insurance Distress Analysis
### Identifying the state's most vulnerable counties needing urgent home insurance policy reform.

# Project Dashboard

![Dashboard Preview](https://github.com/user-attachments/assets/68edc040-370d-4fd3-9feb-2c990808e6a9)

<br>
<br>

<div align="center">
  <img src="https://github.com/user-attachments/assets/95265dca-0c6c-4f63-9569-0328dc0ba2d5" width="48%" style="margin-right: 10px;" />
  <img src="https://github.com/user-attachments/assets/62ba39d1-3fb6-4769-ae67-464743c92223" width="48%" />
</div>



## 📖 Executive Summary
In January 2025, catastrophic wildfires swept through California, exacerbating a growing crisis where climate disaster meets economic vulnerability. This project serves as a comprehensive data analysis of over **100,000 structure damage records**, cross-referencing recent devastation with a century of historical fire data (1910-2020), socioeconomic indicators, and home insurance market shifts. 

The objective is to identify which California counties are the most **"distressed"**—suffering from a deadly combination of high destruction, surging insurance costs, widespread reliance on the FAIR Plan (the state's insurer of last resort), and lower median incomes.

---

## 🔍 Key Discoveries (The "So What?")

### 1️⃣ The Wildland-Urban Interface is Ground Zero
* **Concentrated Destruction:** Sonoma and Butte counties face repeated mega-fires (e.g., the Tubbs and Camp fires). Despite having smaller populations than coastal hubs, Sonoma saw the highest number of severely destroyed structures (>50% damage) at **18,719**, followed by Los Angeles (7,221) and Butte (3,231).
* **Fire Patterns:** High *acres-per-fire* metrics (e.g., Kings County: 49k acres/fire) indicate massive, intense events, while high frequency/lower acreage (Butte: 28 historical fires) suggests chronic, inescapable risk.

### 2️⃣ The Uninsurability Crisis
* **FAIR Plan Explosion:** As private insurers flee, reliance on the FAIR Plan has skyrocketed statewide by +300%. Butte County saw a massive **+622%** increase in FAIR policies, while Los Angeles added over 20,000 policies between 2019 and 2024—a massive signal of standard market exit.
* **The Cost of Risk:** Riverside County now faces some of the highest median property insurance costs (~$2,000/year), directly correlating with recent burn scars and driving up the cost of living.

### 3️⃣ The Socioeconomic Divide
* **Vulnerability & Poverty:** A stark inequity exists. Rural, low-income counties like Trinity and Modoc (median income ~$42k-$45k) face outsized fire risks. When disaster strikes, these communities lack the financial resilience to recover, and their high FAIR Plan shares indicate they are effectively uninsurable in the private market.
* **Population vs. Intensity:** While the massive population in Los Angeles drives the sheer *scale* of total financial damage, the per-capita intensity and economic distress are most acute in Northern California (Sonoma, Napa, Butte).

---

## 💻 The Data Engine (What the Notebook Does)
The included Jupyter Notebook (`Cali_analysis.ipynb`) serves as the analytical engine, combining 7 disparate datasets into a unified distress index. 

**Key Technical Workflows:**
* **Data Fusion:** Merges CAL FIRE structure damage reports, Census population/income data, and California Department of Insurance metrics by County FIPS codes.
* **Statistical Correlation:** Employs Seaborn heatmaps to prove that while destruction and acres burned are highly correlated ($r \approx 0.7$), income has a weak negative correlation ($r \approx -0.3$)—proving poorer areas are disproportionately vulnerable.
* **Geospatial Mapping:** Generates interactive Plotly Choropleth and Density maps to visualize metrics like `Acres_per_fire` and `Fair_Plan_Change` across the state.
* **Feature Engineering:** Pivots 100k+ damage records by severity to create actionable composite scores for distress ranking.

---

## 🚀 Future Enhancements (What's Next?)
To evolve this analysis into a complete tool for policymakers and urban planners, the following dimensions will be added:

* **📉 The Private Insurer Exodus:** Track the specific departure of admitted market carriers (e.g., State Farm, Allstate). Analyzing non-renewal notices and policy drops by county will show exactly *where* the private market is collapsing fastest before those homeowners are forced onto the FAIR Plan.
* **🏗️ Building Codes & Survival Rates:** Correlate the `Year Built` of structures with survival rates to prove the ROI of modern, fire-hardened building codes (WUI codes post-2008).
* **🔮 Predictive Distress Modeling:** Train a machine learning classifier to predict which counties will breach critical "distress thresholds" (uninsurability) by 2030 based on current climate and economic trajectories.

---
*Built to bring data-driven clarity to California's intersection of climate risk and housing policy.*
