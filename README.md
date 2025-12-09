## :dollar: ANALYSIS AND ML PREDICTION ON THE ADULT CENSUS DATASET

### :open_book: OVERVIEW
Date: December 2024\
Author(s): Ashneet Rathore

 The [**Census Income dataset**](https://archive.ics.uci.edu/dataset/20/census+income), otherwise known as the Adult dataset, contains 14 features, which are a mix of categorical and integer types. The target variable has two labels: `<=50K` and `>50K`. This dataset can be used for **binary classification** tasks, where the goal is to predict whether or not an individual’s annual income exceeds $50,000 based on 1994 census data. The following sections present an exploratory analysis of the dataset and the accuracy performance of three different boosting algorithms – **AdaBoost**, **Gradient Boosting**, and **XGBoost** – across different parameter settings.

> [!NOTE]
> All figures referenced in this report can be found in the corresponding Jupyter Notebook (`project.ipynb`) in the repository.

### :bar_chart: EXPLORATORY ANALYSIS
During the analysis phase, the relationships between various features and the likelihood of earning more than $50,000 were examined to identify characteristics associated with higher income.

Figure 1 displays the percentage of people earning more than $50,000 categorized by sex. The bar chart reveals that while 30% of males earned more than $50,000 in 1994, only about 10% of all females did. This disparity reflects broader trends in the 1990s: although women were increasingly entering the workforce, they were still underrepresented in high-paying roles and often earned less than their male counterparts for comparable work.

Figure 2 displays the percentage of people earning more than $50,000 categorized by age. The plot shows that middle-aged adults, ranging from 40 to 60 years old, had the highest percentage of income greater than $50,000, with the peak occurring at age 50. This upside-down U shape aligns with typical career trends: while young adults are either in school or just beginning their careers, and older adults people are reducing their workload and preparing for retirement, middle-aged adults are typically in the prime of their established careers, more likely at higher-paying positions in the industries they work in.

Figure 3 shows the percentage of people earning more than $50,000 categorized by education level. Individuals with bachelor's and master's degrees have noticeably higher proportions of high earners compared to those with an associate degree, which displays the role that a four-year or higher degree can play in accessing better-paying jobs. The gap is even larger for those with doctorate or professional degrees, which aligns with the common trend that advanced degrees in specialized fields, such as law or medicine, are linked to higher incomes.

Figure 4 shows the frequency of adults in each occupation, separated by income category (`<=50K` and `>50K`). Each occupation has two bars representing the number of individuals earning 50K or less and those earning more than 50K. This visualization highlights which occupations tend to have more high-income earners and which are dominated by lower-income earners, providing a clear view of how income is distributed across different types of work. 

According to the chart, executive-managerial and professional-speciality positions have the highest relative proportion of individuals earning above $50,000, indicating a larger fraction of high earners compared to other occupations. Roles involving technical manual labor and administrative tasks, such as administrative-clerical, craft-repair, and sales occupations, have a large gap between the two bars, with the majority earning $50,000 or below and only a small fraction earning above $50,000. Farming-fishing, service, and tech support roles show an even wider gap between the two bars, with relatively few high earners. These income patterns do not necessarily correspond to the societal importance of the occupations. For instance, farming plays a critical role in society, yet it shows a relatively low proportion of high-income earners, illustrating that essential work is not always matched with higher pay.

### :trophy: EVALUATION OF BOOSTING ALGORITHMS
