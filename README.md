# What, why and how

I completed an **Inferential Statistics** course from the University of Amsterdam (UvA) and wanted to apply what I learned to real data. I chose four simple questions about students and used a classic test to answer each one.

## Data

The **Student Performance dataset** from the [UCI repository](https://archive.ics.uci.edu/dataset/320/student+performance) contains data on 649 students from two schools in Portugal (Cortez & Silva, 2008). It includes their grades and background information such as sex, parents' education, study time, and absences.

15 students with a final grade of 0 were removed before the tests. They all had 0 absences, so the 0 most likely means they did not take the final exam (for example, they left school).

## Questions and answers

### Q1 · Do students who want higher education get better scores?

**Yes.** They score about 3 points higher on average (95% CI: 2.5 to 3.5). The difference is significant.

`t-test` · *d ≈ 1.36*

### Q2 · Does a mother's level of education affect her child's grades?

**Yes, but only a little.** It explains around 9% of the difference in grades. Grades go up slowly with the mother's education, and the biggest jump is in the highest education group.

`Welch's ANOVA` · *η² ≈ 0.09*

### Q3 · Do absences affect grades?

**Yes, but the effect is small.** More absences usually mean slightly lower grades, but the relationship is weak. Keeping the 15 students with a grade of 0 makes it look even weaker (r ≈ −0.09).

`Pearson ≈ −0.20` · `Spearman ≈ −0.21`

### Q4 · Is there a difference between boys and girls in wanting higher education?

**No real difference.** Both groups are very similar (91% vs 88%).

`chi-square`