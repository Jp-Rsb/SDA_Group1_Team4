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

## Methods applied (course workflow)
1. **General information & cleaning** — `describe()`, `info()`, missing values, duplicates, `fillna` (mean / mode)
2. **Distribution & probability** — Shapiro-Wilk normality test, normal model (`norm.cdf`, `norm.ppf`), empirical vs. theoretical probabilities
3. **Exploratory Data Analysis** — correlation heatmap, boxplots, bar charts, scatter plots
4. **Hypothesis testing** — independent samples (Welch *t* / Mann-Whitney), paired samples (paired *t* / Wilcoxon), one-way ANOVA
5. **Machine learning** — Logistic Regression & Random Forest to classify burnout risk, with accuracy, F1, confusion matrix and feature importance

## Key findings
1. Traditional study hours are the strongest habit linked to GPA improvement (r ≈ 0.38).
2. *Quality beats quantity* — advanced prompt-engineers improve most (ANOVA, p < 0.05).
3. Heavy AI use goes with higher perceived dependency (r ≈ 0.66) and is the top predictor of burnout.
4. The paid-vs-free gap is statistically significant but tiny — *significant ≠ important*.
5. Burnout can be predicted only moderately (accuracy ≈ 0.53 vs. 0.42 baseline) — honest limits matter.

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
pip install pandas numpy matplotlib seaborn scipy scikit-learn jupyter
jupyter notebook AI_Impact_on_Students_Statistics_Project.ipynb
```

## Team & responsibilities
| Member | Section |
|--------|---------|
| [Juan Pablo García](https://github.com/Jp-Rsb) | Import, general information & cleaning |
| Doaa | Descriptive statistics, distribution & probability |
| [Ana Rodriguez](https://github.com/anitar1412) | Exploratory data analysis (charts) |
| [Zaid](https://github.com/zaiddely) | Hypothesis testing |
| Ikram | Machine learning & conclusions |

---

