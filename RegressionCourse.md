---
title: Applied Statistics II (Regression Analysis)
description: This is a homepage for MAT300, Regression Analysis, with Dr. Gilbert at Southern New Hampshire University. This course introduces students to the construction, assessment, and interpretation of models in the regression setting.
---

## MAT 300 - Applied Statistics II: Regression Analysis

<img src="/SiteFiles/ISLR.png" align="left" width=200>[**Syllabus (Spring 2023)**](https://drive.google.com/file/d/16uY1DsSHVn3eMP1pL3G1t592U7ljlw2O/view?usp=share_link)<br/>
<br/>
***Course Description:*** This is a second course in statistics that builds upon knowledge gained in MAT 240 or an AP statistics course. Students will learn to build statistical models and develop skills for implementing regression analysis in real-world problems from engineering, sociology, psychology, science and business. Topics include multiple regression models (including first-order, second-order and interaction models with quantitative and qualitative variables), regression pitfalls and residual analysis. Additional topics will be covered if time permits. Students will gain experience not only in the mechanics of regression analysis (often by means of a statistical software package) but also in deciding on appropriate models, selecting inferential techniques to answer a particular question, interpreting results and diagnosing problems.<br/>
<br/>

Students in this course will use R, in particular the `tidyverse` and `tidymodels` ecosystems, to build and analyze regression models. The course covers simple and multiple linear regression, curvi-linear regression with polynomial and interaction terms, regularization with Ridge Regression and the LASSO, and tree-based models/ensembles. Cross-validation is implemented as an important technique for stable and unbiased model performance estimates, for identifying appropriate levels of model flexibility, and for hyperparameter tuning.<br/>
<br/>

### Course Timeline and Notebooks

Below is a tentative timeline for our course. It includes preparatory work that should be done prior to each class meeting, a detailed set of notes corresponding to each class meeting, and assignments following each class meeting. The prepared notebooks use the Palmer `penguins` and `ames` housing datasets and are provided so that you have a detailed account of each topic we discuss. We'll learn this content better by *doing* it that we will by simply *reading* and *running* pre-existing code, so we'll plan to utilize different data in class. For now, I'm planning to start with [this data set](https://github.com/rfordatascience/tidytuesday/tree/master/data/2022/2022-07-05) on rental properties in the San Francisco Bay Area posted to Craigslist, generously made open by [Dr. Kate Pennington](https://www.katepennington.org/data). We can switch to alternate data sets as student interest dictates. I've prepared the following **student notes template** ([html](https://agmath.github.io/RegressionCourse/StudentNotesTemplate.html), [rmd](https://agmath.github.io/RegressionCourse/StudentNotesTemplate.Rmd)) that I hope you'll use to follow along during our in-class discussions. 

| Class Meeting | Before Class | During Class | After Class |
|---------------|--------------|--------------|-------------|
| 1 | [Review Syllabus](https://drive.google.com/file/d/16uY1DsSHVn3eMP1pL3G1t592U7ljlw2O/view?usp=share_link) <br/> [Install R and RStudio](https://agmath.github.io/RegressionCourse/1b_AccessingRandRStudio.html) | [Introduction and What to Expect](https://agmath.github.io/RegressionCourse/1d_Outline.html)<br/> Ethics and Data Models |  |
| 2 | Enroll in Competition <br/> Read ISLR S2.1 ([Part I](https://www.youtube.com/watch?v=p9n2w236B48), [Part II](https://www.youtube.com/watch?v=HndOzII4jzs)) | [What is Statistical Learning?](https://agmath.github.io/RegressionCourse/2d_StatisticalLearning.html) <br/> Competition Discussion <br/> What is an Analytics Report? ([html](https://agmath.github.io/RegressionCourse/WhatIsAnAnalyticsReport.html), [rmd](https://agmath.github.io/RegressionCourse/WhatIsAnAnalyticsReport.Rmd)) | [Competition Assignment 1](https://agmath.github.io/RegressionCourse/CA1_StatementOfPurpose.html)  <br/> Analytics Report Shell ([html](https://agmath.github.io/RegressionCourse/AnalyticsReportShell.html), [rmd](https://agmath.github.io/RegressionCourse/AnalyticsReportShell.rmd)) |
| 3 | [Read ISLR S2.3](https://youtu.be/VaN1RUDuioQ) | Introduction to R: Enter the `tidyverse` ([html](https://agmath.github.io/RegressionCourse/3d_CrashCourse_TidyR.html), [rmd](https://agmath.github.io/RegressionCourse/3d_CrashCourse_TidyR.Rmd)) | |
| 4 | [Read R4DS S3.1 - 3.10](https://r4ds.had.co.nz/data-visualisation.html) <br/> (Optional) | Data Viz and `ggplot2` ([html](https://agmath.github.io/RegressionCourse/4d_DataViz_Primer.html), [rmd](https://agmath.github.io/RegressionCourse/4d_DataViz_Primer.Rmd)) | [Competition Assignment 2](https://agmath.github.io/RegressionCourse/CA2_ExploratoryDataAnalysis.html) |
| 5 |  | R Workshop Day: R Markdown |  |
| 6 |  | Data Wrangling Workshop ([html](https://agmath.github.io/RegressionCourse/6d_DataWrangling.html), [rmd](https://agmath.github.io/RegressionCourse/6d_DataWrangling.Rmd)) | Homework 1 ([html](https://agmath.github.io/RegressionCourse/HW1_DataWrangling.html), [rmd](https://agmath.github.io/RegressionCourse/HW1_DataWrangling.rmd)) |
| 7 |  | Introduction to `tidymodels` ([html](https://agmath.github.io/RegressionCourse/7d_tidymodelsOverview.html), [rmd](https://agmath.github.io/RegressionCourse/7d_tidymodelsOverview.Rmd)) |  |
| 8 | Intro Stats Review | Hypothesis Testing and Confidence / Prediction Intervals in Regression ([html](https://agmath.github.io/RegressionCourse/8d_IntroStatsForRegression_Review), [rmd](https://agmath.github.io/RegressionCourse/8d_IntroStatsForRegression_Review.Rmd)) | Homework 2 ([html](https://agmath.github.io/RegressionCourse/HW2_UnderstandingAssumptions.html), [rmd](https://agmath.github.io/RegressionCourse/HW2_UnderstandingAssumptions.rmd)) |
| 9 | Read ISLR S3.1 ([Part I](https://youtu.be/7TgVO_K75EY), [Part II](https://youtu.be/z10DqaVJh3c)) | Simple Linear Regression: <br/> Construction, Interpretation, and Model Assessment ([html](https://agmath.github.io/RegressionCourse/9d_SimpleLinearRegression.html), [rmd](https://agmath.github.io/RegressionCourse/9d_SimpleLinearRegression.Rmd)) | [Competition Assignment 3](https://agmath.github.io/RegressionCourse/CA3_SimpleLinearRegression_SubmitPredictions.html) |
| 10 | Read ISLR S 3.2 ([Part I](https://youtu.be/yzQHONabWhs), [Part II](https://youtu.be/lo7KnnvyEU0)) | Multiple Linear Regression: <br/> Construction, Interpretation, and Model Assessment ([html](https://agmath.github.io/RegressionCourse/10d_MultipleLinearRegression.html), [rmd](https://agmath.github.io/RegressionCourse/10d_MultipleLinearRegression.Rmd)) |  |
| 11 | Read ISLR S3.3 ([Part I](https://youtu.be/lo7KnnvyEU0), [Part II](https://youtu.be/sK80ZnhiaRI)) | Categorical Predictors and Interpretations <br/> Feature Engineering with `step_other()` and `step_dummy()` ([html](https://agmath.github.io/RegressionCourse/11d_CategoricalPredictors.html), [rmd](https://agmath.github.io/RegressionCourse/11d_CategoricalPredictors.Rmd)) | [Competition Assignment 4](https://agmath.github.io/RegressionCourse/CA4_MultipleLinearRegression_Interpretation_SubmitPredictions.html) |
| 12 |  | Model Building, Assessment, and Interpretation Workshop |  | 
| 13 |  | Higher-Order Terms: <br/> Curvi-Linear Regression and Polynomial Terms with `step_poly()` ([html](https://agmath.github.io/RegressionCourse/13d_HigherOrderTerms_Polynomial.html), [rmd](https://agmath.github.io/RegressionCourse/13d_HigherOrderTerms_Polynomial.Rmd)) | [Competition Assignment 5](https://agmath.github.io/RegressionCourse/CA5_HigherOrderModel_SubmitPredictions.html) |
| 14 |  | Higher-Order Terms: <br/> Interaction with `step_interact()` ([html](https://agmath.github.io/RegressionCourse/14d_HigherOrderTerms_Interaction.html), [rmd](https://agmath.github.io/RegressionCourse/14d_HigherOrderTerms_Interaction.Rmd)) |  |
| 15 | [Read ISLR S2.2](https://youtu.be/VaN1RUDuioQ) | Bias/Variance Trade-Off and Model Performance Concerns ([html](https://agmath.github.io/RegressionCourse/15d_BiasVarianceTradeOff_Overfitting.html), [rmd](https://agmath.github.io/RegressionCourse/15d_BiasVarianceTradeOff_Overfitting.Rmd)) |  |
| 16 | Read ISLR S5.1 ([Part I](https://youtu.be/ngrOYWgJjb4), [Part II](https://youtu.be/rSGzUy13F_0), [Part III](https://youtu.be/r64tRyHFAJ8)) | Performance Concerns Continued: Different Test, Different Expectations <br/> Cross-Validation and Unbiased Model Performance ([html](https://agmath.github.io/RegressionCourse/16d_CrossValidation.html), [rmd](https://agmath.github.io/RegressionCourse/16d_CrossValidation.Rmd)) | Homework 3 |
| 17 |  | Cross-Validation Workshop |  |
| 18 | Read ISLR S6.1, 6.2 ([Part IV](https://youtu.be/f_hkP_We0JY), [Part V](https://youtu.be/I8bPQ272Pbs), [Part VI](https://youtu.be/FlSQgXv7Dvw), <br/> [Part VII](https://youtu.be/8oEZkHqf_Rk)) | Variable Selection Methods: <br/> Stepwise Regression, Ridge Regression, and the LASSO ([html](https://agmath.github.io/RegressionCourse/17d_VariableSelectionMethods.html), [rmd](https://agmath.github.io/RegressionCourse/17d_VariableSelectionMethods.Rmd)) |  |
| 19 |  | Other Regressors ([html](https://agmath.github.io/RegressionCourse/18d_OtherRegressors.html), [rmd](https://agmath.github.io/RegressionCourse/18d_OtherRegressors.Rmd)) | [Competition Assignment 6](https://agmath.github.io/RegressionCourse/CA6_OtherRegressors_SubmitPredictions.html) | 
| 20 |  | Hyperparameters and Tuning <br/> More uses for Cross-Validation ([html](https://agmath.github.io/RegressionCourse/19d_HyperparameterTuning.html), [rmd](https://agmath.github.io/RegressionCourse/19d_HyperparameterTuning.Rmd)) |  |
| 21 |  | Hyperparameters, Tuning, and Other Regressors Workshop |  | 
| 22 | [Read ISLR S4.3](https://youtu.be/RN_dweQpcpo) | Classification with Logistic Regression ([html](https://agmath.github.io/RegressionCourse/20d_ClassificationAndLogisticRegression.html), [rmd](https://agmath.github.io/RegressionCourse/20d_ClassificationAndLogisticRegression.Rmd)) |  |
| 23+ | Projects | Projects | Projects |

<br/>
<br/>

***

> [1] DeCock, Dean (2011). Ames, Iowa: Alternative to the Boston Housing Data as an End of Semester Regression Project. Journal of Statistics Education Volume 19, Number 3(2011),
http://www.amstat.org/publications/jse/v19n3/decock.pdf
>
> [2] Horst AM, Hill AP, Gorman KB (2020). palmerpenguins: Palmer Archipelago (Antarctica) penguin data. doi:10.5281/zenodo.3960218, R package version 0.1.0, https://allisonhorst.github.io/palmerpenguins/.
>
> [3] Pennington, Kate (2018). Bay Area Craigslist Rental Housing Posts, 2000-2018. Retrieved from https://github.com/katepennington/historic_bay_area_craigslist_housing_posts/blob/master/clean_2000_2018.csv.zip.

***

<br/>
<br/>

[Back to Hompage](https://agmath.github.io/)
