# Module21_Deep-Learning-Challenge
Alphabet Soup - Deep Learning Challenge - Week 19 - Data Analytics Boot Camp - University of Oregon

## Background
The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. With machine learning and neural networks, I'm using the features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

From Alphabet Soup’s business team, I have received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization, such as:

- **EIN** and **NAME—Identification** columns
- **APPLICATION_TYPE** — Alphabet Soup application type
- **AFFILIATION** — Affiliated sector of industry
- **CLASSIFICATION** — Government organization classification
- **USE_CASE** — Use case for funding
- **ORGANIZATION** — Organization type
- **STATUS** — Active status
- **INCOME_AMT** — Income classification
- **SPECIAL_CONSIDERATIONS** — Special considerations for application
- **ASK_AMT** — Funding amount requested
- **IS_SUCCESSFUL** — Was the money used effectively

# Approach

This project was initially created in [Google Colab Project](https://colab.research.google.com/drive/1oVZ4ZpVErVYIB_9UTXLzWDW00broKoRK?usp=sharing).  A copy has been downloaded to GitHub for easy reference.


**Data Preprocessing**
- I dropped the *EIN* and *NAME—Identification* columns as they have no revelence to what we're evaluating
- I reduced the number of values in *APPLICATION_TYPE* and *CLASSIFICATION* by categorizing smaller segments into an "other" label.
- I expended categorial variables with pd.get_dummies()
- We're using the *IS_SUCCESSFUL* column as our target for X
- We kept all of the other datapoints to be evaluated for Y
- I split the data into training ad testing datasets.
- I scaled the training and testing features uinsing StandardScaler before fitting it to the model.


**Compiling, Training & Evaluating**



Summary



# Result