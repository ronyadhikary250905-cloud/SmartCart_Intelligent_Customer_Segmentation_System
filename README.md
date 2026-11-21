# SmartCart – Intelligent Customer Segmentation System Using Unsupervised Machine Learning

## Project Overview

SmartCart is an intelligent customer segmentation project that uses
Unsupervised Machine Learning to identify different customer groups
based on their demographics, income, purchasing behaviour, spending
patterns, and website activity.

The objective is to help an e-commerce platform understand its
customers better by grouping them into meaningful segments.

Instead of treating all customers equally, this project identifies
distinct customer profiles and suggests targeted business strategies
to improve customer engagement, conversions, and retention.

## Problem Statement

SmartCart is a growing e-commerce platform serving customers across
multiple countries. It has collected customer data containing
demographic information, purchase behaviour, website activity,
and campaign responses.

However, the platform treats all customers similarly without
understanding their different purchasing behaviours.

The goal is to apply Unsupervised Machine Learning techniques to
discover meaningful customer segments and develop data-driven
marketing strategies for each group.

## Dataset Information

- Total Records: 2,240 customers
- Total Features: 22
- Dataset File: smartcart_customers.csv

The dataset contains information related to:

- Customer demographics
- Education and marital status
- Income
- Product spending patterns
- Purchase frequency
- Shopping channel preferences
- Website visits
- Campaign responses

## Technologies Used

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Kneed

## Project Workflow

### 1. Data Loading and Exploration

- Imported the customer dataset using Pandas.
- Examined dataset dimensions and initial records.
- Identified missing values and explored the available features.

### 2. Data Preprocessing

- Handled missing Income values using median imputation.
- Checked and handled outliers.
- Removed unnecessary columns.

### 3. Feature Engineering

Created meaningful features from existing customer information:

- Age
- Customer Tenure (Days)
- Total Spending
- Total Children

Also simplified categorical features:

- Education levels
- Living status (Alone / Partner)

### 4. Outlier Detection and Handling

Used visual analysis and feature-based filtering to handle
extreme values in Age and Income.

### 5. Correlation Analysis

- Examined relationships between numerical features.
- Used a correlation heatmap to understand feature relationships.

### 6. Categorical Encoding

Applied One-Hot Encoding to convert categorical features
into numerical representations.

### 7. Feature Scaling

Applied StandardScaler to standardize numerical features
before dimensionality reduction and clustering.

### 8. Dimensionality Reduction – PCA

Applied Principal Component Analysis (PCA) to reduce the
feature space to three principal components.

Used a 3D visualization to explore the transformed data.

### 9. Finding the Optimal Number of Clusters

Used two evaluation techniques:

- Elbow Method (WCSS)
- Silhouette Score

Also used KneeLocator to identify the elbow point.

### 10. Customer Clustering

Implemented two clustering algorithms:

- K-Means Clustering
- Agglomerative Clustering

Both models were configured to identify four customer clusters.

### 11. Cluster Analysis

Analyzed the resulting customer groups using:

- Cluster distribution
- Income and spending patterns
- Purchase behaviour
- Shopping channel preferences
- Website activity
- Campaign response

## Customer Segments Identified

The project identified four distinct customer segments:

### Cluster 0 – Low-Spending Partner Customers

- Average Income: ₹39,681
- Average Total Spending: ₹222
- Prefer physical store shopping.
- Have more website visits but fewer online and catalog purchases.

**Business Strategy:**
Offer discounts, personalized product recommendations,
and promotional campaigns to encourage purchases.

### Cluster 1 – High-Value Partner Customers

- Average Income: ₹72,808
- Average Total Spending: ₹1,237
- Frequently purchase through web, catalog, and physical stores.
- Show strong purchasing activity.

**Business Strategy:**
Provide loyalty rewards, premium offers, and exclusive
product recommendations to retain valuable customers.

### Cluster 2 – Low-Spending Customers Living Alone

- Average Income: ₹36,960
- Average Total Spending: ₹166
- Make fewer purchases across shopping channels.
- Have the highest average website visits.

**Business Strategy:**
Use targeted discounts, personalized suggestions,
and engaging marketing campaigns to increase conversions.

### Cluster 3 – High-Value Customers Living Alone

- Average Income: ₹70,723
- Average Total Spending: ₹1,190
- Frequently purchase through online, catalog, and physical stores.
- Have the highest campaign response rate (32%).

**Business Strategy:**
Focus on customer retention, personalized campaigns,
premium services, and cross-selling opportunities.

## Key Learnings

Through this project, I explored and implemented:

- Data Cleaning and Preprocessing
- Missing Value Imputation
- Feature Engineering
- Outlier Handling
- Correlation Analysis
- One-Hot Encoding
- Feature Scaling
- Principal Component Analysis (PCA)
- Elbow Method
- Silhouette Score
- K-Means Clustering
- Agglomerative Clustering
- Cluster Characterization
- Data Visualization
- Business Insights from Customer Segmentation

## Conclusion

SmartCart demonstrates how Unsupervised Machine Learning can
transform raw customer data into meaningful customer segments.

By identifying four distinct customer groups, the project
provides insights into customer spending habits, income levels,
shopping preferences, and campaign responses.

These insights can help businesses develop targeted marketing
strategies, improve customer engagement, increase conversions,
and build stronger customer relationships.

---

**Project Name:** SmartCart – Intelligent Customer Segmentation System

**Domain:** Unsupervised Machine Learning

**Algorithm Focus:** K-Means and Agglomerative Clustering
