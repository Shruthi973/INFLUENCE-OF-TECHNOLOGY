# 📱 Impact of Technology Use on Academic Performance and Life Satisfaction Among Youth

## 🧠 Research Goal
To examine how technology usage affects academic performance (`EDUC`) and life satisfaction (`HAPPY`) among youth using the General Social Survey (GSS) dataset, while also considering the role of social determinants like age, race, sex, and income.


<p align="center">
  <img src="TECHNOLOGY.jpg" width="600"/>
  <br>
  <em>🧠 fNIRS brain mapping – Understanding neurophenotypes in Parkinson’s Disease</em>
</p>

---

## 🗝️ Key Variables

- **Dependent Variables**:
  - `EDUC`: Education level (Academic Performance)
  - `HAPPY`: Self-reported Life Satisfaction
  - `LifeSat`: Binary version of `HAPPY` (Very Happy = 1, others = 0)

- **Independent Variables**:
  - `USETECH`: Technology usage score
  - `AGE`, `SEX`, `RACE`, `MARITAL`, `WRKSTAT`, `RINCOME`, `HRS1`, `HRS2`

---

## 📊 Methodology

- Cleaned and recoded GSS 2018 data using R
- Missing values in `USETECH` replaced with mean
- Derived:
  - `USETECH_group` (High/Low based on median)
  - `LifeSat` (binary from `HAPPY`)
- Used summary statistics and plots to explore distributions

---

## 📈 Models and Tests Used

- **Descriptive Statistics & Visualizations**:
  - Bar plots: Education level, Happiness level
  - Scatter plots: `USETECH` vs `EDUC`, `USETECH` vs `HAPPY`
  - Histogram: Age distribution

- **Inferential Statistics**:
  - Independent Samples t-test (`EDUC`, `HAPPY` by `USETECH_group`)
  - Wilcoxon Test (non-parametric for `HAPPY`)
  - ANOVA and Kruskal-Wallis Tests (across `RACE`, `MARITAL`)
  - Tukey’s HSD (Post-hoc comparisons)
  - Cohen’s d (Effect sizes)

- **Predictive Models**:
  - Multiple Linear Regression: Predict `HAPPY`
  - Binary Logistic Regression: Predict `LifeSat`

---

## 🔍 Interpretation of Results

- **Academic Performance**:
  - Higher `USETECH` → Significantly higher `EDUC` (p < 0.00001, Cohen’s d = 0.20)
  
- **Life Satisfaction**:
  - No significant difference in `HAPPY` across `USETECH` groups
  - `AGE` positively predicted `LifeSat` (older = more likely Very Happy)
  - `RACE` (Black > White) positively associated with `HAPPY`

---

## ✅ Conclusion

Technology usage is associated with **higher academic attainment**, but **not directly linked** to higher life satisfaction. Social factors like **age** and **race** have stronger predictive value for happiness. This suggests a complex relationship between tech use and well-being that depends on broader social contexts.

---

## 📚 References

1. Lepp et al., 2014  
2. Moksnes et al., 2016  
3. Crede et al., 2015  
4. Żerebecki & Opree, 2022  
5. Sampasa-Kanyinga et al., 2022

---

