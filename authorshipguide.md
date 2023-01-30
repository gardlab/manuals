# Gard Lab Authorship Guidelines

This document describes the guidelines for determining authorship in the Gard Lab. The guidelines were informed by discussions among Gard Lab members (undergraduates, postbac staff, graduate students) during the Fall 2022 semester. Inspiration was drawn from the following sources: the Kosslyn lab (https://kosslynlab.fas.harvard.edu/files/kosslynlab/files/authorship_criteria_nov02.pdf), an article in Science (https://www.science.org/content/article/how-navigate-authorship-scientific-manuscripts), and the CRediT Taxonomy (https://credit.niso.org/). 

## Steps in Creating the Authorship Guidelines

1. All lab members ranked the 14 CRediT Contributor Roles on a Likert scale from 1 - 10, where 10 = most contribution and 1 = least contribution. Ratings were based on four criteria: skill, time, replaceability, creativeness. Definitions for each criteria were arrived through group consensus.

Skill = technical expertise
Replaceability = could you easily hire someone else to do this task
Creativeness = originality of thought/ideas
Time = balance of effort and efficiency. For example, a task is that straightforward but takes 100 hours could be high time and high replaceable

2. Dr. Gard calculated the Intra-Class Correlation for the ratings of the 14 CRediT Contributor Roles. A two-way random-effects model (ICC2) was calculated, which is appropriate for when the same raters evaluate each "item" (or in this case, contributor roles). The average ICC (i.e., across raters) was calculate. The ICC2 was calculated based on absolute agreement, which measures the extent to which different raters assign the same score to the same "item". 

> icc(authordf_transp,model="twoway",type="agreement",unit="average")
 Average Score Intraclass Correlation

   Model: twoway 
   Type : agreement 

   Subjects = 14 
     Raters = 13 
  ICC(A,13) = 0.875

 F-Test, H0: r0 = 0 ; H1: r0 > 0 
  F(13,155) = 8.62 , p = 4.79e-13 

 95%-Confidence Interval for ICC Population Values:
  0.754 < ICC < 0.952

> apply(authordf_small,2,median)
Conceptualization     Data-Curation 
               10                 6 
         Analysis           Funding 
                8                 6 
  Data-Collection       Methodology 
                7                 7 
    Project-Admin         Resources 
                5                 4 
         Software        Validation 
                4                 5 
    Visualization  Writing-Original 
                5                10 
  Writing-Editing       Supervision 
                6                 7 



