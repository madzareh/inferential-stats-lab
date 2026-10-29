# Inferential Stats Lab

I completed an inferential statistics course from the University of Amsterdam and wanted to apply what I learned to real data. Here I look at four questions about students in two Portuguese schools.

## Data

The data is the Portuguese class part of the [Student Performance dataset](https://archive.ics.uci.edu/dataset/320/student+performance) on UCI (Cortez & Silva, 2008). It has 649 students. Grades go from 0 to 20, and G3 is the final grade.

15 students have a final grade of 0. All of them have 0 absences and a first-period grade between 4 and 11, so the 0 most likely means a missed final exam. I left them out of the tests, which leaves 634 students.

## Results

| | Question | Test | Answer |
|---|---|---|---|
| Q1 | Do students who want higher education get better scores? | Welch t-test | Yes, about 3 points higher (95% CI 2.5 to 3.5, d ≈ 1.36) |
| Q2 | Do students with more educated mothers get better grades? | Welch's ANOVA | A little (η² ≈ 0.09), with the biggest jump in the highest group |
| Q3 | Do students with more absences get lower grades? | Pearson, Spearman | Yes, but it's weak (r ≈ −0.20) |
| Q4 | Is there a difference between boys and girls in wanting higher education? | Chi-square | No significant difference (91% vs 88%, p = 0.11) |

Q3 changed the most when the zeros were removed. With them, r is only −0.09: they all have 0 absences and a grade of 0, so they pull the line flat.

For Q4, the 95% CI of the gap is about −1 to 9 percentage points, so a small difference is still possible.

## Limitations

Q1 and Q3 are both significant, but the effect in Q1 is large and in Q3 it's small, so the p-value alone doesn't say much. Since the data is observational and comes from only two schools in one country, the results show associations in this sample and may not hold elsewhere.