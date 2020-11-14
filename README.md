# What factors make a Kickstarter campaign successful?

This repository provides explanations of the data analysis process for the DataRes article "[INSERT YOUR TEAM'S ARTICLE TITLE HERE](INSERT URL)", published [INSERT DATE]. Please check out our article, which contains visualizations and insights about Kickstarter campagins.
Contributors: Raymond Bai, Samantha Chung, Emily Hou, Andy Shen, Amy Tang

# Data
The data used to develop our Medium article came from Kaggle: https://www.kaggle.com/kemical/kickstarter-projects?select=ks-projects-201801.csv
Give some background about the data here. When was the data set created? What year(s) was the data from the data set from? How many variables were in it?

There were 15 variables. 

The data set contained the following columns:
* `id` - Internal Kickstarter project ID
* `name` - Name of the project
* `category` - Variable description
* `main_category` - Variable description
* `currency` - Variable description
* `deadline` - Variable description
* `goal` - Variable description
* `launched` - Variable description
* `pledged` - Variable description
* `state` - Variable description
* `backers` - Variable description
* `country` - Variable description
* `usd.pledged` - Variable description
* `usd_pledged_real` - Variable description
* `usd_goal_real` - Variable description


# Data Processing
In this section, focus on discussing the technical data cleaning/analysis that you did. How did you clean the data? Were there any columns with NAs or missing values and how did you treat them? What variables did your team omit, if any, and why? What variables did your team analyze in your article? What other issues with the data did your team encounter and how did you address it?




# Analysis and Code
The analysis can be found at `[analysis/]`https://github.com/amytang-ml/blueteam/tree/main/analysis. 
Each member of our team contributed to developing visualizations for our article. Discuss the languages you used (R/Python) and what libraries you utilized for analysis and visualizations. Also talk about the types of research questions your team came up with and how you went about analyzing them.

We set out to answer questions about what makes a successful project:

# Time elapsed between launch date and date the goal was reached
What is the summary and distribution of time elapsed for all campaigns and successful campaigns? Is there a point where people should just give up on meeting their goal because it's been too long? How many days does it take for most projects to be completed? Median time elapsed of top categories? [Amy]

# Categories 
Count (looking at the top three project categories, are projects in those categories more likely to succeed because of popularity or less likely because they are drowned out by others?) [Raymond]

# Funding goal
How big can projects get? How high is too high? Is there an ideal goal amount that has highest rates of success?) [Emily]

# Number of backers
For the successful campaigns, the 95th percentile is 885 backers, with there being a large range, as the third quartile is 167 backers but the maximum is 219382 backers. Also, the 219382 backers comes from the project main category of games.  By looking at the first, median, and third quartiles, we noticed that there are generally around under one thousand backers for successful projects.

For the unsuccessful campaigns, which is defined by cancelled and failed campaigns, the 95th quantile is 72, and the third quartile is 13 backers.
For everything else, defined by the live, suspended, and undefined campaigns, the 95th quantile is 122.7 and the third quartile is 6 backers.

Furthermore, visually, the "successful" campaigns seems to have a backer distribution that is more left skewed than the failed and cancelled, or "others" category. Henceforth, in general, successful campaigns appears to be funded by a larger number of backers.

Additionally, we also looked at the top three categories: arts, crafts, and comics. Amongst these, the quartile distributions, and 95th quartile distribution is not too different from the overall distribution of the number of backers. Therefore, we can also conclude that amongst the most popular categories, the number of backers funded is no different than other categories that were not as popular.

Finally, this is in line with our predictions because one would expect a project with a greater amount of backers to be the most successful.

