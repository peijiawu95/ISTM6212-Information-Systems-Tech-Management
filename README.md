# ISTM6212-Federal Election Commission Data Warehouse Design
### Our team used the open data source on FEC to answer the interesting questions listed below. 

## Data Source
The data was sourced from Federal Election Commission which reveals how the candidates and committees raised and spent money in the elections. 
https://www.fec.gov/data/browse-data/?tab=bulk-data

Only the following data were used:
* All Candidates (https://www.fec.gov/campaign-finance-data/all-candidates-file-description/)
* Candidate Master (https://www.fec.gov/campaign-finance-data/candidate-master-file-description/)
* Committee master (https://www.fec.gov/campaign-finance-data/committee-master-file-description/)
* Contributions from committees to candidates file description (https://www.fec.gov/campaign-finance-data/contributions-committees-candidates-file-description/)

# Problem of Interest
* What are the names of the top 5 committees which contributed the single highest amount to Joe Biden and Donald Trump in 2020, and Hillary Clinton and Donald Trump in 2016?
* What are the top 5 candidates from the Democratic party that received the highest amount of total contributions from committees in 2020 and 2016? What are the top 5 candidates from the Republican party that received the highest amount of total contributions from committees in 2020 and 2016?
* Which state contributed the most to Joe Biden, and which state contributed the most to Donald Trump in 2020?

# Methodology 
1. Using Trifacta wrangle and clean all required datasets and integrated them into one dataset, saved in S3 bucket. 
2. Design Dimension and fact schema. 
3. Create table and load data using Spark SQL.
4. Using Spark SQL query the answers for the above questions.
5. Output the answers and use Tableau to present them. 
