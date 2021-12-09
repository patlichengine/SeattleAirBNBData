# Using CRISP-DM Walkthrough for SeattleAirBNBData Project ![Data Science Udacity Nanodegree](https://miro.medium.com/max/1400/1*80Nz4D9AhCjxTfDPsAINGA.jpeg)
### This section illustrates the process steps of CRISP-DM in the project above. Some vital information on the project has been provided on the Project Blog Post on medium. You can use the link below to access the blog post https://medium.com/@patlichengine/my-first-data-science-blog-post-365784c0d189

1. Business Understanding: 
  This specifies what we want to accomplish from a business perspective. For the chosen dataset, we are expected to identify 3 questions that would address business need and use     the data to solve them. The following questions would be answered:
  * How does user from each location respond to the different review categories and which rooms were visited the most?
  * In what way did the reviews affect the revenue of the company?
  * What policy affected the choice of review on the site and in which was do they visitors respond to the reviews.

2. Data Understanding:
   This stage deals with the data with the data which would be used to support the solution of the business problem stated above. This data source was provided though the Udacity nanodegree program. To get a understanding of the data, I downloaded the three data sources as follows:
   * Listing dataset
   * Review dataset and
   * Calender dataset
   This datasets were inspected to understand the composition using Pandas Dataframe function. The sample of the data is shown below:
   ![Data Understanding](https://miro.medium.com/max/875/1*pVf6vajlI7_dNooZNccMCA.jpeg)
   
3. Data Preparation:
   This step entails organizing data in a way it will help to answer business questions of interest. It involves handling missing values, categorizing data. Hence the two dataset was merged in order to get meaningful data and prices of product. Since the price field contained some currency symbols, I used a python function to cleaning the field.
