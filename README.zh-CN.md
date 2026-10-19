<p align="center"><a href="https://github.com/chengchenwork">English</a> &nbsp; | &nbsp; <strong>中文</strong> &nbsp; | &nbsp; <a href="https://chengchenwork.github.io/data-analysis-portfolio/">交互作品集 ↗</a></p>

<img src="assets/header-bold.svg" width="100%" alt="陈澄 Cheng Chen · 数据分析、统计建模与交互看板" />

<p align="center">
<a href="mailto:cc1053688674@gmail.com"><img src="assets/contact-email-bold.svg" height="36" alt="邮件联系" /></a>
<a href="https://www.linkedin.com/in/cheng-chen-work"><img src="assets/contact-linkedin-bold.svg" height="36" alt="LinkedIn" /></a>
<a href="#精选项目"><img src="assets/contact-projects-bold.svg" height="36" alt="查看项目" /></a>
</p>

### 你好，我是陈澄。把数据整理成可使用的分析工具。

墨尔本大学 **数据科学硕士在读，统计学方向**。我的工作涵盖校园空间分析、电商经营诊断、预算规划与用户行为分析，使用 Python、SQL、统计建模和交互看板支持问题分析与业务讨论。

<img src="assets/companies-bold.svg" width="100%" alt="Apple、得物（POISON Global）、SHEIN、贝卡尔特工作经历" />

<p align="center"><a href="#精选项目">精选项目</a> &nbsp; / &nbsp; <a href="#相关经历">相关经历</a> &nbsp; / &nbsp; <a href="#工具与方法">工具与方法</a> &nbsp; / &nbsp; <a href="#教育背景">教育背景</a></p>

## 精选项目

**[打开交互作品集 ↗](https://chengchenwork.github.io/data-analysis-portfolio/)** — 经营诊断、渠道预算规划与校园空间分析。经营分析演示使用合成数据，界面为中文。校园完整看板为英文。

<img src="assets/project-campus-bold.svg" width="100%" alt="Campus Space Pulse · 336 万条小时记录 · 404 间教室 · 46 栋建筑" />

### Campus Space Pulse：教学空间利用率与规划

**教室很空，是空间过大，还是人数记录偏低？** 为 **336 万条小时记录、404 间教室与 46 栋建筑**构建 Python 数据处理与聚合流水线，连接教室容量、排课计划和教学日历。

`Python` `HTML / CSS / JavaScript` `SVG` `Cloudflare` `交互分析`

**[打开完整英文校园看板 ↗](https://long-sunset-9e69.cc1053688674.workers.dev/#overview)**

<details>
<summary><strong>查看数据处理、指标设计、联动视图与预测探索</strong></summary>

- **数据整合:** 构建用于校园空间分析的数据处理与聚合流水线，整合人数记录、空间容量、排课计划及教学日历。
- **指标设计:** 区分教室利用率、计划班级规模匹配与已排课低人数时段。建筑指标按同一小时合并房间人数与容量，将超过 150% 的利用率读数单独处理，并区分缺失记录与零人数。
- **交互分析:** 开发 5 个联动分析视图，包含校园地图、时段热力图和建筑到教室的下钻。加入学期、教学周与空间类型筛选。
- **预测探索:** 实现本地预测 CSV 导入与校验、教室与周度探索，以及提供实际值后的误差汇总。通过 Cloudflare 部署英文看板，提供可离线使用的资源和可分享的筛选视图。

</details>

<img src="assets/project-fuel-bold.svg" width="100%" alt="澳洲燃油价格与公众舆情分析 · Elasticsearch 数据层与时间对齐检索" />

### 澳洲燃油价格与公众舆情分析

**从价格趋势到可检索的公众讨论。** 设计 **4 类 Elasticsearch 索引**，整合周度燃油价格与 **25,039 条处理后的 Bluesky 记录**，覆盖 2026 年 1–5 月。

2026.04–2026.05  
`Python` `Elasticsearch` `FastAPI` `Kubernetes` `Docker` `Fission` `Jupyter Notebook` `VADER`

<details>
<summary><strong>查看数据层、数据整合与查询校验</strong></summary>

- **数据层:** 为原始及处理后的 Bluesky 帖文、GDELT 新闻和 AIP 燃油价格设计索引，使用字段映射与稳定文档 ID 支持重复导入和更新。
- **整合与检索:** 实现关键词、日期和澳洲相关性筛选，提供主题统计及日度、周度聚合。修复默认日期筛选造成的空结果，校验字段映射、导入和查询，支持 API 与 Notebook 分析。

</details>

<img src="assets/project-credit-bold.svg" width="100%" alt="Lending Club · 125,000 条贷款记录 · 特征工程与跨时间验证" />

### Lending Club 信贷违约预测与特征工程评估

**复杂特征能否改善未来周期的预测？** 处理 **125,000 条贷款记录**并比较特征方案与模型。LightGBM 在 **7,954 条跨时间测试记录**上达到 **0.7339 AUC**，复杂特征仅使其测试 AUC 增加 **0.0005**。

2026.04–2026.05  
`Python` `Pandas` `NumPy` `scikit-learn` `LightGBM` `PyTorch` `特征工程` `Bootstrap`

<details>
<summary><strong>查看泄露防控、特征对比与模型评估</strong></summary>

- **数据与特征:** 剔除泄露字段，完成 CPI 调整、缺失填补和类别编码。使用按时间划分的数据集，比较金融压力、还款能力、信用历史、宏观经济和时间标准化特征。
- **模型评估:** 使用 10 折扩展窗口验证比较 Logistic Regression、LightGBM 与 NODE，并通过 Bootstrap 评估不确定性。在相同特征集下，LightGBM 的跨时间测试 AUC 比 Logistic Regression 约高 0.0199。

</details>

## 相关经历

### 墨尔本大学 · 智慧校园项目

**数据分析与看板开发** · 澳大利亚墨尔本  
2026.03–2026.11（**预计完成**）

Campus Space Pulse 为大学课程项目。我承担的数据流水线、指标设计、交互看板与预测探索工作见[上方项目介绍](#campus-space-pulse教学空间利用率与规划)。

<img src="assets/experience-apple-online.svg" width="100%" alt="Apple · 线上渠道 · 数据分析实习生 · 2026.06–09" />

### Apple · 数据分析实习生 — 线上渠道

**大中华区销售部** · 中国北京  
2026.06–2026.09

**天猫渠道经营分析与 MDF 预算规划** — 围绕经营诊断、历史预测验证与预算规划，支持业务复盘和经销商管理。

<details>
<summary><strong>查看经营诊断、历史验证与预算工具</strong></summary>

- **数据整合:** 整合生意参谋、销售、财务、广告与库存数据，统一日期和商品映射，按日期 × Sub-LOB 组织分析。
- **因子分析:** 围绕需求、转化、利润、库存和竞争构建诊断框架。使用相关性聚类、Sparse Group Lasso 与 Elastic Net 减少冗余，结合 CatBoost + SHAP 解释预测贡献，将库存指标连接到产品排序与风险诊断。
- **预测验证:** 使用 5 折扩展式 walk-forward 验证比较历史基线、Ridge、CatBoost、TimesFM 和残差组合。常规日历史验证排除大促和异常日期，结果用于历史方法比较，不表述为已经实现的业务增量。
- **MDF 规划:** 分析 FY26 Q1–Q3 Marketing Development Fund 计划与实际，区分计划内执行和计划外支出，结合历史执行率与安全垫测算经销商提报需求。开发 Excel 批量校验、汇总和报表输出。
- **看板交付:** 面向负责经销商管理的运营负责人交付经营看板、每日行动工作台与资金视图，提供下钻、Offer 对比及 13 周滚动视图，支持业务复盘和预算讨论。

</details>

<img src="assets/experience-apple-stores.svg" width="100%" alt="Apple · 多门店渠道 · 数据分析实习生 · 2026.01–04" />

### Apple · 数据分析实习生 — 多门店渠道

**大中华区销售部** · 中国北京  
2026.01–2026.04

**乡镇门店分群与人流转化分析** — 在原有周度复盘中加入门店分群与停留时长分析。

<details>
<summary><strong>查看门店分群、停留时长与经营诊断</strong></summary>

- **门店分群:** 将周度复盘从转化率头尾门店排名及门店自述，扩展至基于客流、转化率和深度到访人数的 K-means 分群，支持分群经营分析和差异化营销。
- **停留时长分析:** 将超过 3 分钟的停留定义为深度到访，比较 3–6、7–10、11–14 和 15 分钟以上区间的转化。观察到转化率并未随停留时长持续上升，7–10 分钟区间的观察转化率最高，为客流质量评估和营销策略提供依据。
- **经营诊断:** 通过 Tableau 展示门店分群下的转化率与异常，向门店运营提供分群结果，用于周报和业务复盘。

</details>

<img src="assets/experience-dewu.svg" width="100%" alt="得物（POISON Global）· 商家运营实习生 · 2025.12–2026.01" />

### 得物（POISON Global）· 商家运营实习生

**国际事业部** · 中国上海  
2025.12–2026.01

<details>
<summary><strong>查看商家支持与经营分析</strong></summary>

- **运营支持:** 支持 20 多家商家的商品上架、风控审批、活动提报与保税仓业务。
- **经营分析:** 跟踪商家 GMV 表现与目标进度，分析未达标案例，支持业务复盘和运营判断。

</details>

<img src="assets/experience-shein.svg" width="100%" alt="SHEIN · 数据分析实习生 · 智能平台组 · 2024.10–2025.02" />

### SHEIN · 数据分析实习生

**研发效能架构部 — 智能平台组** · 中国江苏南京  
2024.10–2025.02

<details>
<summary><strong>查看平台使用分析、埋点校验与自助分析支持</strong></summary>

- **使用情况分析:** 使用 SQL 支持跨部门取数，搭建覆盖用户、使用时长和频率的内部平台使用看板，为平台评估和功能优先级提供依据。
- **指标校验:** 校验 FCP、LCP、UV、PV 的事件埋点和指标一致性，识别 FCP 异常波动及潜在数据质量问题，支持监控与排查。
- **平台优化:** 与产品团队协作完善监控平台界面和功能逻辑，加入排除节假日及周末的分析选项，协调跳出率指标和数据导出的前后端优化，支持自助分析。

</details>

<img src="assets/experience-bekaert.svg" width="100%" alt="贝卡尔特 · 实验室 · 数据分析实习生 · 2023.07–08" />

### 贝卡尔特 · 数据分析实习生

**实验室** · 中国江苏无锡  
2023.07–2023.08

<details>
<summary><strong>查看设备数据、异常分析与日报系统</strong></summary>

- **数据清洗:** 了解橡胶混炼流程及生产设备的数据生成机制，使用 Microsoft Access 清洗、整理和结构化原始数据，导出到 Excel 支持分析与报表。
- **异常分析:** 通过 Power BI 构建每日设备数据看板，展示机器运行情况，调查异常模式及可能原因。
- **日报系统:** 使用 HTML、Python 和 CSS 开发 Web 日报系统，自动更新和展示压力、温度、湿度等指标。将日报发布到 SharePoint，方便团队与管理人员访问。

</details>

## 工具与方法

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

- **编程：** Python、R、SQL、Java
- **库与 BI 工具：** Pandas、NumPy、scikit-learn、PyTorch、Tableau、Power BI、Matplotlib、Seaborn、Excel
- **核心能力：** 数据清洗、统计建模、机器学习、特征工程
- **模型与评估：** Elastic Net、Sparse Group Lasso、CatBoost、LightGBM、TimesFM、时间序列交叉验证、Bootstrap、SHAP
- **数据库：** MySQL、Hive、Elasticsearch
- **环境：** Docker、Kubernetes、Linux
- **语言：** 普通话（母语）、英语（熟练）

## 教育背景

🎓 **墨尔本大学｜数据科学硕士 — 统计学方向**  
2025.03–2026.12 · 澳大利亚墨尔本

🎓 **曼尼托巴大学**  
经济学文学学士（辅修数学）与数学文学学士（辅修统计学）  
2019.01–2024.06 · 加拿大温尼伯  
**奖项：** 优秀国际学生奖学金（Outstanding International Student Scholarship）

<a href="mailto:cc1053688674@gmail.com"><img src="assets/footer-bold.svg" width="100%" alt="联系陈澄 · cc1053688674@gmail.com" /></a>

<p align="center"><sub>数据分析 · 统计建模 · 交互看板 &nbsp; / &nbsp; <a href="https://www.linkedin.com/in/cheng-chen-work">LinkedIn ↗</a></sub></p>
