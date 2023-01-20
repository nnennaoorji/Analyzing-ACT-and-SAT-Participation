# Analyzing ACT and SAT Participation by State Policy


### Problem Statement 

Following recent debates on the use of the SAT and ACT tests in determining college readiness, the South Carolina State Board of Education is re-assessing its policy stance on the issue. Currently, the State does not require its highschoolers to sit for either the SAT or the ACT, but provides funding to enable 11th graders take either test for free. The State has hired me as a consultant to profer an answer to the question:

**Will making the SAT or ACT mandatory have any effect on the State's average test scores?**

### Executive Summary

Effort has gone into researching the link between states' participation rate and average performance in both the SAT and ACT. These studies largely suggest a negative relationship between the two variables, wherein average performance by a state in a test tends to drop, as participation increases. This has been explained by the tendency for participation in a given test to increase when a test is made mandatory and/or provided for free by the state. A mandatory test also often implies that the test/test resources will be free and/or subsidized, leading to a larger and more diverse pool of candidates. In contrast, a low participation rate often implies that the candidate pool is less diverse, and usually more academically sound. This is because students who take the non-mandatory test (especially in addition to mandatory tests) tend to be "high acheivers", not indigent, and/or have access to more opportunities (Dargan, 2020).

Studies have also shown a negative correlation between the SAT and the ACT, whereby a student who takes the SAT is not likely to take the ACT. Both exams have also been shown to be quite similar in terms of aim/objective, difficulty level and overall structure. In order words, it makes sense to just take one of these exams, except a student is an over-acheiver and/or is applying to multiple schools which require/accept one or both.

Importantly, states tend to deploy significant amount of resources aimed at making the test more accessible and aiding students to be successful, especially in contexts where the test is mandatory. While we understand the relationship between participation and succeess rate, it will be interesting to analyse success rate by distinguishing between states where the SAT is required, states where the ACT is required, states which require at least one of the tests, and states where neither test is required. The aim is to ascertain whether relavant information can be obtained on the link between participation and student success, while controlling for a significant factor which affects participation (state policy). 

#### Background

The SAT and ACT are popular standardized tests that several colleges and universities in the United States use to assess a student's college readiness and aptitude. As at 2020, more than half of the United States' 50 states required high school seniors to have taken either the SAT or the ACT as a prerequisite for graduation. However, this statistic is evolving with recent evidence that shows that standardized tests such as the SAT or ACT may favour privileged segments of the population, at the expense of minority and less privileged students. Supporters of standardized tests, however, argue that it remains the one objective parameters that places all college applicants on a level playing field, thus allowing all student populations a fair chance at compteting for college admissions. Importantly, both tests are fundamentally similar in terms of aim/objective and difficulty level. As such, a student who does well on the ACT should fare just as well on the SAT and vice versa.

State policy on standardized tests vary from state to state. Some states require the SATs, while some others require the ACTs, In some states students must take either of the exam, whereas in others, neither of the tests is required. More so, in some "test optional" states, one or both of the tests are provided to interested students for free. As at 2020, 9 states required the SAT, 14 states required the ACT, and 3 states- Ohio, Idaho and Tennessee required students to take either the ACT or the SAT. Washington D.C and South Carolina are examples of states where neither test is mandatory, but provided for free to interested students.


### Conclusion
This analysis sought to answer the question "Will making the SAT or ACT mandatory have any effect on the State of South Carolina's average test scores? The answer to this question is **Yes** and the likely nature of this relationship is negative. This is premised, primarily, on the observed negative association between participation rate and avarage tests scores, and the positive association between participation rates and a "test mandatory" policy stance. Key findings from the analysis are listed below:

> 1. Average test scores of a test are lowest in states where that test is mandatory and highest in states where the alternative test is mandatory.

> 2. States that do not require either of the tests generally outperform states that require students to take at least one of them.

> 3. In some cases, states with an "either or" policy recorded higher median SAT sectional scores than "test optional" states.

> 4.It is possible to record over 50% participation in both tests even when one of the tests is mandatory in the state. Surpisingly, none of the states which require either the SAT or the ACT met this criteria.

> 5. Despite having a "test optional" policy stance and providing both exams for free to interested students, the state of South Carolina scored below the national average in both the ACT and SAT across the three years studied.

> 6. A strong, positive correlation was observed between average scores on the SAT Math and Evidence-Based Reading and Writing Sections.

### Recommendations
> 1.  Findings of the analysis suggest that states concerned with raising average test scores are likely better off having a test optional policy stance. The state can therefore retain its current policy stance.

> 2. There is need for deeper analysis into uncovering the reason for below average test scores in the State. The positive correlation observed between the two sections on the SAT suggest that efforts to increase average test scores need to be holistic, and not necessarily targeted to specific sections of the test. 

### Data

In addressing the problem statement, this study analysed ACT and SAT data for the 50 states in the United States, spanning the period 2017 to 2019. The ACT dataset utilized includes information on states' participation rates and composite (average) ACT scores, while the SAT dataset contains information on state's participation rates and average scores, including a breakdown of scores by section i.e. Maths and Evidence-Based Reading and Writing (EBRW). These datasets are referenced and linked below:

* [`act_2017.csv`](./data/act_2017.csv): 2017 ACT Scores by State ([source](https://blog.prepscholar.com/act-scores-by-state-averages-highs-and-lows))
* [`act_2018.csv`](./data/act_2018.csv): 2018 ACT Scores by State ([source](https://blog.prepscholar.com/act-scores-by-state-averages-highs-and-lows))
* [`act_2019.csv`](./data/act_2019.csv): 2019 ACT Scores by State ([source](https://blog.prepscholar.com/act-scores-by-state-averages-highs-and-lows))
* [`act_2019_ca.csv`](./data/act_2019_ca.csv): 2019 ACT Scores in California by School ([source](https://www.cde.ca.gov/ds/sp/ai/) | [data dictionary](https://www.cde.ca.gov/ds/sp/ai/reclayoutact19.asp))
* [`sat_2017.csv`](./data/sat_2017.csv): 2017 SAT Scores by State ([source](https://blog.collegevine.com/here-are-the-average-sat-scores-by-state/))
* [`sat_2018.csv`](./data/sat_2018.csv): 2018 SAT Scores by State ([source](https://blog.collegevine.com/here-are-the-average-sat-scores-by-state/))
* [`sat_2019.csv`](./data/sat_2019.csv): 2019 SAT Scores by State ([source](https://blog.prepscholar.com/average-sat-scores-by-state-most-recent))

#### Data Dictionary

|Feature | Dataset | Type | Description|
|---|---|---|---|
|state| ACT&SAT | object|State in the USA|
|sat_p_rate_2017| SAT_2017 | integer | State SAT Participation Rate 2017 |
|sat_r&w_2017| SAT 2017 | integer | Average Score in SAT reading & writing section |
|sat_math_2017| SAT 2017 | integer | Average Score in SAT Math section |
|sat_total_2017| SAT 2017 | integer | Average Total Score |
|sat_2017_policy | SAT 2017 | object | State Policy on SAT |
|sat_p_rate_2018| SAT 2018 | integer | State SAT Participation Rate in 2018 |
|sat_r&w_2018| SAT 2018 | integer | Average Score in SAT reading & writing section |
|sat_math_2018| SAT 2018 | integer | Average Score in SAT Math section |
|sat_total_2018| SAT 2018 | integer  | Average Total Score |
|sat_2018_policy | SAT 2018 | object | State Policy on SAT |
|sat_p_rate_2019| SAT 2019 | integer | State SAT Participation Rate in 2019 |
|sat_r&w_2019| SAT 2019 | integer | Average Score in SAT reading & writing section |
|sat_math_2019| SAT 2019 | integer | Average Score in SAT Math section |
|sat_total_2019| SAT 2019 | integer | Average Total Score |
|sat_2019_policy | SAT 2019 | object | State Policy on SAT |
|act_p_rate_2017 | ACT 2017 | integer | State ACT Participation Rate in 2017 |
|act_total_2017 | ACT 2017 | float | Average Total Score | 
|act_2017_policy | ACT 2017 | object | State Policy on ACT |
|act_p_rate_2018 | ACT 2018 | integer | State ACT Participation Rate in 2017 |
|act_total_2018 | ACT 2018 | float | Average Total Score | 
|act_2018_policy | ACT 2018 | object | State Policy on ACT |
|act_p_rate_2019 | ACT 2019 | integer | State ACT Participation Rate in 2017 |
|act_total_2019 | ACT 2019 | float | Average Total Score | 
|act_2019_policy | ACT 2019 | object | State Policy on ACT |

### References 

[](https://prepmaven.com/blog/test-prep/states-require-sat-act/  https://testive.com/state-sat-act/) 
[](https://www.providencejournal.com/news/20181025/with-sat-required-ri-sees-jump-in-participation-decline-in-scores) 
[](https://wvde.state.wv.us/news/3413/)
[](https://www.fairtest.org/state-sat-scores-reflect-spending) 
[](https://reports.collegeboard.org/archive/sat-suite-program-results/2019/benefits-sat-school-day)
[](https://www.brookings.edu/research/act-sat-for-all-a-cheap-effective-way-to-narrow-income-gaps-in-college/) 
[](https://blog.collegevine.com/states-that-require-sat/)
[](https://stephengodfrey.net/ )
[](https://medium.com/@james.dargan/participation-skews-state-averages-f68969371a01)


