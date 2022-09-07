# Automatic Customer Complaint Classification

## Problem statement
For a financial company, customer complaints carry a lot of importance, as they are often an indicator of the shortcomings in their products and services. If these complaints are resolved efficiently in time, they can bring down customer dissatisfaction to a minimum and retain them with stronger loyalty. This also gives them an idea of how to continuously improve their services to attract more customers. 

These customer complaints are unstructured text data; so, traditionally, companies need to allocate the task of evaluating and assigning each ticket to the relevant department to multiple support employees. This becomes tedious as the company grows and has a large customer base.

## Business goal

Create a model that can automatically classify customer complaints based on the products and services that the ticket mentions. By doing so, the financial company can segregate these tickets into their relevant categories and, therefore, help in the quick resolution of the issue.

## Approach
With the help of non-negative matrix factorization (NMF), an approach under topic modelling, we can detect patterns and recurring words present in each ticket. This can be then used to understand the important features for each cluster of categories. By segregating the clusters, we will be able to identify the topics of the customer complaints. 

Since this data is not labelled, we need to apply NMF to analyse patterns and classify tickets into the following five clusters based on their products/services:

- Credit card / Prepaid card
- Bank account services
- Theft/Dispute reporting
- Mortgages/loans
- Others 

Once the mapping is done, we can then use this data to train any supervised model such as logistic regression, decision tree or random forest. Using this trained model, you can classify any new customer complaint support ticket into its relevant department.

## Dataset

The dataset is available in the [complaints.zip file](https://github.com/lasrado/Auto_Ticket_Classification/raw/main/complaints.zip). Uncompress the zip file to extract the .json file.

The dataset given is in the .json format and contains 78,313 customer complaints with 22 features. We need to convert this to a dataframe in order to process the given complaints.

## Technologies Used
- The project is built on python using numpy, pandas.
- The project used spacy and nltk libraries.
- sklearn is used to build and evaluate the models.

## Contact
Created by [@lasrado] - feel free to contact me!