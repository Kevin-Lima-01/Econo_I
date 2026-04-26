# Unemployment and Suicide: A Cross-Section Analysis of Brazilian Municipalities

This repository contains the final project and supporting codes developed as part of a **Cross-Section Econometrics** course. The study explores the relationship between two variables of critical importance for mental health policy and unemployment mitigation: **suicide** and **unemployment**. Starting from a unidirectional causal hypothesis — that unemployment leads to suicide — the analysis examines this link across Brazilian municipalities in 2010, drawing on data from **IBGE**, **IPEA**, and **SUS**.

## Research Objective

The central goal is to empirically test whether municipal unemployment rates have a statistically significant effect on suicide rates. The study adopts a cross-sectional framework using data from all Brazilian municipalities for the year 2010, treating the municipal suicide rate as the dependent variable and the municipal unemployment rate as the key explanatory variable.

## Hypothesis

The analysis departs from a simple causal premise:

> *Higher unemployment rates increase financial distress, social exclusion, and psychological strain, thereby leading to higher suicide rates.*

The empirical strategy tests this hypothesis while remaining open to confounding factors, indirect effects, and potential non-linearities.

## Data Sources

The dataset is constructed from three official Brazilian sources:

| Source | Description |
|--------|-------------|
| **IBGE** | Brazilian Institute of Geography and Statistics — municipal socioeconomic and demographic indicators, including unemployment rates from the 2010 Census. |
| **IPEA** | Institute for Applied Economic Research — complementary municipal-level economic and social indicators. |
| **SUS** | Brazilian Unified Health System — municipal suicide mortality records (DATASUS) for the construction of suicide rates. |

- **Unit of Analysis:** Brazilian municipalities
- **Year:** 2010 (cross-section)

## Methodology

The empirical approach applies cross-sectional regression techniques to estimate the unemployment–suicide relationship:

| Step | Description |
|------|-------------|
| **1. Data Compilation** | Merging municipal-level data from IBGE, IPEA, and SUS into a unified cross-sectional dataset. |
| **2. Variable Construction** | Computing suicide rates per capita and unemployment rates at the municipal level. |
| **3. Model Specification** | Baseline OLS regression of suicide rate on unemployment rate with control variables. |
| **4. Diagnostic Testing** | Heteroskedasticity tests (Breusch-Pagan, White), normality checks, and outlier analysis. |
| **5. Robustness Checks** | Alternative specifications, sensitivity analysis, and discussion of indirect effects. |

## Key Findings

The results challenge the simple unidirectional hypothesis:

- The direct effect of unemployment on suicide is either **not statistically significant** or exhibits a **counterintuitive negative sign** — suggesting that, in the cross-section, higher unemployment is associated with *lower* suicide rates in some specifications.
- These findings do not necessarily refute the unemployment–suicide link but rather highlight the importance of:
  - **Indirect effects:** Unemployment may affect suicide through channels such as income loss duration, social safety nets, or stigma, which are not captured in a simple contemporaneous cross-section.
  - **Ecological fallacy:** Municipal-level aggregates may mask individual-level dynamics.
  - **Omitted variables:** Cultural, religious, and institutional factors that correlate with both unemployment and suicide.

> *The study concludes that the relationship between unemployment and suicide is more complex than a simple unidirectional causal chain, emphasizing the need for nuanced policy design that accounts for indirect mechanisms and contextual factors.*
