# Olist E-Commerce Data Analysis: End-to-End Diagnostic & Predictive Framework

[![Python](https://img.shields.io/badge/Python-3.12+-blue.svg?style=flat&logo=python)](https://www.python.org/)
[![Power BI](https://img.shields.io/badge/Power_BI-Data_Visualization-F2C811?style=flat&logo=powerbi)](https://powerbi.microsoft.com/)
[![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-K--Means_Clustering-F7931E?style=flat&logo=scikit-learn)](https://scikit-learn.org/)
[![Hugging Face](https://img.shields.io/badge/%F0%9F%A4%97-BERTopic_%2B_NLLB--200-FFD21E)](https://huggingface.co/)

This repository delivers an advanced analytics solution engineered for the **Olist e-commerce ecosystem**, encompassing **15.49M BRL in revenue** and over **100k transaction records**. By uniting multi-page **Power BI dashboards** with machine learning (**RFM + K-Means**), natural language processing (**BERTopic**), and predictive forecasting (**SARIMAX**), this project bridges operational diagnostic friction with actionable growth strategies.

---

## 📂 Project Directory Structure

```text
Olist-E-Commerce-Data-Analysis/
├── Diagnostic & Predictive Analysis (RFM K-means + NLP Topic Model + SARIMAX)/
│   ├── NLP Topic Model/
│   ├── RFM K-means/
│   ├── SARIMAX/
│   └── Diagnostic & Predictive Analysis PowerPoint.pptx
├── PowerBI/
├── Data Collection Methodology.pdf
├── Project_Outline.pdf
└── README.md
```

### 📁 Repository Component Breakdown
* **`NLP Topic Model/`** – Contains Jupyter Notebook scripts, datasets, and output charts/tables.
* **`RFM K-means/`** – Contains Jupyter Notebook scripts, datasets, and output charts/tables.
* **`SARIMAX/`** – Contains Jupyter Notebook scripts, datasets, and output charts/tables.
* **`Diagnostic & Predictive Analysis PowerPoint.pptx`** – Comprehensive slide deck summarizing key project findings and executive presentation deliverables.
* **`PowerBI/`** – Houses compiled interactive dashboard application files (`.pbix`) alongside high-resolution interface screenshots.
* **`Project_Outline.pdf`** – Comprehensive project blueprint documenting precise data cleaning pipelines and the baseline Entity-Relationship Diagram (ERD).
* **`Data Collection Methodology.pdf`** – Comprehensive documentation outlining data collection methodologies, ethical considerations, and core limitations.

---
### 📺 Executive Video Presentations & Walkthroughs

To provide a complete breakdown of this project's architecture, the analytical workflow is split into two specialized video walkthroughs covering both data visualization and advanced intelligence tracks:

| 📊 Power BI Dashboard Analytics | 🧠 Diagnostic & Predictive AI Pipeline |
| :--- | :--- |
| **Focus:** Consumer Purchasing Behaviors & Experience, Geographic Retention & Merchant Performance.<br><br>🎥 **[Watch the Power BI Walkthrough](https://www.youtube.com/watch?v=xFCZaVdFS-o)** | **Focus:** Algorithmic execution across RFM K-Means, BERTopic, and SARIMAX.<br><br>🎥 **[Watch the Advanced ML/NLP Analysis](https://www.youtube.com/watch?v=VGxmjx2cL8I&t=129s)** |

## 📊 Interactive Power BI Dashboards

Our 3-page interactive Power BI Dashboard provides strategic overviews of Sales, Logistics, Product Performance, and Customer Loyalty.

### 🔌 Entity-Relationship Diagram (ERD)
The underlying analytical schema utilizes an optimized star-schema layout to connect customer, seller, order, and product attributes seamlessly.

<p align="center">
  <img src="https://github.com/TimTam672/Olist-E-Commerce-Data-Analysis-Power-BI-Dashboard-Featuring-RFM-K-Means-NLP-and-SARIMAX-/blob/0a015c21da8580df2e7d8d4d44b83380f11986a9/PowerBI/Finalized%20ERD.png" width="100%" alt="Finalized ERD Schema">
</p>

### 🎨 Dashboard Interfaces

![Sales & Logistics](https://github.com/TimTam672/Olist-E-Commerce-Data-Analysis-Power-BI-Dashboard-Featuring-RFM-K-Means-NLP-and-SARIMAX-/blob/8dd34751100f766e6f00c5f98d4859001575e2b5/PowerBI/Sales%20%26%20Logistics.png)

![Product Performance & Customer Sentiment Analysis](https://github.com/TimTam672/Olist-E-Commerce-Data-Analysis-Power-BI-Dashboard-Featuring-RFM-K-Means-NLP-and-SARIMAX-/blob/268303a75f7228182adf85e409647b71c98a92f6/PowerBI/Product%20Performance%20%26%20Customer%20Sentinment%20Analysis.png)

![Customer Loyalty & Seller Ecosystem](https://github.com/TimTam672/Olist-E-Commerce-Data-Analysis-Power-BI-Dashboard-Featuring-RFM-K-Means-NLP-and-SARIMAX-/blob/8eba5989621e8c1bb8fd03057ec9d5ed5ae99e63/PowerBI/Customer%20Loyalty%20%26%20Seller%20Ecosystem.png)

### 🔍 Key Dashboard-Derived Business Insights

* **💳 Consumer Purchasing Behaviors & Experience**
  * **Payment & Timing Preferences**: Transaction data indicates that customers heavily prefer shopping on **weekdays** and overwhelmingly complete purchases utilizing **credit cards** as their primary payment mechanism.
  * **The High-Value Experience Friction**: A critical paradox was identified where **high-spending customer cohorts report significantly lower satisfaction scores (worse user experiences)** compared to baseline spenders. This highlights a pressing need to optimize the premium delivery and customer service funnel.
* **📦 Category Revenue Hierarchy**
  * Aggregate business revenues follow a distinct category structural distribution, led by home goods and trailing into media supplies: `Home & Living` > `Lifestyle` > `Tech & Gadgets` > `Media & Essentials`.
* **🗺️ Geographic Retention & Supply Dynamics**
  * **The Retention Divide**: **Coastal regions exhibit noticeably lower customer retention rates** compared to interior markets. Spatial analysis indicates this churn is primarily driven by intense localized market competition.
  * **Growth Engine Imbalance**: The platform currently faces an over-reliance on **continuous new customer acquisition** to sustain transaction volumes, rather than relying on robust organic user retention.
* **🏪 Merchant Performance & Scaling Friction**
  * **Mature Seller Expansion**: The volume of **stable, long-tenure merchant accounts (3+ months)** operating on the Olist marketplace is steadily expanding, establishing a reliable ecosystem backbone.
  * **The Scale vs. Quality Dilemma**: A strong inverse relationship exists between transaction volumes and service metrics. Merchants managing **high sales volumes face severe structural difficulties in maintaining peak service quality and high ratings**, pointing to a need for better seller logistics infrastructure.

---

## 🧩 Track 1: Customer Segmentation (RFM + K-Means Clustering)

This module builds a robust customer segmentation engine designed to transition the ecosystem away from acquisition reliance toward automated, high-yield retention.

### 🛠️ Data Preprocessing & Methodology
1. **RFM Transformation**: Raw transaction data was tidied into Recency, Frequency, and Monetary metrics and standardized into a **1–4 scale** using statistical quartiles.
2. **Recency Scoring**: Scored inversely—rewarding recent activity—to surface the most engaged, highest-value customers.
3. **Feature Engineering**: 
   * **Log Transformation**: Applied to mitigate heavy monetary skewness.
   * **Standardization**: Harmonized disparate RFM scales to ensure unbiased distance calculations for the K-Means algorithm.
4. **Model Optimization**: The **Elbow Method** identified **K=4** as the optimal cluster count, achieving the best trade-off between model complexity and Within-Cluster Sum of Squares (WCSS) reduction.

### 📈 Key Insights & Strategic Diagnostics
* **New-Customer Dependence**: Our current growth relies heavily on continuous acquisition rather than repeat purchases. This is a structurally unsustainable model.
* **The Loyalty Paradox**: High-value spenders (**Cluster 1**) are not being retained. This creates a severe revenue leak that actively offsets our acquisition gains.
* **Strategic Priority**: Fixing the post-purchase experience for **Cluster 1** high-spenders is the fastest path to transforming transactional cycles into a sustainable loyalty ecosystem.

### 🎯 Targeted Retention & Growth Programs
* **📦 New User Program (Clusters 0 & 2)**
  * *Tactics*: Introductory incentives and welcome bonuses.
  * *Goal*: Convert one-time new customers into repeat buyers.
* **🛡️ Stable Core Program (Cluster 3)**
  * *Tactics*: Exclusive retention programs and tier-based loyalty benefits.
  * *Goal*: Maintain and protect high-value customer engagement.
* **💎 Platinum Tier Program (Top 0.8% | RFM Score 11–12)**
  * *Tactics*: Premium benefits including free shipping and priority customer support.
  * *Goal*: Stabilize our most profitable segment and maximize Customer Lifetime Value (CLV).

![Elbow](https://github.com/TimTam672/Olist-E-Commerce-Data-Analysis-Power-BI-Dashboard-Featuring-RFM-K-Means-NLP-and-SARIMAX-/blob/3540e95101ae8eb3fb4d74e0a722d65d6970aff3/Diagnostic%20%26%20Predictive%20Analysis%20(RFM%20K-means%20%2B%20NLP%20Topic%20Model%20%2B%20SARIMAX)/RFM%20K-means/Elbow.png) 

![Olist KMeans Table](https://github.com/TimTam672/Olist-E-Commerce-Data-Analysis-Power-BI-Dashboard-Featuring-RFM-K-Means-NLP-and-SARIMAX-/blob/3540e95101ae8eb3fb4d74e0a722d65d6970aff3/Diagnostic%20%26%20Predictive%20Analysis%20(RFM%20K-means%20%2B%20NLP%20Topic%20Model%20%2B%20SARIMAX)/RFM%20K-means/Olist_KMeans_Diagnostic_Table_Final.png) |

---

## 🔤 Track 2: NLP Topic Modelling & Customer Pain Point Discovery

We applied advanced NLP sentiment analysis on **9,869 1-star reviews** to extract and isolate structural drivers of platform dissatisfaction down to **4 core operational risk themes** (encompassing 5,619 high-impact reviews).

### 🛠️ Pipeline Methodology & Technical Stack
1. **Neural Translation**: Used Facebook's **NLLB-200** model to normalize international customer feedback by converting Portuguese text to English while strictly preserving semantic nuances.
2. **Rigorous Text Preprocessing**: Stripped URLs, punctuation, digits, and nonsensical strings; pruned standard stop words, high-frequency baseline terms, and rare outliers; and executed emoticon-to-text mapping alongside strict lemmatization.
3. **Quality Audit & Validation**: Leveraged **LaBSE (Language-Agnostic BERT Sentence Embedding)** to run semantic similarity checks. Achieved a benchmark score of **0.657**, validating that textual meaning was completely preserved post-cleaning.
4. **Advanced Refinement & Topic Discovery**: Integrated `CountVectorizer` to catch multi-word phrases/n-grams, passing them to a **BERTopic** pipeline optimized with `KeyBERTInspired` embeddings.

### 📊 Structural Matrix: Themes by Category

| Core Theme | Home & Living | Tech & Gadgets | Media & Essentials | Lifestyle |
| :--- | :---: | :---: | :---: | :---: |
| **Product Specification** | 🔴 Discrepancies | | | |
| **Installation Issues** | | 🔴 Poor Manuals | | |
| **Customer Anxiety** | | | 🔴 Poor Tracking | 🔴 Poor Tracking |
| **Fulfillment & Returns** | ⚠️ High Impact | ⚠️ High Impact | ⚠️ High Impact | ⚠️ High Impact |

### 🎯 NLP Solutions & Operational Interventions
* **📋 1. Proactive Logistics & Dispute Management**
  * *Interventions*: Deploy **Live Customer Service** frameworks to mediate and de-escalate transaction disputes in real-time. Construct automated monitoring triggers for orders with extreme lead times, backed by **strict penalties** for underperforming third-party sellers.
  * *Expected Result*: Target and eliminate systemic **Customer Anxiety** (both "Action" and "Psychological" blockers), dropping anxiety-driven customer support tickets significantly.
* **🛡️ 2. Product Integrity & Information Standards**
  * *Interventions*: Execute a platform-wide **specification audit** to purge inaccurate product sheets. Enforce a **Mandatory Digital Documentation** standard, requiring merchants to supply localized video tutorials or enhanced digital manuals.
  * *Expected Result*: Systematically eliminate **Specification Discrepancies** and **Installation Failures**, reducing avoidable post-purchase returns.

![WordCloud](https://github.com/TimTam672/Olist-E-Commerce-Data-Analysis-Power-BI-Dashboard-Featuring-RFM-K-Means-NLP-and-SARIMAX-/blob/3540e95101ae8eb3fb4d74e0a722d65d6970aff3/Diagnostic%20%26%20Predictive%20Analysis%20(RFM%20K-means%20%2B%20NLP%20Topic%20Model%20%2B%20SARIMAX)/NLP%20Topic%20Model/WordCloud.png) 

![Customer Pain Point Diagnosis Matrix](https://github.com/TimTam672/Olist-E-Commerce-Data-Analysis-Power-BI-Dashboard-Featuring-RFM-K-Means-NLP-and-SARIMAX-/blob/3540e95101ae8eb3fb4d74e0a722d65d6970aff3/Diagnostic%20%26%20Predictive%20Analysis%20(RFM%20K-means%20%2B%20NLP%20Topic%20Model%20%2B%20SARIMAX)/NLP%20Topic%20Model/Customer%20Pain%20Point%20Diagnosis%20Matrix.png) 

---

## 📈 Track 3: Predictive Time-Series Forecasting (SARIMAX Model)

To proactively navigate future shifts across macro product categories, I implemented a **SARIMAX (Seasonal Autoregressive Integrated Moving Average with Exogenous Regressors)** model, turning operational friction points into model parameters.

### 🛠️ Model Specification & Feature Engineering
* **Exogenous Variables (External Drivers)**: Integrated **Weekend Ratio** and **Delivery Days** directly into the model to isolate how consumer purchasing patterns and courier lag affect revenue.
* **Model Selection**: The **Media & Essentials** category achieved the **lowest AIC (Akaike Information Criterion)** score, rendering its revenue predictions the most stable, reliable, and mathematically sound across the portfolio.
* **Growth Vector**: Time-series projections identify **Media & Essentials** as possessing the most dominant long-term growth trend compared to all other product categories.

### 📊 Strategic Forecasting & Trend Insights
* **🚀 Standout Performer (Media & Essentials)**: Projected to achieve a dominant **9.7% increase** in revenue. Revenue in this category is heavily influenced by **delivery speed**.
* **🛡️ Resilient Core (Lifestyle)**: Demonstrates stable structural health, maintaining a steady and predictable momentum with a projected **1.3% growth**.
* **⚠️ Declining Categories (Tech & Home)**: 
  * **Tech & Gadgets**: Anticipated to experience the most significant contraction, dropping by **3.7%**.
  * **Home & Living**: Expected to experience a moderate structural decline of **1.8%**.

### 🎯 Predictive Solutions & Growth Strategy
* **💰 1. Strategic Resource Reallocation**
  * *Interventions*: Reallocate paid performance marketing budgets away from contracting segments (**Tech & Gadgets**) and heavily toward the **Media & Essentials** category to lock in predictable, high-margin transaction flows.

* **🚚 2. Logistics Stress Testing for Media & Essentials**
  * *Interventions*: Conduct aggressive logistical stress testing specifically tailored to the Media & Essentials merchant network. Compress average delivery days, keeping velocity high.
  * 
![Olist SARIMAX Forecast Charts](https://github.com/TimTam672/Olist-E-Commerce-Data-Analysis-Power-BI-Dashboard-Featuring-RFM-K-Means-NLP-and-SARIMAX-/blob/3540e95101ae8eb3fb4d74e0a722d65d6970aff3/Diagnostic%20%26%20Predictive%20Analysis%20(RFM%20K-means%20%2B%20NLP%20Topic%20Model%20%2B%20SARIMAX)/SARIMAX/Olist_SARIMAX_Forecast_Charts.png) 

![Olist Strategic Analysis Table](https://github.com/TimTam672/Olist-E-Commerce-Data-Analysis-Power-BI-Dashboard-Featuring-RFM-K-Means-NLP-and-SARIMAX-/blob/3540e95101ae8eb3fb4d74e0a722d65d6970aff3/Diagnostic%20%26%20Predictive%20Analysis%20(RFM%20K-means%20%2B%20NLP%20Topic%20Model%20%2B%20SARIMAX)/SARIMAX/Olist_Strategic_Analysis_Table.png)
