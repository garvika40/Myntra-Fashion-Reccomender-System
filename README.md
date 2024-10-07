# Myntra Fashion Data Analysis and Recommendation System

**Project:** Analyzing Myntra Fashion Trends & Building a Recommendation System  

## Overview

This project involves the analysis of Myntra's fashion data, exploring various trends in the fashion industry such as discount patterns, popular brands, and material preferences. In addition, we implemented a collaborative filtering recommendation system to generate personalized product suggestions for users.

### Dataset

The dataset used is from Myntra, containing 15,000 rows and 27 columns, covering aspects like product ratings, brand, size, material, and discount.

- **Source:** Myntra Fashion Data
- **Key Columns:**  
  - `User_id`, `p_id`, `Ratings`, `brand`, `size`, `actual_color`, `variant_price`, `variant_compare_at_price`, `dominant_material`, `ideal_for`, `discount`

## Project Structure

### File 1: Exploratory Data Analysis (EDA)
- **Discount Calculation**
- **Category-wise Product Distribution by Gender**
- **Top 10 Popular Brands**
- **Brands Offering the Highest Discounts**
- **Top Selling Fabrics**
- **Top 7 Expensive Fabrics**
- **Discount Variations by Gender (Including Unisex)**
- **Top Selling and Least Sold Products**
- **Most Expensive Items**

### File 2: Recommendation System
- **Installations and Setup**
- **Data Preprocessing**
- **Popularity-Based Filtering**
- **Memory-Based Collaborative Filtering**
  - User-User Collaborative Filtering
  - Item-Item Collaborative Filtering
- **Train-Test Split**
- **Evaluation Metric:** RMSE (Root Mean Squared Error)
- **Cosine Similarity for Similarity Weights**
- **Model Evaluation and RMSE Comparison**
  - Collaborative Filtering Model: RMSE and Predicted Ratings
  - Top 10 Product Recommendations for Users
- **Model-Based Collaborative Filtering**
  - K-Nearest Neighbors (KNN)
  - Matrix Factorization (SVD)

## Collaborative Filtering Model Evaluation

### 1. **User-User Collaborative Filtering**
- **RMSE**: 0.4107

### 2. **Item-Item Collaborative Filtering**
- **RMSE**: 0.2685
- **Inference:** Item-Item CF outperforms User-User CF with a lower RMSE.

### 3. **K-Nearest Neighbors (KNN)**
- **k-value**: 10
- **Similarity Measure**: Cosine similarity
- **RMSE**: 0.4563  
- **MAE**: 0.3892

### 4. **Singular Value Decomposition (SVD)**
- **RMSE**: ~0.4471  
- **MAE**: ~0.3835
- **Inference**: SVD is more accurate and computationally efficient compared to KNN.

## Analysis & Insights

### Gender Distribution
- **Women**: 58.6%  
- **Men**: 28.3%  
- **Girls**: 4.69%  
- **Boys**: 4%  
- **Unisex**: 4.3%

### Popular Brands
- **Top Brands:** Anouk, Biba, Global Desi
- **Brands Offering Highest Discounts:** Aaeeah, Stylo Bug, I Am For You

### Material Preferences
- **Top Selling Fabrics:** Cotton, Viscose Rayon, Silk
- **Most Expensive Materials:** Velvet, Net, Tensil

### Discount Trends
- **Highest Average Discount:** Unisex, followed by Girls and Men


## Conclusion

- **Best Performing Model:** Item-Item Collaborative Filtering with RMSE of 0.2685
- **SVD Performance:** More accurate and computationally efficient compared to KNN.
- **Material Insights:** Cotton is the most popular fabric; velvet is the most expensive.



