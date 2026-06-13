# NSS, IIT ROORKEE

# Social Program Evaluation & Budget Optimization

A data-driven evaluation of a multi-intervention education program operating across 200 schools in Rajasthan. This project uses statistical modeling, cost-effectiveness analysis, and policy simulation to identify which interventions generate the highest learning outcomes per rupee spent and recommends an optimized budget allocation strategy for education in school.

---

## Project Objective

Many social programs combine multiple interventions without evaluating which components actually drive outcomes.

This project aims to:

- Quantify the impact of each intervention on student learning gains
- Control for confounding variables using regression analysis
- Compare interventions on a cost-effectiveness basis
- Recommend an evidence-based budget reallocation strategy
- Estimate projected improvements under the optimized allocation

---

## Program Evaluated

The education program consists of three interventions:

| Intervention | Purpose |
|-------------|----------|
| Mid-Day Meal (MDM) | Improve attendance and nutrition |
| Remedial Teaching | Provide targeted learning support |
| ASHA Health Visits | Reduce health-related absenteeism |

**Geography:** Rajasthan, India

**Coverage:** 200 Schools across 5 districts

---

## Methodology

### Outcome Variable

Learning improvement measured as:

```
Score Gain = Endline Score − Baseline Score
```

### Statistical Model

Ordinary Least Squares (OLS) Regression:

```
Score_Gain =
β₀ +
β₁(Remedial) +
β₂(MDM) +
β₃(ASHA) +
β₄(Baseline Score) +
β₅(Teacher Ratio) + ε
```

### Confounders Controlled

- Baseline Assessment Score
- Teacher–Pupil Ratio

---

## Tech Stack

- Python
- Pandas
- NumPy
- Statsmodels
- OpenPyXL
- Jupyter Notebook

---

## Project Structure

```
├── SocialProgram_Evaluation.ipynb      # Complete analysis notebook
├── SocialProgram_Evaluation.xlsx       # Dataset + model outputs
├── SocialProgram_EvaluationReport.docx # Final policy report
├── Optimizing_Education_ROI.pptx       # Executive presentation
└── README.md
```

---

## Key Findings

### Regression Results

| Intervention | Effect Size | Significance |
|-------------|------------|--------------|
| Remedial Teaching | +5.36 points | p < 0.001 |
| Mid-Day Meal | +3.32 points | p < 0.001 |
| ASHA Visits | +1.12 points | p = 0.013 |

### Interpretation

- **Remedial Teaching** emerged as the strongest predictor of learning gains.
- Schools implementing remedial classes achieved an average improvement of **5.36 additional score points**.
- Mid-Day Meals generated meaningful improvements but at a substantially higher cost.
- ASHA Health Visits produced positive but smaller effects.

---

## Cost-Effectiveness Analysis

| Intervention | Cost per School | Score Gain | Score Gain per ₹1000 |
|-------------|---------------|------------|----------------------|
| Remedial Teaching | ₹42.3K | +5.36 | 0.127 |
| ASHA Visits | ₹18.2K | +1.12 | 0.064 |
| Mid-Day Meal | ₹85.2K | +3.32 | 0.039 |

### Ranking

 Remedial Teaching

 ASHA Health Visits

 Mid-Day Meal

Remedial Teaching was found to be:

- **3.3× more cost-effective** than Mid-Day Meals
- **2× more cost-effective** than ASHA Visits

---

## Budget Optimization Strategy

### Current Budget

₹24.94 Million

### Recommendation

Reallocate approximately:

```
₹3.214 Million
(12.9% of total budget)
```

from lower-ROI budget lines toward expanding remedial teaching coverage.

### Coverage Expansion

| Metric | Current | Proposed |
|----------|----------|----------|
| Schools with Remedial Classes | 108 | 184 |
| Coverage | 54% | 92% |

---

## Projected Impact

| Outcome | Current | Optimized |
|----------|----------|----------|
| Average Score Gain | 2.38 | 4.11 |
| Schools with Positive Gains | 54% | 78% |
| Cost per Score Point | ₹334K | ₹194K |

### Expected Benefits

- +72.7% improvement in learning outcomes
- 42% reduction in cost per score point
- Significant expansion of high-impact interventions without increasing total budget

---

## Limitations

This analysis uses observational data and therefore does not establish causality.

Potential limitations include:

- Selection bias
- Unobserved confounders
- Non-random intervention assignment
- District-level heterogeneity

Future validation should include:

- Difference-in-Differences (DiD)
- Randomized Controlled Trials (RCTs)
- Instrumental Variable approaches

---

## Policy Recommendation

The evidence strongly suggests that prioritize **Remedial Teaching** as the highest-return on educational investment.

Rather than increasing overall expenditure, policymakers can improve learning outcomes by reallocating existing resources toward interventions with the highest demonstrated impact per rupee spent.

---

## References

- J-PAL South Asia
- Pratham – Teaching at the Right Level (TaRL)
- 3ie Evidence Gap Maps
- IRIS+ Framework

---

## Author

- Krish Goyal 23113086
- Ekansh Shakya 23113054
- Hemant Bhakar 23113066
- Himanshu Yadav 23113070
- Rohit Yadav 2311903

Data Analytics | Econometrics | Social Impact Evaluation
 
