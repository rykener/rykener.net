---
date: 2023-01-10 07:30:35 +0300
title: Product Recommendation Pipeline for a Food Delivery Online Marketplace
subtitle: Data Analysis
image: '/images/food_recs.jpg'
---

### Problem

The client was exploring data-driven enhancements to user experience and profitability within its online delivery marketplace. Four use cases were identified: product recommendation, delivery time prediction, dynamic fare pricing, and delivery route optimization. After evaluating the availability of data and feasibility of each case, product recommendation for the food segment was selected for a proof-of-concept initiative.

The food segment alone accounted for over 205,000 orders in 2023, generating approximately $6 million in revenue to the company. Despite its success, the existing interface lacked any types of recommendations. The client's objective was to improve user experience by providing personalized food recommendations, inspired by advanced techniques such as those detailed in [Uber Eats’ approach to recommendations](https://www.uber.com/en-CH/blog/uber-eats-recommending-marketplace/).

### Solution

A proof-of-concept product recommendation pipeline was designed that combined content-based and collaborative filtering methods to deliver personalized food suggestions. The development process began with the extraction and manipulation of relevant user and product data from MongoDB, which was then parsed into pandas DataFrames for detailed analysis. The solution involved:

- **Exploratory Data Analysis (EDA):** We conducted thorough exploratory data analysis to uncover patterns and relationships within the data, essential for refining our recommendation strategies based on real user behaviors and product characteristics.
- **Content-Based Filtering:** User and food taste profiles were developed using extracted features from product descriptions and user preferences. These profiles were transformed into numerical vectors using sklearn’s DictVectorizer, enabling us to calculate similarity scores between user tastes and product profiles.
- **Collaborative Filtering:** This method utilized users’ purchase histories to identify products favored by similar users, thus dynamically capturing changing user preferences.
- **Hybrid Approach:** The integration of content-based and collaborative filtering allowed our engine to suggest food items similar to those previously liked by the user, as well as new items popular among similar users, enhancing both accuracy and discovery.

### Tools Used

- **MongoDB:** Primary database for storing user and product data.
- **Python:** The primary programming language for developing the recommendation algorithms and performing data analysis.
- **Pandas:** Utilized for data manipulation and analysis to convert raw data into insights.
- **Matplotlib:** Primary library used to visualize data trends and algorithmic outputs.
- **Sklearn (DictVectorizer):** Used for encoding categorical data into numerical vectors, critical for our machine learning models.

### Outcome

The proof-of-concept recommendation pipeline showcased the capacity to implement complex AI-driven solutions in real-world scenarios. The success of this pipeline is a promising step toward expanding recommendation services to other segments of the marketplace, potentially revolutionizing the shopping experience for customers across various categories.

The proof-of-concept will be implemented in the coming weeks in a sandbox environment of the marketplace. This will allow us to simulate real-world usage more closely and make necessary adjustments before full deployment.