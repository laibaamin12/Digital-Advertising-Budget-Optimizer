# Digital Advertising Budget Optimizer

**A Python-based project for analyzing digital advertising campaigns, evaluating marketing performance, and recommending an optimized advertising budget allocation across multiple platforms.**

---

## 1. Project Overview

Businesses invest significant amounts in digital advertising across platforms such as Facebook, Instagram, Google, TikTok, and YouTube. However, deciding how to distribute advertising budgets effectively is a major challenge.

The Digital Advertising Budget Optimizer analyzes historical campaign performance using key marketing metrics to identify high-performing platforms and recommend how a company should allocate its next **Rs. 1,000,000 advertising budget**.

The project uses simulated campaign data, Python-based analytics, and a performance-based budget recommendation approach to support data-driven marketing decisions.

## 2. Project Objectives

- Analyze digital advertising campaign performance across multiple platforms.
- Generate and analyze synthetic advertising datasets.
- Calculate important marketing performance metrics.
- Identify high-performing and low-performing advertising platforms.
- Analyze campaign performance across different audience segments.
- Compare data processing performance using Pandas, MapReduce, and Apache Spark.
- Develop a Marketing Budget Recommendation Engine.
- Recommend an optimized allocation of Rs. 1,000,000 based on historical ROAS.

## 3. Advertising Platforms

The project analyzes five major digital advertising platforms:

- Facebook
- Instagram
- Google
- TikTok
- YouTube

## 4. Dataset Description

The project generates a synthetic dataset using Python and NumPy.

The initial dataset contains **10,000 campaign records** with the following attributes:

| Column | Description |
|---|---|
| Date | Campaign activity date |
| Campaign | Campaign identifier |
| Platform | Advertising platform |
| Impressions | Number of times an advertisement is displayed |
| Clicks | Number of clicks received |
| Spend | Advertising expenditure |
| Conversions | Number of completed conversions |
| Revenue | Revenue generated |
| Age | Customer age group |
| Gender | Customer gender |
| City | Customer location |
| Device | Device used by the customer |

The dataset also supports analysis across different audience demographics, geographical locations, and devices.

**Note:** The dataset is simulated and does not represent actual advertising campaign records.

## 5. Key Performance Metrics

The project calculates the following marketing performance indicators:

| Metric | Formula | Purpose |
|---|---|---|
| CTR | (Clicks / Impressions) × 100 | Measures advertisement engagement |
| CPC | Spend / Clicks | Measures cost per click |
| CPA | Spend / Conversions | Measures cost per acquisition/conversion |
| CVR | (Conversions / Clicks) × 100 | Measures conversion efficiency |
| ROAS | Revenue / Spend | Measures advertising return |
| Revenue | Total generated revenue | Measures campaign revenue |

These metrics help compare advertising platforms and identify opportunities for improving marketing efficiency.

## 6. Project Methodology

The project follows these major stages:

### Stage 1: Synthetic Data Generation

- Generate 10,000 simulated advertising records.
- Assign campaign data across five advertising platforms.
- Generate impressions, clicks, spending, conversions, and revenue.
- Include demographic and geographical attributes.

### Stage 2: Performance Analysis

- Calculate CTR, CPC, CPA, CVR, and ROAS.
- Aggregate campaign performance by advertising platform.
- Identify the best and weakest platforms based on ROAS.
- Compare performance across age, gender, city, and device categories.

### Stage 3: Data Visualization

Generate visualizations to understand:

- ROAS by advertising platform.
- Monthly ROAS trends.
- Recommended budget distribution.
- Platform and device performance.

### Stage 4: Big Data Simulation

To understand how different processing approaches perform with increasing dataset sizes, the project generates:

- 10,000 records
- 100,000 records
- 1,000,000 records

The execution time of three processing approaches is compared:

**Pandas**
- Uses DataFrame operations and group-by aggregation.
- Suitable for small and medium-sized datasets.

**MapReduce**
- Implemented as a pure Python simulation.
- Demonstrates the Map, Shuffle, and Reduce stages.
- Groups campaign records by advertising platform.

**Apache Spark**
- Uses PySpark for distributed data processing.
- Reads CSV datasets and performs platform-wise aggregation.

The processing time is recorded and visualized to compare performance across dataset sizes.

*Note: The current benchmark implementation covers up to 1 million records. A 10-million-record benchmark is a potential future extension.*

### Stage 5: Marketing Budget Recommendation Engine

The project recommends how to distribute a fixed advertising budget of Rs. 1,000,000.

The recommendation uses a weighted allocation approach:

- 70% weight based on historical platform ROAS.
- 30% weight based on equal budget distribution.

The engine calculates:

- Recommended budget percentage for each platform.
- Recommended budget amount in Pakistani Rupees.
- Historical platform ROAS.
- Estimated revenue based on historical ROAS.

This approach balances performance-based allocation with budget diversification.

## 7. Technologies and Tools

| Technology | Purpose |
|---|---|
| Python | Main programming language |
| Pandas | Data manipulation and analysis |
| NumPy | Synthetic data generation and numerical operations |
| Matplotlib | Data visualization |
| Jupyter Notebook | Project development and execution |
| MapReduce | Simulated large-scale data processing |
| Apache Spark / PySpark | Distributed data processing |
| GitHub | Version control and project documentation |

## 8. Project Structure

```text
Digital-Advertising-Budget-Optimizer/
│
├── Digital_Advertising_Budget_Optimizer.ipynb
│
└── README.md
```

The Jupyter Notebook contains the complete implementation, including data generation, metric calculations, campaign analysis, visualizations, budget recommendations, and processing-time comparisons.

## 9. How to Run the Project

### Requirements

- Python 3.x
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- PySpark (for Spark comparison)

### Install Dependencies

```bash
pip install pandas numpy matplotlib
```

For Spark processing:

```bash
pip install pyspark
```

### Run the Notebook

1. Clone or download the repository.
2. Open the project notebook in Jupyter Notebook.
3. Install the required dependencies.
4. Execute the notebook cells in sequence.
5. Review the campaign analysis, visualizations, and budget recommendations.

## 10. Expected Outcomes

The project provides:

- A comprehensive analysis of digital advertising performance.
- Platform-wise comparison using marketing performance metrics.
- Identification of high-performing advertising channels.
- Audience segmentation insights.
- Processing-time comparison between Pandas, MapReduce, and Spark.
- A data-driven recommendation for distributing Rs. 1,000,000 across advertising platforms.

## 11. Limitations

- The project uses simulated rather than real advertising data.
- Budget recommendations depend on historical ROAS.
- Actual advertising performance may change when budgets increase.
- The current Big Data benchmark is limited to 1 million records.
- Spark performance depends on the available computing environment.

## 12. Future Enhancements

- Extend Big Data simulation to 10 million records.
- Integrate real advertising platform datasets.
- Develop an interactive marketing analytics dashboard.
- Introduce predictive models for campaign performance.
- Incorporate diminishing returns into budget optimization.
- Improve budget allocation using advanced optimization techniques.

## 13. GitHub References

The following open-source projects were reviewed as references for campaign analytics, marketing metrics, and advertising budget optimization.

**1. Marketing Campaign Performance Analysis**

https://github.com/reactwithrajeev/Marketing-Campaign-Performance-Analysis

Relevant concepts:
- Campaign performance analysis.
- CTR, CPC, CPA, CVR, and ROAS.
- Marketing analytics and visualization.

**2. Marketing Budget Optimizer**

https://github.com/adwaith27/Marketing-budget-optimizer

Relevant concepts:
- Marketing budget allocation.
- Optimization across multiple advertising channels.
- Performance-based spending recommendations.

**3. Automated Marketing Budget Optimizer**

https://github.com/ahmedsaad181920h-dot/Automated-Marketing-Budget-Optimizer

Relevant concepts:
- ROAS-based campaign evaluation.
- Weighted budget reallocation.
- Multi-channel advertising analysis.

**4. Marketing Analytics – LTV & CAC**

https://github.com/elfakb/marketing-analytics-ltv-cac

Relevant concepts:
- Customer Acquisition Cost (CAC).
- Return on Ad Spend (ROAS).
- Conversion analysis.
- Marketing efficiency.

These repositories were reviewed for learning and reference purposes. The present project has its own simulated dataset, analysis workflow, and budget recommendation implementation.

---

## 14. Conclusion

The Digital Advertising Budget Optimizer demonstrates how data analytics and Big Data processing approaches can support digital marketing decisions.

By analyzing campaign performance, calculating key marketing metrics, comparing processing techniques, and developing a budget recommendation engine, the project provides a structured approach to improving advertising budget allocation and marketing efficiency.
