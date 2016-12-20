### Project Overview

In this project, you will analyze a business problem in the mail-order catalog business. You're tasked with predicting how much money your company can expect to earn from sending out a catalog to new customers. This task will involve building the model and applying the results in order to provide a recommendation to management.

#### How do I Complete this Project?
This project uses skills learned throughout our "Problem Solving with Advanced Analytics” course. To complete this project:
* Go through the course.
* Apply the skills learned in the course to solve the business problem given in the project details section. 
* Use our guidelines and rubric to help build your project.
* When you're ready, submit it to us for review using the submission template found in the supporting materials section.

Note: Depending on your experience, you may not need to take the whole course to complete this project.
<br></br>

#### Skills Required
In order to complete this project, you must be able to:
* Build a [linear regression model](https://classroom.udacity.com/nanodegrees/nd008/parts/c0b53068-1239-4f01-82bf-24886872f48e/modules/bf705147-0d7c-4492-842a-698a6410a8a3/lessons/4e33b70a-72a4-47cb-959a-28632ae6aaff/concepts/50223fb9-0a0a-4672-ba4c-deef74ebcc19#) and apply the results to a business problem.

## The Business Problem

You recently started working for a company that manufactures and sells high-end home goods.  Last year the company sent out its first print catalog, and is preparing to send out this year's catalog in the coming months. The company has 250 new customers from their mailing list that they want to send the catalog to.

Your manager has been asked to determine how much profit the company can expect from sending a catalog to these customers. You, the business analyst, are assigned to help your manager run the numbers. While fairly knowledgeable about data analysis, your manager is not very familiar with predictive models. 

You’ve been asked to predict the expected profit from these 250 new customers. Management does not want to send the catalog out to these new customers unless the expected profit contribution exceeds $10,000.

## Details

* The costs of printing and distributing is $6.50 per catalog. 
* The average gross margin (price - cost) on all products sold through the catalog is 50%.
* Make sure to multiply your revenue by the gross margin first before you subtract out the $6.50 cost when calculating your profit.

Write a short report with your recommendations outlining your reasons why the company should go with your recommendations to your manager.

<h3>Steps to Success</h3>
<h4>Step 1: Business and Data Understanding</h4>

Your project should include:
* A description of the key business decisions that need to be made.  

**Note:** Clean data is provided for this project, so you can skip the data preparation step of the Problem Solving Framework.

<h4>Step 2: Analysis, Modeling, and Validation</h4>

Build a [linear regression model](https://classroom.udacity.com/courses/ud976/lessons/4e33b70a-72a4-47cb-959a-28632ae6aaff/concepts/50223fb9-0a0a-4672-ba4c-deef74ebcc19), then use it to predict sales for the 250 customers. We encourage you to use [Alteryx to build the best linear model](https://classroom.udacity.com/courses/ud976/lessons/4e33b70a-72a4-47cb-959a-28632ae6aaff/concepts/cd0c2143-7268-4c76-8cf5-310be222da59) with your data. 

**Note**: For students using software other than Alteryx, if you decide to use Customer Segment as one of your predictor variables, please set the base case to Credit Card Only.

However, feel free to use any tool you’d like. You should create your linear regression model and come up with a linear regression equation.

Once you have your linear regression equation, you should use your linear regression equation to predict sales for the individual people in your mailing list. 

<h4>Step 3: Writeup</h4>
Once you have your predicted or expected profit, write a brief report with your recommendation to whether the company should send the catalog or not.

**Hint:** We want to calculate the expected revenue from these 250 people in order to get expected profit. This means we need to multiply the probability that a person will buy our catalog as well. For example, if a customer were to buy from us, we predict this customer will buy $450 worth of products. At a 30% chance that this person will actually buy from us, we can expect revenue to be $450 x 30% = $135.

## Review

Use the [project rubric](https://review.udacity.com/#!/rubrics/186/view) to review your project. If you are happy with your submission, then you're ready to submit your project. If you see room for improvement, keep working to improve your project.

## Submission Template

Use the [submission template](https://d17h27t6h515a5.cloudfront.net/topher/2016/October/581389d2_submissiontemplate/submissiontemplate.docx) at the bottom of this section to submit your project.  After filling it out, save it as a PDF and submit the PDF in the next section.

## Data
*[p1-customers.xlsx](https://d17h27t6h515a5.cloudfront.net/topher/2016/July/578d24c0_p1-customers/p1-customers.xlsx)* - This dataset includes the following information on about 2,300 customers. **Important**: You should build your model on this dataset and not *p1-mailinglist.xlsx*. 

*[p1-mailinglist.xlsx](https://d17h27t6h515a5.cloudfront.net/topher/2016/July/5790023a_p1-mailinglist/p1-mailinglist.csv)* - This dataset is the 250 customers that you need to predict sales. This is the list of customers that the company would send a catalog to. Use this dataset to estimate how much revenue the company can expect if they send out the catalog. It has the same fields as P1_Customers.xlsx, but includes two additional variables. 	
* Score_No: The probability that the customer WILL NOT respond to the catalog and not make a purchase.
* Score_Yes: The probability that the customer WILL respond to the catalog and make a purchase.

**Hint:** We want to calculate the expected revenue from these 250 people in order to get expected profit. This means we need to multiply the probability that a person will buy our catalog as well. For example, if a customer were to buy from us, we predict this customer will buy $450 worth of products. At a 30% chance that this person will actually buy from us, we can expect revenue to be $450 x 30% = $135.
