# Digital Marketing Campaign Sales Analysis

An end-to-end Exploratory Data Analysis (EDA) project that investigates the performance of digital marketing campaigns and identifies the key factors driving customer conversions.

---

##  Project Overview

Digital marketing campaigns run across multiple channels — Email, Social Media, PPC, SEO, and Referral — but understanding *which* channels, *which* customers, and *which* strategies actually convert is the real challenge. This project digs into a dataset of 8,000 customer records to uncover patterns in customer behavior, campaign effectiveness, advertising spend, and engagement metrics.

The findings are designed to help marketers make smarter, data-driven decisions about budget allocation and campaign targeting.

---

##  Objectives

- Identify the most valuable customer segments
- Analyze which age groups and genders respond best to different campaigns
- Determine the most effective marketing channels and campaign types
- Examine customer behaviors that lead to conversions
- Evaluate the impact of advertising spend on campaign performance
- Provide actionable recommendations for future marketing strategies

---

##  Dataset

| Attribute | Details |
|---|---|
| **Source** | [GitHub — digital-marketing-campaign-conversion-prediction](https://github.com/Elakkiya-U/digital-marketing-campaign-conversion-prediction) |
| **File** | `Digital_Marketing_Campaign_Dataset.csv` |
| **Records** | 8,000 rows |
| **Features** | 20 columns |
| **Target Variable** | `Conversion` (0 = No Conversion, 1 = Conversion) |

### Key Features

| Column | Description |
|---|---|
| `Age`, `Gender`, `Income` | Customer demographics |
| `CampaignChannel` | Marketing channel (Email, PPC, SEO, Social Media, Referral) |
| `CampaignType` | Campaign objective (Awareness, Conversion, Retention, Consideration) |
| `AdSpend` | Advertising expenditure |
| `ClickThroughRate`, `ConversionRate` | Campaign performance metrics |
| `WebsiteVisits`, `PagesPerVisit`, `TimeOnSite` | Engagement metrics |
| `EmailOpens`, `EmailClicks`, `SocialShares` | Channel interaction metrics |
| `PreviousPurchases`, `LoyaltyPoints` | Customer loyalty indicators |

---

##  Tech Stack

| Library | Purpose |
|---|---|
| `pandas` | Data loading, cleaning, and manipulation |
| `numpy` | Numerical operations |
| `matplotlib` | Static visualizations |
| `seaborn` | Statistical visualizations |
| `plotly` | Interactive charts and dashboards |

---

## Project Structure

```
├── Digital_Marketing_Campaign_Sales_Analysis.ipynb   # Main analysis notebook
├── Digital_Marketing_Campaign_Dataset.csv            # Dataset (download separately)
└── README.md
```

---

##  Analysis Workflow

### 1. Data Loading & Initial Overview
Loading the dataset and examining its shape, structure, and basic statistics.

### 2. Data Preprocessing
- **Missing Values** — No missing values found; dataset was complete.
- **Duplicate Records** — No duplicates detected.
- **Trailing Spaces** — Stripped from all categorical columns.
- **Column Renaming** — Standardized to readable, space-separated labels.
- **Derived Columns** — Created `Age Group`, `Income Group`, and `Customer Value Score`.
- **Column Removal** — Dropped `Customer ID`, `Advertising Platform`, and `Advertising Tool` as non-informative.

### 3. Exploratory Data Analysis (EDA)
- **Univariate Analysis** — Distribution of individual features
- **Bivariate Analysis** — Conversion rates by channel, campaign type, gender, age, and income
- **Multivariate Analysis** — Combined impact of multiple demographic and campaign variables

### 4. Data Visualization (7 Sections)
| Section | Focus |
|---|---|
| I | Customer Demographics |
| II | Customer Segmentation & Conversion |
| III | Advanced Segmentation (Age × Gender × Channel) |
| IV | Campaign Performance |
| V | Customer Engagement |
| VI | Advertising Spend & Marketing ROI |
| VII | Distribution Analysis of Numerical Variables |

### 5. Insights & Recommendations
A comprehensive report with key findings and future strategy recommendations.

---

##  Key Findings

- **Conversion campaigns** dramatically outperform all other campaign types (~93% conversion rate vs ~85–86% for others).
- The **36–45 age group** is the highest-converting segment (90.14%) and the most engaged across all channels.
- **Referral (88.31%)** and **PPC (88.28%)** are the top-performing marketing channels.
- **Gender has virtually no impact** on conversion rates (males: 87.69% vs females: 87.62%).
- **Ad spend shows near-zero correlation** with conversions and website visits — more spending doesn't guarantee better results.
- **Low-income customers** show high engagement during the Consideration phase but drop off sharply at conversion, indicating a price-sensitivity barrier.
- **SEO and PPC** work best for males aged 36–45; **Email** is more reliable for males aged 46–55.

---

## Strategic Recommendations

1. **Shift budget toward Conversion campaigns** — they deliver the highest ROI by a significant margin.
2. **Prioritize the 36–45 age segment** in creative, messaging, and targeting strategies.
3. **Deploy channel-specific strategies by segment** rather than uniform budget allocation across all channels.
4. **Move to performance-based budget allocation** — ad spend volume alone does not drive outcomes.
5. **Address the low-income conversion barrier** with tiered pricing, friction reduction, and trust-building content.
6. **Build retention campaigns** for high Customer Value Score segments (age 36–65) to maximize lifetime value.

---
