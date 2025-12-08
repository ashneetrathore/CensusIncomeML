## :dollar: ANALYSIS AND ML PREDICTION ON THE ADULT CENSUS DATASET

### :open_book: OVERVIEW
Date: December 2024\
Author(s): Ashneet Rathore

 The [**Census Income dataset**](https://archive.ics.uci.edu/dataset/20/census+income), otherwise known as the Adult dataset, contains 14 features, which are a mix of categorical and integer types. The target variable has two labels: `<=50K` and `>50K`. This dataset can be used for **binary classification** tasks, where the goal is to predict whether or not an individual’s annual income exceeds $50K based on 1994 census data. The following sections present an exploratory analysis of the dataset and the accuracy performance of three different boosting algorithms – **AdaBoost**, **Gradient Boosting**, and **XGBoost** – across different parameter settings.

> [!NOTE]
> All figures referenced in this report can be found in the corresponding Jupyter Notebook (`project.ipynb`) in the repository.

### :bar_chart: EXPLORATORY ANALYSIS
During the data exploration phase, the relationships between various features and the likelihood of earning more than 50K were examined to identify characteristics associated with higher income.

Figure 1 displays the percentage of people earning more than 50K categorized by sex. The bar chart reveals that while 30% of males earned more than 50K in 1994, only about 10% of all females did. This disparity reflects broader trends in the 1990s: although women were increasingly entering the workforce, they were still underrepresented in high-paying roles and often earned less than their male counterparts for comparable work.


### :trophy: EVALUATION OF BOOSTING ALGORITHMS
