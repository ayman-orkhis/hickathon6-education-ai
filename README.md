# Curriculum Compass — Team 11  

### Performance in the Hi!ckathon #6 Competition  
We ranked 17th out of 69 teams on the official leaderboard for the regression task, achieving an R² = 0.78, demonstrating the robustness and competitiveness of our predictive modeling pipeline.

---

## 1. Problem Overview

Many students finish compulsory schooling without mastering key mathematical concepts.  
Misunderstandings accumulate unnoticed, teachers only see local difficulties, and ministries rely on aggregate exam results that hide conceptual issues.

Additional challenges include:

- Unequal access to academic support  
- Lack of curriculum-aligned AI tools  
- Employers relying on credentials instead of observable skills  

Curriculum Compass addresses these systemic issues by combining AI tutoring, predictive analytics, and national-scale learning insights.

---

## 2. Dataset Description

We used a unified dataset combining the 2015, 2018, and 2022 PISA cycles, containing:

- Approximately 1.7 million student samples  
- More than 250 engineered numerical features  
- Variables grouped into themes such as:  
  - Learning habits  
  - Family and socioeconomic background  
  - School climate  
  - Item-level behaviour (scores and response times)

### Task 1 — Regression  
Predict each student's MathScore using survey-based and behavioural features.

### Task 2 — Innovation  
Design an AI-powered educational solution leveraging insights from the dataset.

---

## 3. Our Modeling Approach

### 3.1 Preprocessing

We built a robust data cleaning pipeline:

- Removed features with more than 80% missing values  
- Prevented data leakage by excluding variables containing target-related averaged scores  
- Consolidated redundant features to reduce dimensionality and improve interpretability  

---

### 3.2 Model Selection

We tested multiple gradient boosting models optimized for tabular data:

- XGBoost — Best performing model  
- LightGBM — Very fast training  
- CatBoost — Strong categorical handling  
- Hybrid ensemble (experimental) combining all three  

---

### 3.3 Hyperparameter Tuning

We used two optimization strategies:

- GridSearchCV for exhaustive search  
- Optuna for Bayesian optimization  

These techniques improved model performance, stability, and generalization.

---

## 4. Insights and Results

Our final model identified several important predictors of mathematical performance:

- Student engagement  
- School environment  
- Family background  
- Cognitive behaviours (response times, attempt patterns)

Future improvements include:

- Feature scaling  
- Advanced imputation  
- Interaction feature creation  

---

## 5. Innovation: Curriculum Compass

Beyond prediction, we developed a complete AI platform concept.

### Student Companion  
A curriculum-aligned AI tutor that provides:

- Reliable explanations  
- Adaptive difficulty  
- Consistent alignment with national standards  

### Curriculum Insights Dashboard  
Aggregates anonymised student questions into:

- Misunderstanding heatmaps  
- Topic difficulty trends  
- Class, school, and country-level analytics  

This intelligence helps teachers, ministries, and researchers continuously improve educational systems.

---

## Hi!ckathon Requirement

This project was developed for Hi!ckathon #6 – AI & Education.  
Please reference the official Hi!ckathon GitHub repository.

---

## Conclusion

Our solution transforms AI from a simple tutoring tool into national educational infrastructure.  
By combining predictive modeling with aligned LLM tutoring and curriculum analytics, Curriculum Compass can:

- Improve learning outcomes  
- Reduce inequality  
- Support teachers  
- Modernize curriculum design  
- Strengthen connections to the labour market  

---
