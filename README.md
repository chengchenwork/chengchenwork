<p align="center"><strong>English</strong> &nbsp; | &nbsp; <a href="https://github.com/chengchenwork/chengchenwork/blob/main/README.zh-CN.md">中文</a> &nbsp; | &nbsp; <a href="https://chengchenwork.github.io/data-analysis-portfolio/index.en.html">Interactive portfolio ↗</a></p>

<img src="assets/header-bold-en.svg" width="100%" alt="Cheng Chen · Data analytics, statistical modelling and dashboards" />

<p align="center">
<a href="mailto:cc1053688674@gmail.com"><img src="assets/contact-email-bold.svg" height="36" alt="Email" /></a>
<a href="https://www.linkedin.com/in/cheng-chen-work"><img src="assets/contact-linkedin-bold.svg" height="36" alt="LinkedIn" /></a>
<a href="#selected-projects"><img src="assets/contact-projects-bold.svg" height="36" alt="Projects" /></a>
</p>

### Hi, I'm Cheng Chen. I turn data into usable analytical tools.

I'm studying **Data Science — Statistics Specialization at the University of Melbourne**. My work spans campus space analytics, e-commerce operating diagnostics, budget planning and user behaviour analysis, using Python, SQL, statistical modelling and interactive dashboards.

<img src="assets/companies-bold-en.svg" width="100%" alt="Experience at Apple, POISON Global, SHEIN and Bekaert" />

<p align="center"><a href="#selected-projects">Selected projects</a> &nbsp; / &nbsp; <a href="#experience">Experience</a> &nbsp; / &nbsp; <a href="#tools-and-methods">Tools and methods</a> &nbsp; / &nbsp; <a href="#education">Education</a></p>

## Selected projects

**[Explore my interactive portfolio ↗](https://chengchenwork.github.io/data-analysis-portfolio/index.en.html)** — Case studies in operating diagnostics, channel budget planning and campus space analytics. Business demos use synthetic data and have Chinese interfaces. The full campus dashboard is in English.

<img src="assets/project-campus-bold-en.svg" width="100%" alt="Campus Space Pulse · 3.36 million hourly readings · 404 rooms · 46 buildings" />

### Campus Space Pulse: Teaching-space Utilisation & Planning

**Is a room too large for the planned class, or is the recorded headcount low?** Built a Python processing and aggregation pipeline for **3.36 million hourly readings across 404 rooms and 46 buildings**, connecting room capacity, timetable plans and academic calendars.

`Python` `HTML / CSS / JavaScript` `SVG` `Cloudflare` `Interactive analytics`

**[Open the full English dashboard ↗](https://long-sunset-9e69.cc1053688674.workers.dev/#overview)**

<details>
<summary><strong>My contribution: data, metrics, linked views and forecast exploration</strong></summary>

- **Data integration:** Built the processing and aggregation pipeline for campus space analysis, integrating headcounts, capacity, timetable plans and academic calendars.
- **Metric design:** Distinguished room utilisation, planned class-size fit and low-count booked hours. Aggregated concurrent room counts and capacity for building-level metrics, separated readings above 150% utilisation, and treated missing observations separately from zero counts.
- **Interactive analytics:** Developed 5 linked views with campus maps, temporal heatmaps and building-to-room drill-downs. Added semester, teaching-week and space-category filters.
- **Forecast exploration:** Implemented local prediction CSV import and validation, room/week exploration and error summaries when actuals are supplied. Deployed an English dashboard on Cloudflare, with offline-capable assets and shareable filtered views.

</details>

<img src="assets/project-fuel-bold-en.svg" width="100%" alt="Australian fuel prices and public sentiment · Elasticsearch data layer and time-aligned queries" />

### Australian Fuel Prices & Public Sentiment Analytics

**From price trends to searchable public discussion.** Designed **4 Elasticsearch index types** and integrated weekly fuel prices with **25,039 processed Bluesky records** spanning Jan–May 2026.

Apr–May 2026  
`Python` `Elasticsearch` `FastAPI` `Kubernetes` `Docker` `Fission` `Jupyter Notebook` `VADER`

<details>
<summary><strong>My contribution: data layer, integration and query validation</strong></summary>

- **Data layer:** Designed indices for raw/processed Bluesky posts, GDELT news and AIP fuel prices. Used field mappings and stable document IDs for repeatable imports and updates.
- **Integration and queries:** Implemented keyword, date and Australia-relevance filters, topic statistics and daily/weekly aggregations. Fixed empty results caused by default date filters and validated mappings, imports and queries for API and notebook analysis.

</details>

<img src="assets/project-credit-bold-en.svg" width="100%" alt="Lending Club · 125,000 loan records · Feature engineering and out-of-time validation" />

### Lending Club Default Prediction & Feature Engineering Evaluation

**Do complex features improve predictions in future periods?** Prepared **125,000 loan records** and compared feature sets and models. LightGBM achieved **0.7339 AUC on 7,954 out-of-time test records**. Complex features added only **0.0005** to its test AUC.

Apr–May 2026  
`Python` `Pandas` `NumPy` `scikit-learn` `LightGBM` `PyTorch` `Feature engineering` `Bootstrap`

<details>
<summary><strong>My contribution: leakage control, feature comparison and model evaluation</strong></summary>

- **Data and features:** Removed leakage fields, adjusted for CPI, imputed missing values and encoded categories. Used time-based splits and compared financial stress, repayment capacity, credit history, macroeconomic and time-normalised features.
- **Model evaluation:** Compared Logistic Regression, LightGBM and NODE over 10 expanding-window folds, with bootstrap uncertainty assessment. On the out-of-time test set, LightGBM AUC was about 0.0199 above Logistic Regression using the same feature set.

</details>

## Experience

### University of Melbourne · Smart Campus Project

**Data Analytics & Dashboard Development** · Melbourne, Australia  
Mar–Nov 2026 (**expected completion**)

Campus Space Pulse is a university project. My data pipeline, metric design, interactive dashboard and forecast exploration work is described [above](#campus-space-pulse-teaching-space-utilisation--planning).

<img src="assets/experience-apple-online-en.svg" width="100%" alt="Apple · Online Channels · Data Analyst Intern · Jun–Sep 2026" />

### Apple · Data Analyst Intern — Online Channels

**Greater China Sales Department** · Beijing, China  
Jun–Sep 2026

**Tmall Channel Analytics & MDF Budget Planning** — Connected operating diagnostics, historical forecast validation and budget planning to support business reviews and dealer management.

<details>
<summary><strong>My contribution: operating diagnostics, validation and budget tools</strong></summary>

- **Data integration:** Integrated commerce analytics, sales, finance, advertising and inventory data with consistent date and product mappings at date-by-Sub-LOB granularity.
- **Factor analysis:** Structured demand, conversion, profit, inventory and competition factors. Used correlation clustering, Sparse Group Lasso and Elastic Net to reduce redundancy, and CatBoost + SHAP to explain predictive contributions. Linked inventory metrics to product rankings and risk diagnostics.
- **Forecast validation:** Compared historical baselines, Ridge, CatBoost, TimesFM and residual combinations using 5 expanding walk-forward folds. Regular-day historical validation excluded major promotions and anomalous days. These evaluations are historical comparisons, rather than evidence of realised business impact.
- **MDF planning:** Reviewed FY26 Q1–Q3 Marketing Development Fund plans and actuals, separated planned execution from unplanned spend, and estimated dealer submission requirements using historical execution rates and safety buffers. Built Excel batch validation, consolidation and report outputs.
- **Dashboard delivery:** Delivered operating dashboards, a daily action workbench and funding views for the operations lead overseeing dealers, including drill-downs, offer comparisons and a 13-week rolling view for business reviews and budget discussions.

</details>

<img src="assets/experience-apple-stores-en.svg" width="100%" alt="Apple · Multi-store Channels · Data Analyst Intern · Jan–Apr 2026" />

### Apple · Data Analyst Intern — Multi-store Channels

**Greater China Sales Department** · Beijing, China  
Jan–Apr 2026

**Township Store Segmentation & Foot Traffic Conversion Analysis** — Extended weekly reviews with store segmentation and dwell-time analysis.

<details>
<summary><strong>My contribution: store segmentation, dwell time and operating diagnostics</strong></summary>

- **Store segmentation:** Expanded weekly reviews beyond top/bottom conversion-rate rankings and store-reported explanations. Applied K-means to foot traffic, conversion and deep-visit counts to support segment-level operating analysis and differentiated marketing.
- **Dwell-time analysis:** Defined deep visits as stays over 3 minutes and compared conversion across 3–6, 7–10, 11–14 and 15+ minute bands. Conversion did not consistently rise with duration. The 7–10 minute band had the highest observed conversion, informing traffic-quality assessment and marketing strategy.
- **Operating diagnostics:** Used Tableau to visualise conversion rates and anomalies by store segment, delivering segmented findings to store operations for weekly reports and business reviews.

</details>

<img src="assets/experience-dewu-en.svg" width="100%" alt="POISON Global · Merchant Operations Intern · Dec 2025–Jan 2026" />

### POISON Global · Merchant Operations Intern

**International Business Department** · Shanghai, China  
Dec 2025–Jan 2026

<details>
<summary><strong>My contribution: merchant support and business analysis</strong></summary>

- **Operational support:** Supported 20+ merchants in product listings, risk-control approvals, campaign submissions and bonded warehouse operations.
- **Business analysis:** Tracked merchant GMV performance and target progress, and analysed underperformance cases to support business reviews and operational decisions.

</details>

<img src="assets/experience-shein-en.svg" width="100%" alt="SHEIN · Data Analyst Intern · Intelligent Platform Team · Oct 2024–Feb 2025" />

### SHEIN · Data Analyst Intern

**R&D Productivity Architecture — Intelligent Platform Team** · Nanjing, Jiangsu, China  
Oct 2024–Feb 2025

<details>
<summary><strong>My contribution: platform usage, instrumentation and self-service analytics</strong></summary>

- **Usage analysis:** Used SQL for cross-functional data requests and built internal platform usage dashboards covering users, duration and frequency, supporting platform assessment and feature prioritisation.
- **Metric validation:** Validated event instrumentation and metric consistency for FCP, LCP, UV and PV. Identified unusual FCP fluctuations and potential data-quality issues for monitoring and troubleshooting.
- **Platform optimisation:** Collaborated with product teams on the monitoring platform’s interface and functional logic. Added holiday/weekend exclusion options and coordinated front-end and back-end enhancements for bounce-rate metrics and data exports to support self-service analysis.

</details>

<img src="assets/experience-bekaert-en.svg" width="100%" alt="Bekaert · Laboratory · Data Analyst Intern · Jul–Aug 2023" />

### Bekaert · Data Analyst Intern

**Laboratory** · Wuxi, Jiangsu, China  
Jul–Aug 2023

<details>
<summary><strong>My contribution: equipment data, anomaly analysis and daily reporting</strong></summary>

- **Data cleaning:** Developed an understanding of rubber mixing and production-equipment data generation. Used Microsoft Access to clean, organise and structure raw data, then exported processed data to Excel for analysis and reporting.
- **Anomaly analysis:** Built a daily machine-data dashboard in Power BI, visualised machine operating conditions and investigated abnormal patterns and possible root causes.
- **Daily reporting:** Developed a web-based daily reporting system with HTML, Python and CSS to automatically update and visualise pressure, temperature and humidity. Published daily reports to SharePoint for team and management access.

</details>

## Tools and methods

<p>
<img src="assets/tool-python.svg" height="36" alt="Python" />
<img src="assets/tool-sql.svg" height="36" alt="SQL" />
<img src="assets/tool-excel.svg" height="36" alt="Excel" />
<img src="assets/tool-tableau.svg" height="36" alt="Tableau" />
<img src="assets/tool-powerbi.svg" height="36" alt="Power BI" />
<img src="assets/tool-pandas.svg" height="36" alt="Pandas" />
<img src="assets/tool-sklearn.svg" height="36" alt="scikit-learn" />
<img src="assets/tool-elastic.svg" height="36" alt="Elasticsearch" />
</p>

- **Programming:** Python, R, SQL, Java
- **Libraries and BI:** Pandas, NumPy, scikit-learn, PyTorch, Tableau, Power BI, Matplotlib, Seaborn, Excel
- **Core skills:** Data cleaning, statistical modelling, machine learning, feature engineering
- **Models and evaluation:** Elastic Net, Sparse Group Lasso, CatBoost, LightGBM, TimesFM, time-series cross-validation, bootstrap, SHAP
- **Databases:** MySQL, Hive, Elasticsearch
- **Environment:** Docker, Kubernetes, Linux
- **Languages:** Mandarin (Native), English (Proficient)

## Education

🎓 **University of Melbourne | Master of Data Science — Statistics Specialization**  
Mar 2025–Dec 2026 · Melbourne, Australia

🎓 **University of Manitoba**  
B.A. in Economics, minor in Mathematics & B.A. in Mathematics, minor in Statistics  
Jan 2019–Jun 2024 · Winnipeg, Canada  
**Award:** Outstanding International Student Scholarship

<a href="mailto:cc1053688674@gmail.com"><img src="assets/footer-bold-en.svg" width="100%" alt="Contact Cheng Chen · cc1053688674@gmail.com" /></a>

<p align="center"><sub>Data analytics · Statistical modelling · Interactive dashboards &nbsp; / &nbsp; <a href="https://www.linkedin.com/in/cheng-chen-work">LinkedIn ↗</a></sub></p>
