### Project Overview

You're a business analyst for Round Roasters, a coffee restaurant in the United States of America. The executive team conducted a market test with a new menu and needs to figure whether the new menu can drive enough sales to offset the cost of marketing the new menu. Your job is to analyze the A/B test and write up a recommendation to whether the Round Roasters chain should launch this new menu.

#### How Do I Complete this Project?

This project uses skills learned throughout the "A/B Testing ” course. To complete this project:

* Go through the course
* Apply the skills learned in the course to solve the business problem given in the project details section. 
* Use our guidelines and rubric to help build your project.
* When you're ready, submit it to us for review using the submission template found in the supporting materials section.

#### Skills Required

In order to complete this project, you must be able to:

* Cleanup, format, and blend a wide range of data sources
* Plan and analyze A/B tests

---------

### The Business Problem

Round Roasters is an upscale coffee chain with locations in the western United States of America.  The past few years have resulted in stagnant growth at the coffee chain, and a new management team was put in place to reignite growth at their stores.

The first major growth initiative is to introduce gourmet sandwiches to the menu, along with limited wine offerings. The new management team believes that a television advertising campaign is crucial to drive people into the stores with these new offerings. 

However, the television campaign will require a significant boost in the company’s marketing budget, with an unknown return on investment ([ROI](http://www.investopedia.com/terms/r/returnoninvestment.asp)).  Additionally, there is concern that current customers will not buy into the new menu offerings.

To minimize risk, the management team decides to test the changes in two cities with new television advertising. Denver and Chicago cities were chosen to participate in this test because the stores in these two cities (or markets) perform similarly to all stores across the entire chain of stores; performance in these two markets would be a good proxy to predict how well the updated menu performs.  

The test ran for a period of 12 weeks (2016-April-29 to 2016-July-21) where five stores in each of the test markets offered the updated menu along with television advertising. The fiscal week for Round Roasters is from Friday through Thursday.

The comparative period is the test period, but for last year.

You’ve been asked to analyze the results of the experiment to determine whether the menu changes should be applied to all stores.  The predicted impact to gross sales should be enough to justify the increased marketing budget: at least 18% increase in gross sales growth compared to the comparative period while compared to the control stores; otherwise known as *incremental lift*.

You have been able to gather three data files to use for your analysis:

* Transaction data for all stores from 2015-January-21 to 2016-August-18
* A listing of all Round Roasters stores
* A listing of the 10 stores (5 in each market) that were used as test markets.

### Steps to Success

#### Step 1: Plan Your Analysis

To perform the correct analysis, you will need to prepare a data set. Prior to rolling up your sleeves and preparing the data, it’s a good idea to have a plan of what you need to do in order to prepare the correct data set.  A good plan will help you with your analysis.

#### Step 2: Clean Up Your Data

You should filter out the necessary dates and aggregate the data in this step. Furthermore, you need to look for outliers in the treatment and control units and remove the outliers from your dataset.

#### Optional Step: Effect Analysis

This is an extra “bonus” step for you to learn how to use transactions and sales mix in order to approximate the effect that the market test has on sales. The reason why analyzing transactions and sales mix is good practice is that these metrics will tell you exactly which items are driving the sales lift.

This step is **completely optional** for you to complete. Further instructions can be found in the project template.

#### Step 3: Analysis and Writeup

Conduct your A/B analysis and create a short report outlining your results and recommendations.


------

### Review

Use the [project rubric](https://review.udacity.com/#!/rubrics/287/view) to review your project. If you are happy with your submission, then you're ready to submit your project. If you see room for improvement, keep working to improve your project.

### Submission Template

Use the [submission template](https://d17h27t6h515a5.cloudfront.net/topher/2016/October/57f43a42_submissiontemplate/submissiontemplate.docx) at the bottom of this section to submit your project.  After filling it out, save it as a PDF and submit the PDF in the next section.

#### Data

*[round-roaster-stores.csv](https://d17h27t6h515a5.cloudfront.net/topher/2016/September/57e314da_round-roaster-stores/round-roaster-stores.csv)* - This file contains store information for each Round Roaster store in the USA.

*[treatment-stores.csv](https://d17h27t6h515a5.cloudfront.net/topher/2016/September/57e314ee_treatment-stores/treatment-stores.csv)* - This file contains store information for each store that offered the new menu items.

*[round-roaster-transactions.zip](https://d17h27t6h515a5.cloudfront.net/topher/2016/September/57e31510_round-roaster-transactions/round-roaster-transactions.zip)* - This file contains transaction level information for all of Round Roaster's stores


-------


#### Sampling

The transaction database contains more than 3 million rows of transaction data. As you create your workflows, we recommend you only sample data and process a few thousand rows of data at a time.  This method will **significantly** reduce your time spent processing your data. If you're using Alteryx, you can use the [Sample](https://help.alteryx.com/10.6/index.htm#Sample.htm) tool.

#### Aggregate and Export

We recommend you save your aggregated transaction database as a separate file to further reduce your development time. You shouldn't need to re-aggregate the transaction database every time you want to test out a new workflow.

#### Weekly Tracker

To help you keep track of the comparative periods and test periods, we recommend you create a file to keep track of the fiscal weeks along with the week number. A weekly tracker could look like this:

| Week | Period   | Week Begin | Week End |
|------|----------|------------|----------|
| 44   | Comp-W12 | 04/04/16   | 04/10/16 |
| 53   | Test-W1  | 06/6/16   | 06/12/16 |
| 54   | Test-W2  | 06/13/16   | 06/19/16 |
