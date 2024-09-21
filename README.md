Data analysis of a real Czech bank. 

### Motivation
The notebook contains an overview of the following questions and even more than that: 
- An overview of the age and gender distribution among customers.
- Can we pinpoint the most promising districts in the Czech Republic for future marketing efforts? Key factors include a larger population, higher average salaries, and lower client representation.
- A review of the credit department's performance across the country: which districts are primarily issuing "good" or "bad" loans?
- An analysis of the bank's cash inflows and outflows: does the bank frequently experience negative cash flow, and are there any discernible patterns in how funds are allocated?

### Install
This project requires Python 3. x and the following Python libraries installed:

1. NumPy
2. Pandas
3. Matplotlib
4. Seborn 
5. Plotly 
6. Collections 

You will also need to have software installed to run and execute an iPython Notebook



### Data 
The dataset comes from a real Czech bank and covers the period from 1993 to 1998, with data collected in 1999. It includes various relationships related to clients and their accounts:

- **Account**: Contains 4,500 records in ACCOUNT.CSV, each detailing the static characteristics of an account.
- **Client**: Features 5,369 records in CLIENT.CSV, describing the characteristics of each client.
- **Disposition**: Links clients to accounts in DISP.CSV, detailing the rights clients have to operate those accounts (5,369 records).
- **Permanent Order**: Includes 6,471 records in ORDER.CSV, describing the characteristics of payment orders.
- **Transaction**: Contains 1,056,320 records in TRANS.CSV, each representing a single transaction on an account.
- **Loan**: Features 682 records in LOAN.CSV, detailing loans granted for specific accounts.
- **Credit Card**: Includes 892 records in CARD.CSV, describing credit cards issued to accounts.
- **Demographic Data**: Comprises 77 records in DISTRICT.CSV, providing demographic characteristics of different districts.

Each account has both static attributes (such as creation date and branch address) detailed in the "account" relation and dynamic attributes (like debits, credits, and balances) found in the "permanent order" and "transaction" relations. The "client" relation outlines the characteristics of individuals who can manage the accounts. One client may hold multiple accounts, and multiple clients can operate a single account, with these relationships mapped in the "disposition" relation. The "loan" and "credit card" relations describe the bank's offerings, where multiple credit cards can be issued per account, but only one loan can be assigned to an account. Lastly, the "demographic data" provides publicly available information about districts, such as unemployment rates, which can help infer additional details about clients.

Data map 

![data map.gif](https://view.dwcontent.com/file_view/lpetrocelli/czech-financial-dataset-real-anonymized-transactions/data%20map.gif?auth=eyJhbGciOiJIUzUxMiJ9.eyJzdWIiOiJwcm9kLXVzZXItY2xpZW50OnRhbGdhdCIsImlzcyI6ImFnZW50OnRhbGdhdDo6ZGRkNjczOGItMjE3My00ZjJmLWJlMzctOTIxNTU2MzgyYWNhIiwiaWF0IjoxNTQ5MjcyMzc5LCJyb2xlIjpbInVzZXIiLCJ1c2VyX2FwaV9hZG1pbiIsInVzZXJfYXBpX3JlYWQiLCJ1c2VyX2FwaV93cml0ZSJdLCJnZW5lcmFsLXB1cnBvc2UiOmZhbHNlLCJ1cmwiOiJlYjA3MWQ2ODY4N2Y3NmY4NzM0ZGUzM2MzZjk3MTIzNDgxOWYwZTBjIn0.1bYEPgFwBlTGWf40nJzSdDyDJbi7YYqPJ-K-yeYOZ7SSc8rkMSc-ubQFbRoFZiQrhvoHpgzyq_mvON_Xo7MQBA)

### Data dictionary 

List of datasets and data dicitonary can be found in Data dictionary.pdf

### Run
In a terminal or command window, navigate to the top-level project directory czech-banking-fin-analysis/ (that contains this README) and run one of the following commands:

ipython notebook Czech-banking-customer-trans-analysis.ipynb
or

jupyter notebook fCzech-banking-customer-trans-analysis.ipynb
This will open the iPython Notebook software and project file in your browser.

### Acknowledgement

I want to express my gratitude to @lpetrocelli for providing the real Czech bank data available at [data.world](https://data.world/lpetrocelli/czech-financial-dataset-real-anonymized-transactions), and to TSilveira for the valuable data visualization examples shared on [Kaggle](https://www.kaggle.com/tsilveira/applying-heatmaps-for-categorical-data-analysis).

### License 
Code released under the MIT License. 
