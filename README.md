# Impact of Generative AI on Students' Academic Performance

A **Statistics & Data Analysis** group project for course **RM402E**.
We analyse 50,000 student records to answer one question:

> **Does the way students use generative AI help or hurt their academic performance,
> skill retention and well-being?**

The Jupyter notebook is the full report — code, charts and written interpretation together.

**Repository:** https://github.com/Jp-Rsb/SDA_Group1_Team4

##  Dataset
- **Source:** [AI Impact on Students](https://www.kaggle.com/datasets/laveshjadon/ai-impact-on-students) (Kaggle, author *laveshjadon*)
- **Size:** 50,000 rows × 16 columns · **License:** CC0 (Public Domain)
- **File in this repo:** `ai_student_impact_dataset.csv`

## Methods applied
- Descriptive statistics, probability & distributions (normality, Q–Q, empirical rule)
- Exploratory Data Analysis (correlation heatmap, boxplots, scatter/regression plots)
- Hypothesis testing & confidence intervals (paired *t*, Welch *t* + Cohen's *d*, one-way ANOVA, chi-square)
- Linear regression & correlation (simple and multiple OLS, residual diagnostics)

## Key findings
1. Traditional study hours are the strongest behavioural driver of GPA improvement (r ≈ 0.38).
2. *Quality beats quantity* — advanced prompt-engineers improve most (ANOVA, p ≈ 0).
3. Heavy AI use tracks dependency (r ≈ 0.66) and burnout.
4. A statistically significant paid-vs-free gap is practically negligible (Cohen's d ≈ 0.03) — *significant ≠ important*.

## Repository contents
| File | Description |
|------|-------------|
| `AI_Impact_on_Students_Statistics_Project.ipynb` | Main notebook (the report) |
| `ai_student_impact_dataset.csv` | Dataset |
| `README.md` | This file |

## ▶️ How to run
**Google Colab:** open the notebook, upload `ai_student_impact_dataset.csv` (or mount Drive), then *Runtime ▸ Run all*.

**Local:**
```bash
git clone https://github.com/Jp-Rsb/SDA_Group1_Team4.git
cd SDA_Group1_Team4
pip install pandas numpy matplotlib seaborn scipy statsmodels jupyter
jupyter notebook AI_Impact_on_Students_Statistics_Project.ipynb
```

## Team & responsibilities
| Member | Section |
|--------|---------|
| [Juan Pablo García](https://github.com/Jp-Rsb) | Introduction, problem definition, data loading & cleaning | 
| Doaa | Descriptive statistics, probability & distributions |
| Ana | Exploratory Data Analysis & visualization |
| Zaid | Hypothesis testing & confidence intervals |
| Ikram | Linear regression, correlation & conclusions |

---

