# CRISP-DM Walkthrough for the SeattleAirBNBData Project 
![Data Science Udacity Nanodegree](https://miro.medium.com/max/1400/1*80Nz4D9AhCjxTfDPsAINGA.jpeg)
### This section illustrates the process steps of CRISP-DM in the project above. Some vital information on the project has been provided on the Project Blog Post on medium. You can use the link below to access the blog post https://medium.com/@patlichengine/my-first-data-science-blog-post-365784c0d189

## 1. Business Understanding: 
   This specifies what we want to accomplish from a business perspective. For the chosen dataset, we are expected to identify 3 questions that would address      business need and      use the data to solve them. The following questions would be answered:
   * How does user from each location respond to the different review categories and which rooms were visited the most?
   * In what way did the reviews affect the revenue of the company?
   * What policy affected the choice of review on the site and in which was do they visitors respond to the reviews.

## 2. Data Understanding:
   This stage deals with the data with the data which would be used to support the solution of the business problem stated above. This data source was            provided though the Udacity nanodegree program. To get a understanding of the data, I downloaded the three data sources as follows:
   * Listing dataset
   * Review dataset and
   * Calender dataset
   This datasets were inspected to understand the composition using Pandas Dataframe function. The sample of the data is shown below:
   ![Data Understanding](https://miro.medium.com/max/875/1*pVf6vajlI7_dNooZNccMCA.jpeg)
   
## 3. Data Preparation:
   This step entails organizing data in a way it will help to answer business questions of interest. It involves handling missing values, data cleaning,          categorizing data, aggregation, formatting, etc. Example of such cleaning function is shown below:
   ```python
   #create a function to clean the currency field
   def clean_currency(x):
      """ If the value is a string, then remove currency symbol and delimiters
      otherwise, the value is numeric and can be converted
      """
      if isinstance(x, str):
          return(x.replace('$', '').replace(',', ''))
      return(x)
   ```
   Hence the two dataset was merged in order to get meaningful data and prices of product. Since the price field contained some currency symbols,        I        used a python function    to cleaning the field. See sample of agregated data below:
   ![Data Preparation](https://miro.medium.com/max/751/1*WzLHn5BYP9DGMU9C3OXXRw.jpeg)
   
## 4.  Data Modelling:
   To answer some of the questions enumerated in the Business Understanding phase, I used the Naive Bayes algorithm. The choice of this models was due to its    Simpler (easy to      understand methods and easy to interpret results), Speed (very fast to learn from the data provided) Less data (it does not require      as much training data) characteristics        which also helped me to focus on the dataset available to provide answers based on specific attributes in the    dataset. For more information, you ca visit my Medium page.
   ![My Medium page](https://medium.com/@patlichengine/my-first-data-science-blog-post-365784c0d189)
    
## 5. Evaluate the Resultts
   Since the Naive Bayes algorithm is a parametric Machine Learning algorithm is used the major the price, location, review data and listing data to estimate    the statistics data needed to answer available questions. Using Pandas Dataframe functions, I was also to run some analysis using the data as                  presented on [My Medium page](https://medium.com/@patlichengine/my-first-data-science-blog-post-365784c0d189)

## Project Installation:
    To install the project, follow the following steps:
    * Clone the project from the GitHub repository
    * Ensure that Python is installed, then configure a virtual environment (preferable) and install Jupiter Notebook (if you are running the app locally)
    * From the GitBash command line terminal, workon to the notebook virtual environment
    * Run jupyter notebook on the terminal
    * Open the python file named: Air_BnB_Data_Findings.ipynb and run the project
    
## Project motivation
    The Udacity Data Science Nanodegree programme has actually been a greate inspiration which also introduced this project and exposed me to specific             Industry principle used in solving business problems (CRISP-DM). This has helped me explore other areas on the standard to also gain more knowledge on its     implementation. You can read more about the [Nanodegree Program here](https://www.udacity.com/course/data-scientist-nanodegree--nd025)
    
## File descriptions:
    The following file types are available in the repository:
    * Python code file
    * CSV files containing datasets for running the project, etc
    
## Results:
    For more result on the project, [click here](https://medium.com/@patlichengine/my-first-data-science-blog-post-365784c0d189)
    
## Acknowledgments
    ![link](https://reviews.udacity.com/static/media/logo.7630e043.svg) Udacity has been very tremendous and my Counrse mentor has provided some insight           throught the Udacity Project review that have helped me make necessary changes to this Read Me.
    
