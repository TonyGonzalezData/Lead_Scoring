# Lead Scoring

## Objective

Large companies often employ a multi-phase inbound sales model.

The challenge arises when the number of leads exceeds the capacity of the sales channels, especially those that require intermediary involvement:

- Overloading the channel
- Generating complaints from sales representatives
- Achieving less than optimal results
- 
Lead Scoring is a technique used to qualify leads and prioritize them, typically by applying business rules.

In this case, we will build a Lead Scoring model based on machine learning, which can be called by a client to qualify their leads.

Additionally, as added value, we will perform an unsupervised segmentation that will provide a better understanding of the type of leads the company is capturing, enabling us to offer tailored consulting recommendations.

> [!NOTE]  
> The entire project was developed in Spanish.
> 
> You can access the notebooks directly in this [folder](https://github.com/TonyGonzalezData/Forecasting_Retail/tree/main/03_Notebooks/02_Desarrollo).


## Project Structure

The development of the Discovery project consists of the following structure:

- **Set up**: We load the data from its original files, merge the necessary data from different tables and extract one dataset for validation and another for working purposes.
- **Data Quality**: Data cleaning, including review of data types and transformation of variables, handling of duplicates and null values.
- **EDA**: Exploraty data analysis of both categorical and numerical variables
- **Data transforation**: Creation of new variables and encoding of categorical variables.
- **Unsupervised Modeling**: We generate the unsupervised classification model that allows us to better understand the types of leads we are capturing and the groups in which we can classify them.
- **Variable preselection**: We select the most predictive variables. To do this, we choose the most reliable result among those obtained through the methods of Mutual Information, Recursive Feature Elimination, and Permutation Importance.
- **Modeling for regression**: We test the modeling process by first applying it to a single product. Then, we test the process on the entire set and verify that the results align with expectations.
- **Preparation of production code**: we combine all previously developed code, including the modeling, and make it ready for deployment.
