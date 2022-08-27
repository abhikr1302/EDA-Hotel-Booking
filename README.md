# Introduction

The success factoring a profitable hotel industry has been changing over time, driven by global competition and increasingly high customer expectations. Hotels focus on customer satisfaction and to exceed customer expectations. 
We have a hotel booking dataset containing information for city and resort hotels. This dataset has 32 variables with around 1,19,000 entries. It is collected in order to predict hotel bookings and its probability of cancellation. Some attributes here are to understand what factors do bring in the revenue for the business. Some attributes show the customers preference for booking whereas some attributes show the factors leading to cancellations.
We have a hotel booking dataset. We are using our Python skills to perform EDA and gain informative insights about factors in hotel bookings and how they affect hotel bookings.

# Project Goal

This data set contains booking information for a city hotel and a resort hotel, and includes information such as when the booking was made, length of stay, the number of adults, children, and/or babies, and the number of available parking spaces, among other things. Purpose of our study is to find the best time to book a hotel room. The optimal length of stay in order to get the best daily rate. Study on special requests.We explore and analyze the data to discover important factors that govern the bookings.

# Exploratory Data Analysis:-

First step is to import libraries such as NumPy, pandas, matplotlib, seaborn.Then load the raw dataset. This data has many unprocessed values which cannot be considered for the study. Here is the workflow of correcting it for our analysis.

# Data Cleaning

## Handling Null Values
Company Id and Agent Id: - These columns have null values of 93% and 15% respectively. Hence, these columns are dropped.

Country: - This has null values less than 5% thus the null values are filled with the mode value.

Children and babies: - There are only 4 null values so the null value is filled with mean
 
## Handling Outliers
An outlier is an extremely high or extremely low data point relative to the nearest data point and the rest of the neighboring co-existing values in a data graph or dataset we work with. 
We have used the Interquartile range method to handle outliers. To find the interquartile range (IQR), ​we first find the median (middle value) of the lower and upper half of the data. These values are quartile 1 (Q1) and quartile 3 (Q3). The IQR is the difference between Q3 and Q1.

# Data Manipulation
## Creating new columns
Kids= Children +babies 

Total stay= stays_in_weekend_nights+ stays_in_week_nights 

Guest= Adults+kids 

Revenue= stay of non-cancelled guests * ADR
 
# Data study
i) UNIVARIATE ANALYSIS: 
Univariate analysis is the simplest form of analyzing data i.e study of one variable. Its major purpose is to describe; distribution of single data, and find patterns in the data.

ii) BIVARIATE ANALYSIS:
Bivariate analysis between two variables. One of the variables will be dependent and the other is independent. The study is analyzed between the two variables to understand to what extent the change has occurred.

iii) MULTIVARIATE ANALYSIS
Multivariate data analysis is the study of relationships among the attributes, classify the collected samples into homogeneous groups, and make inferences about the underlying populations from the sample.

# Data Visualization :-

Data visualization is the practice of translating information into a visual context, such as a map or graph, to make it easier to understand and gain insights from them. 
The graphs used here for study are: -

Box Plot. 

Histogram. 

Pie Chart. 

Bar Plot. 

Line Plot. 

Scatter Plot. 

Geo Mapping. 

# Conclusion

Resort hotels are more expensive as compared to City hotels.

People prefer city hotels for shorter stay and resort hotels for longer stay.

Best time to book a resort hotel is from October to April and best time to book a City hotel is from November to March.

Maximum number of bookings and cancellations are done in the month of August.

Both hotel types are getting higher revenue between June to September.

As lead time and total stays increases ADR decreases. This means if a customer book a hotel in advance or stays for a longer duration, he can get a better deal.

Hotels having refundable policy are expensive whereas hotel with no-refund policy are cheaper.

Majority of the bookings and cancellations are made through Travel agencies and Tour Operators.

Cancellation is more in City hotels as compared to Resort hotels.

Every year there is 25-30% cancellation for resort hotels and 40-45% cancellation for city hotels.

Majority of the people prefer the BB (bed & breakfast) meal in both the hotel types.

