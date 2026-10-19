<div align="center">

# 🍱 Beyond the Mess Tray
### *An Empirical & Econometric Study on Campus Dining Habits, Peer Contagion, and Student Expenditure*

[![BAMAT207](https://img.shields.io/badge/Course-BAMAT207%20Stats-3B82F6?style=for-the-badge&logo=google-classroom&logoColor=white)](https://github.com)
[![Dataset](https://img.shields.io/badge/Sample%20Size-N%20%3D%20208-10B981?style=for-the-badge&logo=google-sheets&logoColor=white)](https://github.com)
[![R Studio](https://img.shields.io/badge/R%20Script-Verified-276DC3?style=for-the-badge&logo=r&logoColor=white)](https://github.com)
[![License: MIT](https://img.shields.io/badge/License-MIT-F59E0B?style=for-the-badge)](https://opensource.org/licenses/MIT)

<br/>

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1000&color=2563EB&center=true&vCenter=true&random=false&width=750&lines=208+Campus+Responses+Modeled;X+~+Binomial(14%2C+p+%3D+0.326)+Meal+Abandonment;Chi-Square+Test+of+Independence%3A+p+%3C+0.0001;Regression%3A+Each+%2B1+Rating+Saves+%E2%82%B9175.64%2Fwk" alt="Typing SVG" />

<p align="center">
  <b>A real-world investigation evaluating whether hostel mess quality and the "roommate ordering effect" systematically drain student budgets.</b>
</p>

[Explore Dataset](#-dataset-architecture--class-midpoints) • [Hypothesis Tests](#-empirical-hypothesis-testing) • [Regression Model](#-econometric-regression-model-theme-4) • [Web Application](#-interactive-web-application) • [Literature Benchmarks](#-literature-review--benchmarks)

---

</div>

## 📌 Executive Summary

Institutional university hostels mandate fixed, prepaid dining contracts, yet students routinely substitute hall meals with food deliveries, retail canteen snacks, and midnight tuck-shop runs. 

This project demonstrates all core modules of **BAMAT207 (Probability & Applied Statistics)** using an empirical primary sample of **$N = 208$ student responses** benchmarked against peer-reviewed literature from the *International Journal for Multidisciplinary Research* (IJFMR) and the *International Hospitality Review* (Emerald).

### Live Deployment link: https://campus-dining-statistical-study.vercel.app/

<div align="center">

| Metric | Empirical Value | Statistical Interpretation |
| :--- | :---: | :--- |
| **Average Weekly Outside Spending ($\bar{Y}$)** | **₹685.82** | Substantial right-skewness; modal baseline matches national college spending. |
| **Average Weekly Meal Skips ($\bar{X}_1$)** | **4.56 / 14 meals** | **1 in 3 prepaid mess meals is abandoned** for outside food. |
| **Average Mess Satisfaction Rating ($\bar{X}_2$)** | **2.91 / 5.00** | Neutral-to-negative satisfaction directly accelerates outside spending. |
| **Estimated Meal Skip Probability ($\hat{p}$)** | **0.3259 (32.6%)** | Modeled via discrete Binomial distribution $X \sim B(14, 0.326)$. |
| **Explained Spending Variance ($R^2$)** | **42.0% ($p < 0.0001$)** | Skipped meals and perceived food quality explain nearly half of all spending shifts. |

</div>

---


### 🎯 Key Highlights & Statistical Tests Covered:
- **Descriptive Statistics & Dispersion**: Class midpoint transformations, skewness, and Pearson correlation matrices ($r = +0.618, -0.483, -0.509$)[cite: 48].
- **Discrete Probability Distribution**: Fitting a Binomial Distribution $X \sim B(n=14, \hat{p}=0.326)$ to weekly skipped meals[cite: 48].
- **Parametric Hypothesis Testing**: One-Sample $t$-test against published national benchmarks ($\mu_0 = \text{₹}750/\text{wk}$, $p = 0.196$) and Welch Two-Sample $t$-test (Hostelers vs. Day Scholars, $df = 6.13, p = 0.051$)[cite: 48].
- **Categorical Association**: $4 \times 3$ Chi-Square ($\chi^2$) Test of Independence ($\chi^2 = 33.28, p < 0.0001$) confirming the "Roommate Domino Effect"[cite: 48].
- **Multiple Linear Regression (OLS)**: Econometric spending formula $\hat{Y} = 694.84 + 110.18\,X_1 - 175.64\,X_2$ ($R^2 = 0.420, F = 74.30$)[cite: 48].
- **Design of Experiments**: One-Way ANOVA across 4 dining arrangement treatments ($F = 6.780, p = 0.00022$) with Tukey HSD post-hoc evaluation[cite: 48].

### 📖 Literature Review & Benchmarks:
1. **Saikia & Sarmah (2025)** — *IJFMR*, Paper ID 53179 (National modal spending $\mu_0 = \text{₹}750/\text{wk}$)[cite: 48].
2. **Seo & Shanklin (2019)** — *International Hospitality Review* (Emerald) (Baseline meal skip probability $p_0 = 0.42$)[cite: 48].
3. **Ismail & Ahmad (2022)** — *Journal of Statistical Modeling and Analytics* ($r = 0.68$ peer & food quality correlation)[cite: 48].
