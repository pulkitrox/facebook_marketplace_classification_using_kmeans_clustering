# 📘 Facebook Marketplace Analysis

## 📌 Project Overview
This project performs an in-depth exploratory and analytical study of **Facebook Marketplace post data** to understand user engagement patterns and identify natural groupings of posts using clustering techniques. The analysis combines statistical insights with machine learning to derive actionable social media strategy recommendations.

The dataset represents real-world activity from Facebook pages of fashion and cosmetics sellers, making the findings highly relevant for digital marketing and data science applications.

---

## 🎯 Objectives
- Analyze how **posting time** affects user engagement
- Study correlations between reactions, comments, and shares
- Compare engagement across different **post types**
- Segment posts into meaningful clusters using **unsupervised learning**
- Provide data-driven insights for optimizing content strategy

---

## 📁 Dataset Description
- **Source:** UCI Machine Learning Repository  
- **Context:** Facebook pages of 10 Thai fashion & cosmetics sellers  
- **Initial Size:** 7050 instances, 16 attributes  
- **Final Dataset:** 12 attributes after cleaning  

### Key Features
- Post type (`photo`, `video`, `status`, `link`)
- Engagement metrics: reactions, comments, shares, likes, loves, wows, hahas, angrys
- Timestamp of post publication

---

## 🧹 Data Preprocessing
The following preprocessing steps were applied:
- Removed redundant columns with excessive missing values
- Converted publication timestamps to datetime format
- Imputed missing numerical values using mean strategy
- Engineered new features (e.g., **posting hour**)
- Applied One-Hot Encoding to categorical variables
- Scaled numerical features using **StandardScaler**

---

## 📊 Key Analysis & Insights

### ⏰ Impact of Posting Time
- Posts published between **6 AM – 8 AM** receive the highest average reactions
- Early-morning posting maximizes visibility and engagement

### 🔗 Correlation Between Engagement Metrics
- Strong positive correlation between **comments and shares (~0.64)**
- Moderate correlation between **reactions and shares**
- Highly shareable posts tend to spark more discussion

### 🖼️ Distribution of Post Types
- **Photos** dominate the platform
- **Videos** are the second most common
- Status and link posts are comparatively fewer

### 📈 Average Engagement by Post Type
- **Videos:** Highest average comments and shares (strong virality)
- **Status posts:** Highest average reactions
- **Link posts:** Good reach with passive engagement

---

## 🤖 Clustering Methodology
- **Algorithm:** K-Means Clustering
- **Features Used:** Encoded post type + all engagement metrics
- **Scaling:** StandardScaler
- **Optimal Clusters:** Determined using the **Elbow Method**

### 🔍 Clustering Result
- Optimal number of clusters: **3–4**
- Represents Low, Medium, and High engagement segments
- Enables targeted content strategy for each engagement group

---

## 📂 Repository Structure
```
├── facebook_marketplace.ipynb
├── Facebook-Marketplace-Analysis.pptx
├── README.md
├── Facebook_marketplace_data.csv
```

---

## 🛠️ Technologies Used
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- Jupyter Notebook

---

## 📌 Key Takeaways
- Visual content (photos & videos) drives engagement
- Early-morning posts perform best
- Shares and comments amplify each other
- Engagement patterns naturally cluster into distinct groups

---

## 🚀 Future Enhancements
- Try alternative clustering algorithms (DBSCAN, Hierarchical)
- Include sentiment analysis on comments
- Extend analysis to other social media platforms
- Deploy insights via an interactive dashboard

---

This project demonstrates practical application of data analysis and unsupervised learning techniques to solve real-world social media engagement problems.
