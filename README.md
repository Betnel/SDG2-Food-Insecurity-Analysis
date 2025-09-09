\# SDG2 — Food Insecurity \& Nutritional Gap Analysis



\## 📌 Project Overview

This project applies the \*\*CRISP–DM framework\*\* to analyze global food insecurity using \*\*World Development Indicators (WDI)\*\*.  

The analysis highlights uneven progress, persistent nutrition gaps, and vulnerabilities to inflation shocks, all within the context of \*\*SDG2: Zero Hunger\*\*.



\## 📊 Data

\- Source: \[World Bank — World Development Indicators](https://databank.worldbank.org/source/world-development-indicators)  

\- Indicators used (where available):

&nbsp; - Prevalence of undernourishment (% of population) – `SN.ITK.DEFC.ZS`

&nbsp; - Food Insecurity Experience Scale (moderate/severe, severe) – `SN.ITK.MSFI.ZS`, `SN.ITK.SVFI.ZS`

&nbsp; - Child stunting (% of children under 5) – `SH.STA.STNT.ZS`

&nbsp; - Anemia in women (% of women 15–49) – `SH.ANM.ALLW.ZS`

&nbsp; - Cereal yield (kg/ha) – `AG.YLD.CREL.KG`

&nbsp; - Arable land (% of land area) – `AG.LND.ARBL.ZS`

&nbsp; - GDP per capita (USD) – `NY.GDP.PCAP.CD`

&nbsp; - CPI Inflation (%/yr) – `FP.CPI.TOTL.ZG`

&nbsp; - Population – `SP.POP.TOTL`



\## 🛠 Methodology

The project follows \*\*CRISP–DM\*\* steps:

1\. \*\*Business Understanding\*\* – Frame SDG2 food insecurity challenge.

2\. \*\*Data Understanding\*\* – Collect and inspect WDI indicators.

3\. \*\*Data Preparation\*\* – Clean, reshape to tidy format, select latest ≤2022 values.

4\. \*\*Modeling\*\* – 

&nbsp;  - K-Means clustering (if ≥3 indicators present).

&nbsp;  - Risk-tier fallback (quantile segmentation) if fewer indicators are available.

5\. \*\*Evaluation\*\* – Assess cluster sizes, median profiles, and stress-test inflation shocks (+10% CPI).

6\. \*\*Deployment\*\* – Summarize insights, risks, and recommendations.



\## 🔑 Key Results

\- \*\*Uneven progress\*\*: some countries exceed 30% undernourishment, others are below 5%.

\- \*\*Nutrition ≠ calories\*\*: stunting and anemia persist even in middle-income countries.

\- \*\*Price shocks\*\*: fragile economies are most vulnerable to inflation volatility.



\## ✅ Recommendations

\- \*\*High-risk\*\*: Scale safety nets, child/maternal nutrition, and yield-raising interventions.

\- \*\*Moderate\*\*: Stabilize prices through logistics, storage, and targeted transfers.

\- \*\*Resilient\*\*: Diversify crops, adopt climate-smart agriculture, and share best practices.

\- \*\*Inflation-sensitive\*\*: Strengthen value chains, facilitate trade, and deploy price stabilization tools.



\## 📂 Repository Contents

\- `SDG2 food insecurity .ipynb` → Jupyter Notebook (full CRISP–DM analysis, visuals, clustering/tiers)

\- `SDG2\_Food Insecurity\_Summary.pdf` → 1-page stakeholder-ready PDF summary

\- `README.md` → Project overview and documentation



\## 🚀 How to Use

1\. Clone this repo:

&nbsp;  ```bash

&nbsp; git clone https://github.com/Betnel/SDG2-Food-Insecurity-Analysis.git
   cd SDG2-Food-Insecurity-Analysis



