# What and Why

I completed an **Inferential Statistics** course from the University of Amsterdam (UvA) and wanted to apply what I learned to real data. I chose four simple questions about students and used a classic test to answer each one.

## Data

The **Student Performance dataset** from the [UCI repository](https://archive.ics.uci.edu/dataset/320/student+performance) contains data on 649 students from two schools in Portugal (Cortez & Silva, 2008). It includes their grades and background information such as sex, parents’ education, study time, and absences.

## Questions and Answers

Q1. Do students who want higher education get better scores?

* Yes. They score about 3.5 points higher on average. The difference is significant. (t-test, d ≈ 1.15)

Q2. Does a mother’s level of education affect her child's grades?

* Yes, but only a little. It explains around 6% of the difference in grades, and the effect is mostly visible in the highest education group. (ANOVA, η² ≈ 0.06)

Q3. Do absences affect grades?

* Yes, but the effect is very small. More absences usually mean slightly lower grades, but the relationship is weak. It’s not a clear straight-line pattern. (Pearson ≈ −0.09, Spearman ≈ −0.16)

Q4. Is there a difference between boys and girls in wanting higher education?

* No real difference. Both groups are very similar (91% vs 87%). (chi-square test)