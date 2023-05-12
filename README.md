# mini-project-III
Repo with the instructions for the Mini Project III.


### Topics
This mini project is dedicated to following topics:

Data Wrangling:

We first had to get an understanding of the data available
 - We have two types of sheets. 
 - Accounts information 
 - Transaction information
 - We created a excel file that listed all dataframes and their connection to each other (located in the powerpoint)
 

Data cleaning:

 - We checked the dataset for null values
 - We explored the dataset for customer accounts information and transaction information
 - We imported the sheets and created two dataframes. One for customer accounts and other for transaction. Tables are joined    using cust_id.

Data Visualization:
 - We visualized the data with by creating pair-plots, bar graphs, and histograms. 
 

Data Preparation and Feature Engineering
- We created our own features by combining features such as states into regions. Debt-usage by combining credit limit and credit balance. 

Dimensionality Reduction
- We used PCA for dimensionality reduction (results in power-point and notebooks)

Unsupervised Learning
- K-means clustering, PCA, hierarchial clustering located in the notebooks. 

### Data
We will be using old data about different financial transactions. You can download the data from [here](https://drive.google.com/file/d/1zAjnf936aHkwVCq_BmA47p4lpRjyRzMf/view?usp=sharing). The data contains following tables:

- twm_customer - information about customers
- twm_accounts - information about accounts
- twm_checking_accounts - information about checking accounts (subset of twm_accounts)
- twm_credit_accounts - information about checking accounts (subset of twm_accounts)
- twm_savings_accounts - information about checking accounts (subset of twm_accounts)
- twm_transactions - information about financial transactions
- twm_savings_tran - information about savings transactions (subset of twm_transactions)
- twm_checking_tran - information about savings transactions (subset of twm_transactions)
- twm_credit_tran - information about credit checking (subset of twm_transactions)


### Output

In this miniproject, we will:

1.  create two separate customer segmentations (using clustering) to split them into 3-5 clusters: 
    - based on demographics (only on the information from twm_customer)
    - based on their banking behavior. We can take following things into consideration as banking behavior:
        - do they have savings account? How much do they save?
        - do they have credit account? How much do they live in debt?
        - are they making lot of small transactions or few huge ones?
        
 
2. visualize the created clusters using [radar charts](https://plotly.com/python/radar-chart/) and compare them agains each other
3. visualize segmentations using scatter plot. We will have to use PCA to be able to plot our observations in 2D.


### Visualizations are located in the notebooks and power-point



### RESULTS:

Banking behaviour: 

Cluster 0: 241 in cluster, individuals with credit cards, higher debt usage, slightly lower income average, makes more transactions of medium amounts.

Cluster 1: 281 in cluster, majority individuals without credit cards, very low debt usage,  lower savings balance, less transactions of lower amounts.

Cluster 2: 225 in cluster, higher income, individuals with credit cards and low debt usage, highest savings balance, makes medium amount of transactions with larger average amounts.


Customer demographics:

Cluster 0: 253 in cluster, average age of 62, medium average income,  

Cluster 1: 240 in cluster, average age of 22, lower average income. 

Cluster 2: 254 in cluster, average age of 41, higher income, higher average of number of children

