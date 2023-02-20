# Advanced Visualisation
## Exploratory Data Analysis and Visualization for Human Resources dataset
Karolina Szczęsna & Mateusz Cedro

The main purpose of this analysis is to display the main characteristics of the organization, find the most significant determinants of a salary, as well as gain information about the most successful employees.

## Dataset description
The original dataset from [Kaggle](https://www.kaggle.com/datasets/rhuebner/human-resources-data-set) contained 311 observations of employees from a certain organization described with 36 variables. We conducted data transformations and feature engineering, and our final dataset consisted of 294 observations and 47 variables.

## Data visualisation

### 1. Organization distribution
![Mock Slide](https://github.com/mateuszcedro/mateuszcedro/blob/main/Visualisation/Plots/s2.png)

The donut chart shows that there are more females in the organization than males. When it comes to race, the majority of employees are of white race, then there are significant shares of employees of black or asian race (pie chart). Based on the horizontal barplot, there is an equal number of widowed females and males in the organization. Moreover, the number of separated females highly exceeds the number of separated males, whereas the differences in other marital statuses are less varied. Stacked barplot indicates that employees of white, black or asian races work in all departments of the organization, while indian/native or other races work in sales or production and all hispanic people are employed in the production sector.

### 2. Salary distribution with respect to departments

![Mock Slide](https://github.com/mateuszcedro/mateuszcedro/blob/main/Visualisation/Plots/s3.png)
Histograms and density plots in the upper part show that all distributions are right-skewed. The boxplots and violin plots indicate that employees from Engineering and IT departments have the highest median of salary compared to Sales and Production. Other than that, violin plots show that there are a lot of extreme observations in the IT department and one or two outliers in Production or Sales - these are the managers who earn much more than other employees.

### 3. Between-Subject Comparisions

![Mock Slide](https://github.com/mateuszcedro/mateuszcedro/blob/main/Visualisation/Plots/s10.png)
Paiswise statistical analysis informs us that p-values of pairs are less than 5%, therefore they are statistically significant. This means that the distributions of pairs are varied.

### 4. How the number of years worked impact the salary?

![Mock Slide](https://github.com/mateuszcedro/mateuszcedro/blob/main/Visualisation/Plots/s7.png)
Scatter plot with trend line shows that there is a slightly inscreasing trend in salary as the number of years worked rises. However, the distribution of observations vary a lot and there occur some outliers, therefore the next scatter plot displays the dependence of years worked on salary with respect to departments.

### 5. How the number of years worked impact the salary in each department?

![Mock Slide](https://github.com/mateuszcedro/mateuszcedro/blob/main/Visualisation/Plots/s8.png)

Based on the second scatter plot, the trend lines for each department are highly impacted by outliers, which are emphasized at the top of the plot. There is one outliers per Production and Sales departments, and 7 outliers in IT department.

![Mock Slide](https://github.com/mateuszcedro/mateuszcedro/blob/main/Visualisation/Plots/s4.png)

From these four bubble plots it is clearly visible that in Production department, there is almost no variety in earned salary based on work experience. In order to better compare all employees, an interactive bubble plot was created.

### 6. Interactive Plot of Salary with respect to Department and Years Worked

![Mock Slide](https://github.com/mateuszcedro/mateuszcedro/blob/main/Visualisation/Plots/S5.gif)

This aggregated interactive plot made with plotly library combines bubble plots presented before for all departments but Production. Similar conclusions can be drawn in Sales, where the only observation with a yearly salary above $150k is a Sales Manager (outlier) and all other employees earn below $100k a year. The employees from the Engineering department also do not earn more as their work experience grows, however the average salary oscillates around $100k a year, which is higher than in Production and Sales. There is an increasing trend in the IT/IS department, meaning the more years an employee works, probably the higher he/she can earn, however only for the best performing employees. There is a group of IT employees, who work from 6-8 years and are stuck on the same level of yearly salary. The html version of this plot is available [here](https://drive.google.com/file/d/1K0MRoyAz230QqygAWnXS6z7GeRkATTiy/view) - You have to download id and than open it.

### 7. Employees’ performance and demographics

![Mock Slide](https://github.com/mateuszcedro/mateuszcedro/blob/main/Visualisation/Plots/s6.png)
This is an alluvial plot which represents employees’ performance and demographics regarding whether they still work (TRUE) or not (FALSE). It can be concluded that termination status is not correlated with performance or demographics of the employees, which matches the information from the dataset that all employees resign of their own will. Besides that, in terms of marital status, females and males are divided equally to single or married. Around half or married and half or single women gained a performance score above average.

###  8. What are the recruitment sources of the best performing employees?

![Mock Slide](https://github.com/mateuszcedro/mateuszcedro/blob/main/Visualisation/Plots/s9.png)

The third scatter plot shows the dependence between number of years worked on the salary with respect to recruitment sources. The outliers, meaning the best performing employees, are highlighted at the top of the plot. They were recruted from employee referal, Linkedin or job fairs.

### 9. How did the number of employees change over the years?

![Mock Slide](https://github.com/mateuszcedro/mateuszcedro/blob/main/Visualisation/Plots/gganim_yearOfHire.gif.png)

The animation presents the aggragated line plots of the number of employments in each department over the years 2006 - 2018. The plot shows that in 2010 there was a huge rise in emplyments in Production, which can indicate a strong focus on expansion of the organization and product development. However, this trend started to decrease later giving focus over to Sales and IT departments. The number of employments in Engineering did not vary much per year.

### 10. Where are located the employees of the organization?

![Mock Slide](https://github.com/mateuszcedro/mateuszcedro/blob/main/Visualisation/Plots/map1.gif)

The first map shows the distribution of employees location over the whole United States. Only the employees from Sales department are scattered over all states, whereas other departments are centered around Boston, where perhaps there is the main office of the organization.

![Mock Slide](https://github.com/mateuszcedro/mateuszcedro/blob/main/Visualisation/Plots/map2.gif)

The second map displays a zoomed version of the first map, which is the distribution of employees location around Boston. It is visible that all Production and Engineering departments employees are located in Boston and its suburbs, while IT department employees are located in Massachusetts, Connecticut and Rhode Island states.

The html versions of the maps are available here: [map1](https://drive.google.com/file/d/10mpIcW6tOYHRnq4o9kuOqGhGQMxlH5xt/view) and [map2](https://drive.google.com/file/d/1znMUXbNFL1OZCx95ZNdi42MDPbC7HtxU/view) - You have to download id and than open it.
