# Gard Lab Authorship Guidelines

This document describes the guidelines for determining authorship in the Gard Lab. The guidelines were informed by discussions among Gard Lab members (undergraduates, postbac staff, graduate students) during the Fall 2022 semester. Inspiration was drawn from the following sources: [the Kosslyn lab](https://kosslynlab.fas.harvard.edu/files/kosslynlab/files/authorship_criteria_nov02.pdf), an article in [Science](https://www.science.org/content/article/how-navigate-authorship-scientific-manuscripts), and [the CRediT Taxonomy](https://credit.niso.org/). 

## Steps in Creating the Authorship Guidelines

1. All lab members ranked the 14 CRediT Contributor Roles on a Likert scale from 1 - 10, where 10 = most contribution and 1 = least contribution. Ratings were based on four criteria: skill, time, replaceability, creativeness. Definitions for each criteria were arrived through group consensus.

Skill = technical expertise
Replaceability = could you easily hire someone else to do this task
Creativeness = originality of thought/ideas
Time = balance of effort and efficiency. For example, a task is that straightforward but takes 100 hours could be high time and high replaceable

2. Dr. Gard calculated the Intra-Class Correlation for the ratings of the 14 CRediT Contributor Roles. A two-way random-effects model (ICC2) was calculated, which is appropriate when the same raters evaluate each "item" (or in this case, contributor roles). The average ICC (i.e., across raters) was calculate. The ICC2 was calculated based on absolute agreement, which measures the extent to which different raters assign the same score to the same "item". 

**Calculate the ICC**
```
icc(authordf_transp,model="twoway",type="agreement",unit="average")
```
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

**Print the Median Rating for Each Category**
```
apply(authordf_small,2,median)
```
Conceptualization  10      
Data-Curation      6   
Analysis           8           
Funding            6  
Data-Collection    7         
Methodology        7  
Project-Admin      5           
Resources          4   
Software           4  
Validation         5   
Visualization      5  
Writing-Original   10   
Writing-Editing    6         
Supervision        7   

3. Based on the average rating for each of the 14 CRediT Contributions, Dr. Gard assigned a point value to each category. The following "default" point values total to 1450. The total points for each phase are divided among authors in proportion to their contribution in that phase of the project. In my lab, if someone contributed more than 0 but less than 10% of the total number of points, they are acknowledged in the footnote. If they contributed at least 10%, they are an author, and the ordering of authorship is determined by the relative number of points. Below are the median ratings, assigned point values, and definitions for each of the 14 CRediT categories. Dr. Gard's edits to the CRediT Contribution definitions are in *italics*. 

* **Writing-Original**: Median Rating = 10; Assigned Point Value = 250. Definition = Preparation, creation and/or presentation of the published work, specifically writing the initial draft (including substantive translation). *This point value is larger than the "Conceptualization" contribution oweing to the amount of time needed to write the original draft of a manuscript*
* **Conceptualization**: Median Rating = 10; Assigned Point Value = 200. Definition = Ideas; formulation or evolution of overarching research goals and aims. *Feedback on an idea, particularly if it occurs only in the context of a lab meeting, is not sufficient to warrant "Conceptualization".*
* **Analysis**: Median Rating = 8; Assigned Point Value = 150. Definition = Application of statistical, mathematical, computational, or other formal techniques to analyse or synthesize study data. *In cases where the analytic plan is simple (e.g., a correlation table), the point value for this category may be adjusted.*
* **Data Collection**: Median Rating = 7; Assigned Point Value = 100. Definition = Conducting a research and investigation process, specifically performing the experiments, or data/evidence collection. *To be eligible for this contribution, an individual must be actively collecting data for at least two semesters of the project OR for the duration of the project (whichever comes first). 
* **Methodology**: Median Rating = 7; Assigned Point Value = 100. Definition = Development or design of methodology; creation of models. *This contribution is similar to the "Analysis" contribution, but can be distinguished by developing the methodology versus running the analyses.*  
* **Supervision**: Median Rating = 7; Assigned Point Value = 100. Definition = Oversight and leadership responsibility for the research activity planning and execution, including mentorship external to the core team.
* **Data Curation**: Median Rating = 6; Assigned Point Value = 75. Definition = Management activities to annotate (produce metadata), scrub data and maintain research data (including software code, where it is necessary for interpreting the data itself) for initial use and later re-use. *In cases where the data cleaning is substantial (e.g., neuroimaging data), the point value for this category may be adjusted.*
* **Funding**: Median Rating = 6; Assigned Point Value = 75. Definition = Acquisition of the financial support for the project leading to this publication.
* **Writing-Editing**: Median Rating = 6; Assigned Point Value = 75. Definition = Preparation, creation and/or presentation of the published work by those from the original research group, specifically critical review, commentary or revision – including pre- or post-publication stages.
* **Visualization**: Median Rating = 5; Assigned Point Value = 75. Definition = Preparation, creation and/or presentation of the published work, specifically visualization/data presentation. *Feedback on visual aides is not sufficient*
* **Validation**: Median Rating = 5; Assigned Point Value = 75. Definition = Verification, whether as a part of the activity or separate, of the overall replication/reproducibility of results/experiments and other research outputs.
* **Project Administration**: Median Rating = 5; Assigned Point Value = 75. Definition = Management and coordination responsibility for the research activity planning and execution.
* **Software**: Median Rating = 4; Assigned Point Value = 50. Definition = Programming, software development; designing computer programs; implementation of the computer code and supporting algorithms; testing of existing code components.
* **Resources**: Median Rating = 4; Assigned Point Value = 50. Definition = Provision of study materials, reagents, materials, patients, laboratory samples, animals, instrumentation, computing resources, or other analysis tools.

Additional Notes:
* All of the 14 CRediT Contributions will not be relevant for all projects (e.g., there is no data collection for secondary data analysis papers). Thus, the total possible point value for each project may not always equal 1450.
* To be an author on any manuscript from the Gard Lab, each contributor must agree to provide approve the manuscript. Approval is expected within 2 weeks, unless otherwise agreed upon. 
* In cases where a contributor changes instituitions, it is their responsibility to provide the first author or senior author with updated contact information. If the contributor cannot be reached within a reasonable amount of time, they forfeit their authorshp. The first author or senior author must may every attempt to notify them.
* If a contributor leaves UMD but made substantial contributions to a project from which multiple manuscript may arise, they will be included as an author on at least 1 manuscript after their departure. The first or senior author may invite such previous lab affiliates to be manuscript contributors at their discretion. 
* The point values outlined above are default point values. For any given project, the point values for each contribution may be adjusted depending on how much time each contribution is likely to take, the complexity of the responsibility, etc.
* The first and last author must decide together on which categories are relevant for a project, and whether the default point value should be adjusted, at the start of the project where possible.  


