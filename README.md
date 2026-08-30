# 📊 Data Analytics Internship Portfolio — ApexPlanet Software Pvt. Ltd.

**Intern Name:** [Your Name]
**Program:** 60-Day Data Analytics Internship
**Organization:** ApexPlanet Software Pvt. Ltd.
**Website:** [www.apexplanet.in](https://www.apexplanet.in)
**Program Duration:** 60 Days (5 Tasks)

---

## 📖 Table of Contents

1. [About ApexPlanet Software Pvt. Ltd.](#about-apexplanet-software-pvt-ltd)
2. [About This Internship Program](#about-this-internship-program)
3. [Repository Structure](#repository-structure)
4. [Task 1: Data Immersion & Wrangling](#task-1-data-immersion--wrangling)
5. [Task 2: Exploratory Data Analysis (EDA) & Business Intelligence](#task-2-exploratory-data-analysis-eda--business-intelligence)
6. [Task 3: Deep-Dive Analysis & Interactive Dashboarding](#task-3-deep-dive-analysis--interactive-dashboarding)
7. [Task 4: Data Storytelling & Statistical Validation](#task-4-data-storytelling--statistical-validation)
8. [Tools & Technologies Used](#tools--technologies-used)
9. [Skills Gained Across the Internship](#skills-gained-across-the-internship)
10. [Key Learnings & Reflections](#key-learnings--reflections)
11. [Challenges Faced & How I Overcame Them](#challenges-faced--how-i-overcame-them)
12. [Contact & Acknowledgements](#contact--acknowledgements)

---

## 🏢 About ApexPlanet Software Pvt. Ltd.

At ApexPlanet Software Pvt. Ltd., the mission is to drive innovation and excellence in digital solutions. Founded with a vision to empower businesses through cutting-edge technology, the company specializes in delivering top-notch web development and app development services tailored to client needs.

Beyond client services, ApexPlanet is deeply committed to nurturing the next generation of tech talent through comprehensive internship programs that provide hands-on experience and mentorship — preparing aspiring developers and analysts for successful careers in the tech industry.

This repository is a direct output of that mission: a real, hands-on **Data Analytics Internship** structured around practical, portfolio-ready tasks.

---

## 🎯 About This Internship Program

The **60-Day Data Analytics Internship** was structured into 5 progressive tasks, each building on the skills developed in the previous one — simulating a real-world data analyst's workflow from raw data to executive-level storytelling:

| Task | Title | Timeline | Focus Area |
|------|-------|----------|------------|
| 1 | Data Immersion & Wrangling | 10 Days | Data cleaning & preparation |
| 2 | EDA & Business Intelligence | 14 Days | Pattern discovery & SQL |
| 3 | Deep-Dive Analysis & Dashboarding | 12 Days | KPIs & interactive BI tools |
| 4 | Data Storytelling & Statistical Validation | 16 Days | Narrative & hypothesis testing |
| 5 | Capstone Integration & Portfolio | 8 Days | Final portfolio consolidation |

Each task required two deliverables: a GitHub submission (code, reports, datasets, dashboards) and a LinkedIn video walkthrough explaining the work and findings.

This document (part of Task 5) consolidates and documents the work completed in **Tasks 1 through 4**.

---

## 🗃️ Repository Structure

```
DataAnalyst-Internship-Portfolio/
│
├── ApexPlanet-Task1-Data-Wrangling/
│   ├── data_dictionary.xlsx
│   ├── cleaning_script.ipynb
│   ├── raw_dataset.csv
│   └── cleaned_dataset.csv
│
├── ApexPlanet-Task2-EDA-BI/
│   ├── eda_report.ipynb
│   ├── sql_queries.sql
│   ├── visualizations/
│   └── dashboard_mockup.pptx
│
├── ApexPlanet-Task3-DeepDive-Dashboard/
│   ├── deep_dive_report.ipynb
│   ├── kpi_definitions.md
│   └── dashboard_link.md
│
├── ApexPlanet-Task4-Storytelling-Stats/
│   ├── final_presentation.pptx
│   ├── hypothesis_testing_summary.ipynb
│   └── narrative_report.md
│
├── ApexPlanet-Task5-Capstone-Portfolio/
│   └── (this repository)
│
└── README.md  ← You are here
```

---

## 🧩 Task 1: Data Immersion & Wrangling

**⏱ Timeline:** 10 Days

### Objective
To rapidly acquaint myself with the provided dataset and master the critical first step of any analysis: acquiring, cleaning, and preparing data for downstream use.

### Detailed Breakdown of Work

#### 1. Data Access & Familiarization
- Gained access to a real-world style dataset (sales transactions / website analytics / customer records)
- Reviewed every column and its likely business context
- Built a **complete data dictionary** documenting:
  - Column name
  - Data type (numeric, categorical, date, text, boolean)
  - Description of what the field represents
  - Business relevance (e.g., "used for calculating monthly revenue," "used to segment repeat customers")

#### 2. Data Quality Assessment
- Ran a full **data profiling pass** across the dataset to catch:
  - **Missing values** — identified which columns had nulls and what percentage of rows were affected
  - **Duplicate records** — checked for exact and near-duplicate rows
  - **Inconsistent formatting** — mismatched date formats, inconsistent capitalization in categorical fields, extra whitespace
  - **Outliers** — used boxplots and z-score/IQR methods to flag anomalous numeric values (e.g., negative prices, impossible ages)

#### 3. Data Cleaning & Transformation
- Wrote a full **cleaning script in Python (Pandas)** to systematically resolve every identified issue:
  - Filled or dropped missing values based on context-appropriate strategy (mean/median imputation, forward-fill, or removal)
  - Removed duplicate rows
  - Standardized all date columns to a single consistent format (`YYYY-MM-DD`)
  - Normalized categorical text fields (trimmed whitespace, standardized casing)
  - Performed **feature engineering**, including:
    - Deriving `Customer Age` from `Date of Birth`
    - Creating `Order Month` and `Order Year` from transaction dates
    - Bucketing continuous variables into categories (e.g., age groups)
- Output a final, fully **analysis-ready cleaned dataset**

### Deliverables Produced
- ✅ Data dictionary (Excel/Markdown)
- ✅ Cleaning script (Jupyter Notebook / Python file)
- ✅ Cleaned dataset (CSV)
- ✅ Video walkthrough of data issues found and how each was resolved

### Key Takeaway
This task reinforced that **data cleaning is not a one-time checkbox** — it requires deliberate, well-documented decisions at every step, since those choices directly affect the validity of every downstream analysis.

---

## 📈 Task 2: Exploratory Data Analysis (EDA) & Business Intelligence

**⏱ Timeline:** 14 Days

### Objective
To uncover patterns, trends, and relationships within the cleaned dataset, while developing proficiency in SQL for structured data extraction and building foundational dashboarding skills.

### Detailed Breakdown of Work

#### 1. Descriptive Statistics & Univariate Analysis
- Calculated key summary statistics for every numerical field: mean, median, mode, standard deviation, min/max, quartiles
- Calculated frequency distributions for categorical fields
- Built univariate visualizations:
  - Histograms for numeric distributions (e.g., order value distribution)
  - Bar charts for categorical breakdowns (e.g., customers by region)

#### 2. SQL for Business Questions
Answered a curated set of **5–7 real business questions** using SQL, such as:
- What are the top 5 products by revenue in the last 6 months?
- What is the monthly user acquisition trend?
- Which customer segment generates the highest average order value?
- What percentage of orders come from repeat customers?
- Which region has the highest churn rate?

For each question, I wrote SQL queries using:
- `GROUP BY` and aggregation functions (`SUM`, `AVG`, `COUNT`)
- `JOIN`s across multiple related tables (e.g., customers, orders, products)
- Filtering with `WHERE` and `HAVING` clauses
- Window functions for trend calculations where applicable

#### 3. Multivariate Analysis & Correlation
- Built advanced visualizations to explore relationships between two or more variables:
  - **Scatter plots** (e.g., marketing spend vs. sales)
  - **Correlation heatmaps** across all numeric fields
  - **Pair plots** to visualize multiple variable relationships simultaneously
- Interpreted correlation coefficients to identify which variables had meaningful relationships worth deeper investigation

#### 4. Static Dashboard Mock-up
- Synthesized EDA insights into a **static dashboard mock-up** built in PowerPoint/Excel
- Proposed the most important KPIs worth tracking going forward (e.g., Monthly Revenue, Customer Acquisition Rate, Average Order Value)
- Designed the mock-up with a business audience in mind — clear visual hierarchy, minimal clutter, actionable metrics front and center

### Deliverables Produced
- ✅ Full EDA report (Jupyter Notebook/PDF)
- ✅ SQL query file with results and explanations
- ✅ Static dashboard mock-up (PPT/Excel)
- ✅ Video showcase of key insights and most complex queries

### Key Takeaway
This task bridged the gap between **raw data and business value** — showing how the same dataset can answer very different stakeholder questions depending on how it's queried and visualized.

---

## 📊 Task 3: Deep-Dive Analysis & Interactive Dashboarding

**⏱ Timeline:** 12 Days

### Objective
To answer complex, multi-faceted business problems through a focused deep-dive analysis, and to build a fully functional, interactive dashboard using a professional BI tool.

### Detailed Breakdown of Work

#### 1. Define Core KPIs
Formally defined **3–5 core Key Performance Indicators**, each with:
- A precise formula
- A clear business rationale for why it matters

Examples of KPIs defined:
- **Conversion Rate** = (Number of Conversions / Total Visitors) × 100
- **Customer Churn Rate** = (Customers Lost / Total Customers at Start of Period) × 100
- **Average Order Value (AOV)** = Total Revenue / Number of Orders

#### 2. Deep-Dive Analysis
Selected **one focused business area** for deep analysis. (Keep only the one that matches your actual work):

- **Cohort Analysis** — Grouped customers by acquisition month/period and tracked retention and lifetime value over time to understand how customer value evolves
- **Funnel Analysis** — Mapped out each stage of a key user journey (e.g., visit → sign-up → cart → purchase) and quantified drop-off rates at each stage to identify friction points
- **Segmentation Analysis** — Applied clustering techniques (e.g., K-Means) or rule-based segmentation to group customers by behavior, value, or demographics for targeted business strategy

#### 3. Interactive Dashboard Build
- Built a **fully interactive, live dashboard** using a professional BI tool (Tableau / Power BI / Looker Studio)
- The dashboard included:
  - Filters and slicers so users can explore data dynamically
  - Visual surfacing of all core KPIs defined earlier
  - Drill-down capability into the deep-dive analysis area
  - Clean, professional layout suitable for stakeholder presentation

### Deliverables Produced
- ✅ Deep-dive analysis report
- ✅ Live, published interactive dashboard
- ✅ Video demo of the dashboard and key findings walkthrough

### Key Takeaway
This task pushed beyond static reporting into **self-service analytics** — building tools that let non-technical stakeholders explore data on their own rather than relying on a report for every question.

---

## 🎤 Task 4: Data Storytelling & Statistical Validation

**⏱ Timeline:** 16 Days

### Objective
To synthesize all prior analysis (Tasks 1–3) into one compelling, cohesive business narrative — and to apply basic statistical methods to add scientific rigor and validate key findings before presenting them as conclusions.

### Detailed Breakdown of Work

#### 1. Craft the Data Story
- Structured all findings from the previous three tasks into a single, cohesive narrative built for a business (non-technical) audience
- Ensured the story followed a clear arc:
  - **Objective** — what business question were we trying to answer?
  - **Analysis** — what did we do and find?
  - **Conclusions** — what does this mean for the business?
  - **Call to Action** — what should stakeholders actually do with this information?

#### 2. Develop the Final Presentation
- Built a **polished, professional presentation deck** (PowerPoint/Google Slides)
- Prioritized:
  - Visual clarity over text-heavy slides
  - One key insight per slide
  - Business impact framing (revenue, retention, cost savings) rather than pure statistics
  - Consistent branding and design throughout

#### 3. Hypothesis Testing
- Formulated a clear, **testable business hypothesis**, for example:
  > "The new website layout led to a statistically significant increase in conversion rate."
- Selected and performed the appropriate statistical test:
  - **T-test** for comparing means between two groups (e.g., A/B test of old vs. new layout)
  - **Chi-squared test** for comparing proportions across categorical groups
- Interpreted results rigorously:
  - Calculated and interpreted **p-values**
  - Calculated **confidence intervals**
  - Translated statistical significance into a clear, plain-English **business conclusion** (avoiding statistical jargon for the stakeholder audience)

### Deliverables Produced
- ✅ Final, polished presentation deck
- ✅ Hypothesis testing summary document/notebook
- ✅ Video presentation delivering stakeholder-style insights

### Key Takeaway
This task taught me that **data is only as valuable as the story told around it** — and that statistical validation is what separates a confident business recommendation from a guess dressed up in a chart.

---

## 🛠️ Tools & Technologies Used

| Category | Tools / Technologies |
|---|---|
| Programming Languages | Python, SQL |
| Data Manipulation | Pandas, NumPy |
| Data Visualization | Matplotlib, Seaborn, Plotly |
| Statistical Analysis | SciPy, StatsModels |
| BI / Dashboarding | Tableau / Power BI / Looker Studio |
| Presentation | PowerPoint, Google Slides |
| Version Control | Git, GitHub |
| Documentation | Markdown, Jupyter Notebooks |

---

## 🎓 Skills Gained Across the Internship

**Technical Skills**
- Data cleaning, wrangling, and feature engineering
- Writing efficient, multi-table SQL queries
- Exploratory and multivariate data analysis
- Building interactive BI dashboards
- Applying and interpreting statistical hypothesis tests (T-tests, Chi-squared tests)
- Version control and professional GitHub repository management

**Business & Soft Skills**
- Translating raw data into actionable business insights
- Defining and justifying KPIs from a business rationale perspective
- Data storytelling for non-technical stakeholders
- Structuring a narrative around objective → analysis → conclusion → action
- Presenting findings confidently on video
- Professional documentation and portfolio building

---

## 💡 Key Learnings & Reflections

Throughout this 60-day internship, the most valuable lesson was understanding that **data analytics is a full pipeline, not a single skill**. Every task built directly on the previous one:

1. **Clean data enables trustworthy analysis** — no amount of clever visualization can fix a poorly cleaned dataset.
2. **SQL and EDA together uncover the "what"** — patterns and trends that raise the right business questions.
3. **Dashboards make insights actionable and repeatable** — turning a one-time analysis into an ongoing decision-making tool.
4. **Statistics turn opinions into evidence** — a compelling story is only credible when it's backed by rigorous validation.

This progression mirrors the real-world responsibilities of a working data analyst, and completing it end-to-end gave me a genuine, portfolio-ready body of work rather than a series of disconnected exercises.

---

## 🧗 Challenges Faced & How I Overcame Them

| Challenge | How I Solved It |
|---|---|
| Handling inconsistent date formats across the dataset | Used Pandas' `to_datetime()` with format inference, then standardized to ISO format |
| Writing efficient multi-table SQL joins without duplicating rows | Carefully mapped primary/foreign key relationships before joining, and validated row counts before/after each join |
| Choosing the right statistical test for hypothesis validation | Researched assumptions behind T-tests vs. Chi-squared tests and matched the test to the data type (continuous vs. categorical) |
| Making a dashboard genuinely "interactive" rather than just static charts | Learned filter/parameter functionality in the BI tool to let users control the view dynamically |
| Presenting technical findings to a non-technical audience | Practiced simplifying language, focusing on business impact framing over statistical terminology in the final presentation |

---

## 📬 Contact & Acknowledgements

I'd like to thank **ApexPlanet Software Pvt. Ltd.** for structuring such a comprehensive, real-world internship program that closely mirrors the actual workflow of a professional data analyst.

**ApexPlanet Software Pvt. Ltd.**
📞 +91 99058 79870
📧 apexplanetgaya@gmail.com
🌐 [www.apexplanet.in](https://www.apexplanet.in)

---

*This README is part of Task 5: Capstone Integration & Portfolio Finalization for the ApexPlanet Data Analytics Internship Program. It serves as the central homepage summarizing all work completed across Tasks 1–4.*
