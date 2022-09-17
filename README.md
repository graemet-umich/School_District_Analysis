# PyCitySchools with Pandas
Repeat the school district analysis with omitted Thomas High School 9th grade scores.

## Overview

The school board suspects that the math and reading scores for Thomas High School 9th graders may have been altered. To uphold state-testing standards, remove the Thomas High School 9th grade scores and rerun the school district analysis. Compare this new school district analysis with the previous one and determine what changes, if any, occurred.

## Results

The results are a comparison between the school district analysis before and after removing the Thomas High School 9th grade math and reading scores.

![Before](./Images/ths9_nan.png)
Sample of Thomas High School 9th grader math and reading scores after being replaced by `NaN`s.

---

- The district summary was only minorly affected for average math score, which reduced by 0.1 points after removal (actually 0.055 points looking at unrounded data not shown here). This difference is negligible.

![Before](./Images/district_summary.png)
District Summary before removal

<br>

![After](./Images/district_summary_a.png)
District Summary after removal

---
- The school summary was unaffected except for Thomas High School where the passing math percentage went down by 0.09%, the passing reading percentage went down by 0.29%, and the overall passing percentage went down by 0.32%. These differences are negligible.

![Before](./Images/per_school_summary.png)
School Summary before removal

<br>

![After](./Images/per_school_summary_a.png)
School Summary after removal

---

- The ranking of Thomas High School as the second highest performing school remained unchanged. The rankings of the top and bottom 5 schools by overall passing percentage are shown.

![Before](./Images/top5.png)
School Summary Top 5 before removal

<br>

![After](./Images/top5_a.png)
School Summary Top 5 after removal

<br>

![Before](./Images/bottom5.png)
School Summary Bottom 5 before removal

<br>

![After](./Images/bottom5_a.png)
School Summary Bottom 5 after removal

---

- The average math and reading scores by grade level by school are identical except where the Thomas High School 9th scores are replaced by `nan`.

| Average Math Scores | |
| :--- | :--- |
| ![Before](./Images/math_scores_by_grade.png) | ![After](./Images/math_scores_by_grade_a.png) |
| Before removal | After removal |

| Average Reading Scores | |
| :--- | :--- |
| ![Before](./Images/reading_scores_by_grade.png) | ![After](./Images/reading_scores_by_grade_a.png) |
| Before removal | After removal |

---

- Scores by school spending remained unchanged. Thomas High School is in the $631-$645 bracket.

![Before](./Images/spending_summary.png)
School Spending Summary before removal

<br>

![After](./Images/spending_summary_a.png)
School Spending Summary after removal

---

- Scores by school size remained unchanged. Thomas High School is a medium sized school.

![Before](./Images/scores_by_school_size.png)
School Size Summary before removal

<br>

![After](./Images/scores_by_school_size_a.png)
School Size Summary after removal

---

- Scores by school type remained unchanged. Thomas High School is a charter school.

![Before](./Images/scores_by_school_type.png)
School Type Summary before removal

<br>

![After](./Images/scores_by_school_type_a.png)
School Type Summary after removal


## Summary

Upon removing (replacing with `NaN`s/`nan`s) the Thomas High School 9th grade math and reading scores, the district summary and school summary showed negligible differences. There was no difference in school ranking (#2), the scores by school spending, scores by school size, or scores by school type.

Moreover, the Thomas High school 9th grade average math and reading scores are in line with those of the Thomas High School 10th, 11th, and 12th graders.

The conclusion is that there is no evidence of academic dishonesty at Thomas High School through 9th grade math and reading score tampering.


