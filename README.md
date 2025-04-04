# British Airways Customer Reviews & Sentiment Analysis - Web Scraping Project

![image](https://github.com/user-attachments/assets/d0bf7d38-bf5a-4ec4-855f-cfc6c0463c46)

# Table of Contents

[Description](#Description)\
[Objective](#Objective)\
[Business Problem](#Business-Problem)\
[Scope](#Scope)\
[Data Acquisition & Preparation](#Data-Acquisition-&-Preparation)\
[Data Overview](#Data-Overview)\
[Recommendations](#Recommendations)
[Tableau Dashboard](#Tableau-Dashboard)


## Description

British Airways (BA) is the UK’s flag carrier airline, with a vast global presence. Every day, thousands of BA flights connect passengers across the world, and the company is responsible for ensuring efficient and seamless operations from scheduling and boarding to landing, all while providing top-class customer service. Understanding customer feedback is critical for maintaining and improving the quality of service.

## Objective

This project aims to analyze customer reviews for British Airways to uncover key sentiment trends. By examining customer feedback, the goal is to help BA improve its customer service and address recurring issues that could enhance the overall customer experience.

## Business Problem

British Airways needs to better understand its customers in order to improve operations and enhance the overall customer experience. To achieve this, the company must gain insights into how customers perceive their experiences with the airline. Without a clear understanding of customer sentiment, BA may struggle to address issues effectively, leading to inefficiencies in operations and customer dissatisfaction.

## Scope

This project involves web scraping customer reviews from the [Skytrax](https://www.airlinequality.com/airline-reviews/british-airways/page/1/), followed by cleaning and processing the data. The cleaned data will be loaded into an SQL database for efficient storage and querying. Finally, a Tableau dashboard will be created to visualize key insights and trends from the reviews.

## Data Acquisition & Preparation

* Web Scraping - use BeautifulSoup (BS4) to scrape customer reviews from Skytrax
* Data Cleaning - clean the data with Python, Pandas, handling missing values and transforming it for analysis
* Sentiment Analysis:
  - TextBlob: Sentiment polarity and subjectivity
  - VADER SentimentIntensityAnalyzer: Sentiment score for short reviews
  - SpaCy & NLTK: Text processing (tokenization, lemmatization, stopword removal)
  - WordCloud: Visualize frequent words
  - Matplotlib: Plot sentiment trends and word frequencies.
* Data Storage - load cleaned data into an SQL database using SQLAlchemy.
* Dashboard Creation - create an interactive Tableau dashboard to visualize sentiment trends and insights.

## Data Overview

The dataset used for this project is based on real passenger reviews of British Airways flights, collected over a period from 2011 to 2025. The data includes reviews from various passengers across different routes, with detailed feedback on various aspects of their travel experience.

##### Collected data: date published, aircraft, type of traveller, seat type, route, date flown, route, review text, ranking (seat comfort, cabin staff, food & bevarages, ground service, value for money), recommended (yes/no), verification status

##### Derived data: departure, destination, layover, sentiment score, sentiment, keywords, word cloud:
<img width="454" alt="image" src="https://github.com/user-attachments/assets/54841a52-1d7d-42f4-88a0-caa1e9a1e27a" />

## Recommendations

### ✅ Address Top Complaints
  - Delays: Improve punctuality through better scheduling and contingency planning
  - Service & Food: Enhance in-flight service quality and food options
  - Comfort & Baggage Handling: Improve seating experience and baggage management efficiency

### ✅ Enhance Offerings
  - Economy Class shows flat service score trends — concern for long-term loyalty
  - Premium Economy is improving steadily — opportunity for targeted upselling
  - Business Travelers are least satisfied — likely due to higher expectations

### ✅ Improve Customer Service & Engagement
  - Cabin staff score (3.2/5) indicates improvement opportunities. More training and responsiveness to customer concerns can help
- Ground service (2.8/5) is also low—optimize airport assistance and check-in processes

### ✅ Monitor & Address Seasonal Trends in Negative Sentiment
  - High negative sentiment in July & October may indicate operational or service inefficiencies during peak travel times

### ✅ Increase Customer Loyalty & Retention Efforts
  - Given only 35.44% recommendation rate, focus on loyalty programs, compensation for delays, and better communication with passengers

## Tableau Dashboard

![image](https://github.com/user-attachments/assets/db4dba13-9557-4bbe-9956-176fe0ebef7a)

[🔗 Tableau Workbook:](https://public.tableau.com/app/profile/emilia.woldan6280/viz/CustomerExperienceDashboardforBritishAirlines/BASummary)

## Next Steps

- enhance project by adding ETL script
