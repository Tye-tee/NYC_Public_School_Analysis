# NYC Schools SAT Performance Analysis

A hands-on data science practice project to explore SAT performance across NYC high schools using Python, Pandas, and Matplotlib. This project helps identify which schools and boroughs are excelling, and where variation in scores suggests deeper insights.

---

## What’s Inside

- Data cleaning, filtering, and aggregation using Pandas  
- Analysis of average Math, Reading, Writing scores and combined Total SAT  
- Identification of high-performing schools by Math and Total SAT  
- Borough-level analysis: mean, standard deviation, and spread of scores  
- Visualization: boxplots to compare performance distributions across boroughs

---

## Features

- Calculate best performing schools in Math (threshold-based)  
- Compute combined SAT (Math + Reading + Writing) and rank top 10 schools  
- Detect the borough with highest variance in Total SAT scores  
- Visual comparison of score distributions by borough  
- Clear, reproducible Python scripts with well-documented steps

---

## Tools & Techniques Used

- **Python** (Pandas for data manipulation)  
- **Matplotlib** for plotting and visual interpretation  
- Pandas functions: `groupby`, `agg`, `sort_values`, `filtering`, new column creation  
- Statistical measures: mean, standard deviation, count, etc.  
- Data cleaning & validation: handling missing values, ensuring consistency

---

## Problem & Business Impact

Many education stakeholders need accessible, clear insights into how different schools and boroughs are performing with respect to SAT scores. Static snapshots often hide variation and inequity. This analysis provides tools to:

- Highlight schools with top performance in Math and overall SAT  
- Identify boroughs with large disparities in performance, potentially pointing to unequal access or resources  
- Inform policy makers, education administrators, or community organizations looking to improve outcomes or allocate support

---

## Analysis Workflow

1. **Data Import & Preview**  
   - Load the dataset `schools.csv` and inspect for missing or anomalous data.

2. **Math Performance Filter**  
   - Filter schools by average Math ≥ 640, sort descending to find top Math performers.

3. **Combined SAT Scores**  
   - Add `total_SAT = average_math + average_reading + average_writing`  
   - Sort and extract top 10 schools by `total_SAT`.

4. **Borough-Level Variance**  
   - Group by `borough`, aggregate count, mean, standard deviation of `total_SAT`  
   - Identify the borough with the highest standard deviation.

5. **Visualization**  
   - Create boxplot of `total_SAT` distribution by borough to visually compare spread and medians.

---

## Key Findings

- Schools with **high Math scores** (≥640) cluster among top performers.  
- The **Top 10 schools by combined SAT** significantly outperform the rest of the city.  
- One borough showed notably larger variation in `total_SAT`, suggesting uneven performance distribution.  
- Boxplot visualizations confirm that boroughs differ not just in average scores but in score spread—some consistent, others very spread out.

---

## Next Steps

- Expand dataset to include socioeconomic or resource factors (e.g. funding, teacher-student ratio) for deeper correlation analysis.  
- Build interactive dashboard (Tableau or Power BI) to allow users to filter by borough, or school type.  
- Apply statistical testing (e.g. ANOVA) to test significance of differences among boroughs.  

