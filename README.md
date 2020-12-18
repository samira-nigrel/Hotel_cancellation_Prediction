Hotel Cancellation Prediction

[TOC]

Executive Summary
Our goal is to build a model able to classify a booking as canceled or not canceled. In order to do so, we used data from the Hotel Booking Demand Datasets. The dataset provides data from real bookings scheduled to arrive between July, 1st 2015 and August, 31st 2017 from two hotels in Portugal (a resort in the Algarve region (H1) and a hotel in the city of Lisbon (H2)). Booking data from both hotels share the same structure, with 31 variables describing the 40,060 observations of H1 and 79,330 observations of H2. For a detailed list and description of those variables refer to the data dictionary. The two hotel datasets were merged into one main dataframe. The dataframe was then cleaned making sure to address any null values, reformat certain features, and engineer new ones. Exploratory analysis included analysis of the cancellation target variable and its relation with other features. Data visualisation tools were used to identify trends and valuable insights from those analysis. A Random forest Classifier model was then used in order to identify the accuracy of the model. The models were evaluated, and conclusions and recommendations were derived to optimize occupancy, improve operations, and increase a hotel's revenue.

Quick Problem Overview
1. Who is our stakeholder? - Booking Manager
2. What is the core business problem we are solving? - Revenue Management, cost implications due to cancellations.
3. Convert Business to DS Problem: Determine if a booking will be canceled or not. And what leads to cancellations.
4. Business Metric: How much Overbookings can we take ( based on reliable cancelation predictions from the model)
5. Data Science Metric: Recall/ Precision/ F1 Score
6. Feature Selection: Done
7. Feature Engineering: Done
8. EDA Questions: Done

Markup :  #### Problem with Cancellations####

1. Customer accustomed to free cancellation policies
2. Operational Problems
3. Non accurate forecast
4. Non-optimized Occupancy
5. Poor Management
6. Revenue Loss

In order to fight the negative impact of cancellations, hotels need to be able to identify which bookings are likely to be cancelled.

Here the solution will allow hotels/resorts to predict if a new booking will be cancelled or not, manage their business accordingly, and increase their revenue.

The Data & Dictionary
From: Property Management System

Bookings are due to arrive between July 01, 2015 and August 31, 2017.

