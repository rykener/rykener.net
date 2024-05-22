---
date: 2023-01-10 07:30:35 +0300
title: Product Recommendation Pipeline for a Food Delivery Online Marketplace
subtitle: Data Analysis
image: '/images/food_recs.jpg'
---

### Problem

An online delivery marketplace aimed to boost its revenue by integrating data-driven improvements into its user experience. After evaluating the data availability and practicality of various use cases, we decided to initiate a proof-of-concept initiative focusing on product recommendations within the food segment.

In 2023, the food segment generated over $6 million from 205,000 orders on the marketplace. The company had underutilized data that wasn't leveraged for analytics or data-driven decisions, and the user interface lacked personalized recommendations. The client aimed to use data science to enhance the user experience with personalized food recommendations.

### Solution

Drawing inspiration from [Uber Eats’ advanced recommendation techniques](https://www.uber.com/en-CH/blog/uber-eats-recommending-marketplace/), we designed a proof-of-concept product recommendation pipeline combining content-based and collaborative filtering methods to deliver personalized food suggestions. The development process included several key steps:

1. **Data Collection**: Extract and manipulate relevant user and product data, converting information into tabular data for in-depth analysis.
2. **Exploratory Data Analysis (EDA)**: Conduct a comprehensive exploratory data analysis to identify patterns and relationships within the data.
3. **Content-Based Filtering**: Create user and food taste profiles, and calculate similarity scores between user tastes and product profiles.
4. **Collaborative Filtering**: Leverage users’ purchase histories to identify products favored by similar users.
5. **Hybrid Approach**: Integrate content-based and collaborative filtering techniques to recommend items based on previous preferences and popular items among similar users.

![Product Recommendations explained](/images/prod_recs.jpg)

{:.image-caption}
*The conceptual difference between content-based and collaborative filtering techniques*

### Tools Used

- **MongoDB:** Primary database for storing user and product data.
- **Python:** The primary programming language for developing the recommendation algorithms and performing data analysis.
- **Pandas:** Utilized for data manipulation and analysis to convert raw data into insights.
- **Matplotlib:** Primary library used to visualize data trends and algorithmic outputs.
- **Sklearn (DictVectorizer):** Used for encoding categorical data into numerical vectors, critical for our machine learning models.

### Outcome

The proof-of-concept recommendation pipeline demonstrated the potential to implement complex AI-driven solutions in real-world scenarios. Its success marks a promising step towards extending recommendation services to other segments of the marketplace, potentially transforming the shopping experience for customers across various categories. Additionally, this initiative highlights the importance of well-structured, ordered, and maintained data for making data-driven decisions. It also reveals gaps in existing data pipelines that, once addressed, could further refine the user experience.