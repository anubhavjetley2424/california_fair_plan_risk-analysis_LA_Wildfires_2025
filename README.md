![image](https://github.com/user-attachments/assets/68edc040-370d-4fd3-9feb-2c990808e6a9)


# Identifying the most distressed counties in California, that require home insurance policy support and change
- The notebook processes 100k+ structure damage records from 2017-2020 CA wildfires, pivoting by county and damage severity (e.g., Destroyed >50%: highest in Sonoma at 18,719, LA at 7,221, Butte at 3,231). Merges with historical fires (1910-2020) for mean acres burned (e.g., Ventura tops at 60k/7 fires) and count (Butte: 28 fires).
- Adds socioeconomic layers: insurance costs (highest in Riverside ~$2k/year), median income (lowest in rural like Modoc ~$45k), population (LA ~9.8M drives scale), FAIR Plan shifts (LA +20k policies 2019-2024 signals market exit).
## **Key Learnings:

- Damage concentrates in wildland-urban interfaces: Sonoma/Butte show repeated mega-fires (e.g., Camp/Tubbs), amplifying destruction despite lower population.
Fire metrics reveal patterns: High acres/fire (Kings: 49k/1 fire) indicate intense events; frequent small fires (Butte: 233 acres/fire) suggest chronic risk.
- Insurance crisis: FAIR surges (Butte +622%, LA +25%) correlate with fire history, hitting low-income counties hardest (e.g., Trinity: high acres, low income $42k).
- Correlations: Heatmap shows strong ties between destruction and acres burned (r~0.7), weak with income (r~-0.3, poorer areas more vulnerable). Population amplifies total damage but not per-fire intensity.
- Trends: Northern CA (Sonoma, Napa) over-represented in top distress; southern (Ventura, LA) in large burns. FAIR growth +300% statewide implies systemic insurance retreat, exacerbating equity issues.

## **Insights Gained:

- Vulnerability hotspots: Sonoma most distressed (high destruction, FAIR reliance, moderate income ~$88k), signaling need for targeted mitigation.
- Socioeconomic disparity: Low-income rural counties (e.g., Trinity, Modoc) face outsized risk with limited recovery resources, as high FAIR shares indicate uninsurability.
- Policy implications: Acres/fire metric highlights prevention gaps in high-intensity areas; overall, data underscores climate-driven escalation, with 2020s fires dwarfing historical averages.
- Broader: Integration reveals cascading effects—fires drive insurance hikes (up 30% avg from national), FAIR as last resort (now 1%+ of policies), potential for depopulation in at-risk zones.
