# Retail-sales-Data-Agent-
Retail sales Data Agent Assignment 

#Introduction
This project is about building a functional data agent that can analyse data, generate insights, and respond to user queries effectively. The assignment also involves uploading a data set on Sequel, Understanding the dataset and preparing the data for testing the agent’s ability to interpret and answer questions accurately, and evaluate the quality of the outputs produced.
Using SQL queries, various data analysis techniques such as aggregation, filtering, grouping, and statistical calculations. In addition, the assignment explores the strengths and limitations of the data agent by identifying loopholes, incorrect responses, unnecessary outputs, and areas where the agent may misinterpret user requests.

#Objective
My overall aim in doing this assignment is to familiarise myself with how data bricks works ,how to prepare data for sequel and to understand how AI-driven data agents operate in practical environments, evaluate their reliability in supporting data-driven decision-making, and identify opportunities for improving the accuracy, relevance, and efficiency of automated data analysis systems.

#Dataset description
•	The retail sales dataset is a set of data detailing Sales of a retail company 
•	The data is from 01/01/2023 till 01/01/2024
•	The data is for the financial year end 2024
•	The transaction ID represents a unique identifier assigned to each sale transition 
•	The column date shows the exact date that the transaction occurred 
•	Customer ID column details a unique identifier used to identify a customer 
•	The gender column shows the gender of the customer; this helps the customer to analyse whether its customer base is   man or mainly women and it can help the company deep dive into how customer buying decisions are influenced 
•	Age column represent the age that the customer is, this can help the company check the demographics of its customers 
•	Product category column details the different divisions of products the retail company sells i.e. Beauty, electronics and clothing 
•	The quantity column represents the number of products the customer purchased per transaction 
•	The price per unit column shows how much each product cost this is the retail company cost price plus their mark up 
•	The total amount column is the quantity multiplied by price per unit, this details how much each transaction id made 
•	The retail sales dataset shows that the company generates $456,000 in total revenue
•	The dataset details 1000 transactions from 1000 unique customers
•	The data is complete and has no missing values 
•	The retail dataset shows that their oldest customer is 65 in the year 2023 Jan to 2024 Jan 
•	With their youngest customer in that same financial year end being 18

#AGENT INSTRUCTIONS
Question 5
Retail sales insights agent role
It enables quick analysis of retail sales transactions to uncover trends, customer insights such as purchasing behaviour, drop in sales, and performance across product categories.it enables the user to have and visualize the data in a matter of minutes while affording them the opportunity to make business decisions in a matter of minutes.
Retail sales insights agent(capabilities)- what it does 
•	Track sales volume and revenue by date, customer demographics, and product category
•	It allows quick data visualization to aid decision making 
•	Identify top-selling products, customer segments, and sales patterns over time
•	Analyse purchase behaviour by gender and age group
•	Aggregates total revenue for retail sales 
•	Provides insight on who exercises their buying power more between men and women
•	Which product category is a cash cow for the company, and which is under performing 
•	Analysis and provides insights on which age group supports the company more 
•	Monitor transaction-level details for operational performance

For whom the data agent is for- (The users)
•	This data agent is for the CEO
•	The sales team
•	The buying team

Dataset to be used by Retail sales insights agent
•	retail_sales_dataset_2
 Agent must not edify dataset from any other table, Retail sales agent must use the above dataset only 

Question types that Retail sales insights agent should answer
•	Sales trends like the highest selling product category
•	Data visualization based on the dataset provided 
•	Age groups trends
•	Highest stock level to be sold 
•	Analysis on Age 
•	Purchasing power of customers based on sale date
•	The distribution (min, max, average, median) of transition total amount

How to explain insights
•	A professional tone to be always kept, as these answers are going to be used by stakeholders
•	To only use data visualization only when asked by the user 
•	Answers to be concise theory backed by factual numbers from the data set 
•	Repetition to be avoided 

How to handle ambiguity
•	The data Retail sales insights agent must handle ambiguity by clarifying the prompt, breaking it into simple under stable query and ensuring that all expectations are met
•	Avoiding repetitions on the Query

How to avoid making things up 
•	Retail sales insights agent must only use the dataset linked and provided, it should never edify the dataset to meet queries 
•	If the query needs Retail sales insight agent dataset to fabricate data that’s not on the retail_sales_dataset_2 it must return a null output

How to give recommendations
•	Retail sales insights agent can give recommendations only when the question is ambiguous

#10 Test questions for Retail sales insights Agent
1.	Total amount of sales made in Jan 2023
2.	Total amount made by each product category as a percentage of total amount of sales 
3.	Create a pie chart of Age categorize by 18-30 Young adult, 30-40 Adult; 40-50 Mid age,51-65 Pensioner 
4.	What is the number of females and what is the number of males on the dataset
5.	What are the patterns on total sales for the current financial year end?
6.	What is the distribution (min, max, average, median) of the transaction total amounts?
7.	Do a bar graph of total amount based on product category
8.	What is the total quantity of products purchased, categorise by month
9.	Total amount greater or equal to 2000
10.	Based on the total amount, which product is the companies cash cow and what can the company do to increase the sales of its other products.
#Validate Questions
1.	what is the total amount grouped by product category
  Answer from the Retail sales insights agent
2.	What is the distribution (min, max, average) of the transaction total amounts?
3.	Sort the data in Descending order using the total amount limit to 10 rows 
#Key insights 
Business Performance Insights

Product Category Performance
•	Electronics leads in revenue at $156,905 (34.4% of total), followed closely by Clothing at $155,580 (34.1%) and Beauty at $143,515 (31.5%). Despite similar revenue contributions, Beauty products command the highest average transaction value at $467, suggesting premium positioning.
•	This might be due to the fact that 51% of the companies’ customers are female.
Customer Demographics
•	The customer base is evenly split between Female (51%) and Male (49%) customers, with nearly identical average transaction values ($456.55 vs $455.43). 
•	The average customer age is 41 years, with a range from 18 to 64 years. 
•	Age group analysis reveals that the 45-54 age group generates the highest absolute revenue at $97,235, but the Under 25 segment shows the highest average transaction value at $501, indicating strong purchasing power among younger customers despite lower transaction volume (149 transactions). 
Temporal Patterns
•	Monthly revenue shows significant volatility, ranging from $23,620 in September to $53,150 in May 2023. 
•	The data reveals no clear seasonal pattern, with peaks occurring in February, May, and October. September represents the weakest month, suggesting potential seasonal challenges or operational issues during that period
Product category trends over time show Electronics experiencing strong performance in May ($23,245) and December ($20,220), while experiencing a significant dip in March ($3,380). This volatility suggests category-specific seasonal factors or inventory challenges.
#Conclusion
•	What assisted the most is following the notes I took from Leratos consultation 
•	The suggested answers on the assignment were quite helpful as they provided a guideline for what the desired outcome should be 
•	Question 2 was the most difficult because Run df.printSchema() and df.describe() are not syntax I’ve come across before 

