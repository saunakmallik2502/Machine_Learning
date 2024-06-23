# Lending Club Case Study - by Saunak MALLIK
> Thie project work is for a consumer finance company which specialises in lending various types of loans to urban customers. In this project I have used various EDA (Exploratory Data Analysis) methods to understand the impact of consumer attributes and loan attributes influence the tendency of loan default.
          
> The final recommendation is provide insights and prescribe recommendations to ensure to mitigate risk while lending to customers. 

## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Project Methodology](#project-methodology)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- When the company receives a loan application, the company has to make a decision for loan approval based on the applicants profile.
- This finance company should decide whether to approve the loan or not  based  on the loan application and available data with the company.
- Two types of risks are associated with the bank's decision:	
   1) If the applicant is likely to repay the loan, then not approving the loan results in a loss of business to the company	
   2) If the applicant is not likely to repay the loan, i.e. he/she is likely to default, then approving the loan may lead to a financial loss for the company	
- The data given from the company contains information about past loan applicants and whether they defaulted or not.
- The aim is to identify patterns which indicate if a person is likely to default, which may be used for taking actions such as denying the loan, reducing the amount of loan, lending (to risky applicants) at a higher interest rate, etc.
- When a person applies for a loan,there are two types of decisions that could be taken by the company:
     1) Loan accepted: If the company approves the loan, there are 3 possible scenarios described below:	
        a)	Fully paid: Applicant has fully paid the loan (the principal and the interest rate).	
	b) Current: Applicant is in the process of paying the instalments, i.e. the tenure of the loan is not yet completed. These candidates are not labelled as 'defaulted'.	
	c) Charged-off: Applicant has not paid the instalments in due time for a long period of time, i.e. he/she has defaulted on the loan.
    2) Loan rejected: The company had rejected the loan (because the candidate does not meet their requirements etc.).		
	 Since the loan was rejected, there is no transactional history of those applicants with the company and so this data is not available with the company (and thus in this dataset)	

- Credit loss is the amount of money lost by the lender when the borrower refuses to pay or runs away with the money owed. In other words, borrowers who default cause the largest amount of loss to the lenders. In this case, the customers labelled as 'charged-off' are the 'defaulters'. 

- The company wants to understand the key driving factors (or driver variables) for loan default, i.e. the variables which hace strong correlation of default.
  The company can utilise this knowledge for its portfolio and risk assessment. 

- Dataset used for this project: "loan.csv"

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Project Methodology
- Data understanding - Use pandas library to study the dataset and gain initial insights on the dataset.
- Data Cleaning and Manipulation - Use pandas library to identify NULL values, redundancies, clean data e.g., removal of %, texts etc. in numerical data columns and finally removal of outliers.
- Data analysis & Insights - Use pandas, matplotlib and seaborn libraries to perform Univariate, Bi-Variate and Multi Variate analysis and produce insights from the data.
- Recommendation - Summarize insights and provide recommendations to the business stakeholders.

## Conclusions
- Track principal repayments very closely:
 Likelihood of repayments stopping if one repayment of principal is not done by the customer.
 Recommendation: Automated system alerts for customers defaulting principal repayment for even 1 cycle.

- Lending cycle:
More loans are disbursed in the last Quarter of the year.
Recommendation: Run promos in the last quarter of the years to augment the lending book.

- Creditworthiness & Due diligence assessment:
Higher grades (A and B) tend to be associated with lower interest rates and lower default rates.
Customers with a history of bankruptcy tend to default more.
Customer with high DTI (already having high debt) are likely to default more.
Recommendation: Lend more to high-grade borrowers. Exercise additional due-diligence before approval of loans to low grade borrowers. 
Avoid customers with history of bankruptcy and high DTI ratio.

- Length of Employment:
Borrowers with longer employment tend to repay loans better
Recommendation: Prioritize borrowers with employment lengths of 5+ years.

- Existing Home Ownership:
Existing Homeowners (with mortgage or owned outright) have lower default rates compared to renters.
Recommendation: Promo offers of lower interest rates to existing homeowners.

- Loan Purpose:
Loans purpose is a critical driver for the loan. Each sector has it’s own nuances and cyclicality which needs proper due diligence to be conducted to avoid default.
Recommendation: Perform strict sectoral due-diligence for each loan purpose.


<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Technologies Used
- python 3 with Jupyter Note Book
- libraries used - numpy, pandas, matplotlib, seaborn

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements

- This project and the data was provided by [IIITB] (https://www.iiitb.ac.in/) & [upGrad](https://www.upgrad.com/) learning platform.
- Please note that the dataset is for learning purposes only.


## Contact
- Created by [Saunak MALLIK](https://github.com/saunakmallik2502)- feel free to connect!
- This project work repository is here : [Lending Club Case Study](https://github.com/saunakmallik2502/Machine_Learning).

    