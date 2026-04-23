# 🛒 Personalized E-commerce Recommendation System

## 🧠 Project Overview

In modern e-commerce, users are often overwhelmed with choices. Generic recommendations fail to capture individual preferences, leading to lower engagement and missed revenue opportunities.

This project builds a **personalized product recommendation system** using customer transaction data. It demonstrates how businesses can use data analytics to move from generic suggestions to **user-specific recommendations**, improving conversion rates and customer experience.

---

## 🎯 Objective

The objective of this project is to:

- Analyze customer purchase behavior  
- Build a recommendation system using data-driven techniques  
- Compare generic and personalized recommendation approaches  
- Derive actionable insights for marketing and business strategy  

---

## 📊 Dataset Description

The dataset consists of real-world e-commerce transactions, including:

- Customer identifiers  
- Product identifiers  
- Order-level purchase data  

To improve computational efficiency and reduce sparsity, the analysis was restricted to the **top 100 most frequently purchased products**.

---

## ⚙️ Project Workflow

### 1. Data Preparation

- Extracted relevant tables from a SQLite database  
- Merged datasets to create a **customer-product interaction dataset**  
- Removed duplicates and cleaned the data  

---

### 2. Popularity-Based Recommendation (Baseline)

- Identified the most frequently purchased products  
- Recommended the same products to all users  

**Limitation:**  
- No personalization  
- Does not consider user preferences  

---

### 3. Improved Popularity Model

- Removed products already purchased by users  
- Ensured recommendations remain relevant  

---

### 4. Collaborative Filtering (Core Model)

- Created a **user-item matrix** (users × products)  
- Applied **cosine similarity** to measure similarity between users  
- Identified users with similar purchase behavior  
- Recommended products based on what similar users have purchased  

**Key Idea:**  
> Users with similar behavior are likely to be interested in similar products.

---

## 📈 Key Insights

### 🔹 Sales Concentration
A small number of products account for a large share of total purchases.

**Business Impact:**  
- Focus on promoting high-performing products  
- Use them strategically in marketing campaigns  

---

### 🔹 User Behavior Patterns
Customers show similar purchasing patterns, enabling behavioral segmentation.

**Business Impact:**  
- Supports targeted marketing and personalization strategies  

---

### 🔹 Personalization vs Generic Recommendations
Collaborative filtering provides more relevant recommendations compared to popularity-based methods.

**Business Impact:**  
- Improves conversion rates  
- Enhances user experience  

---

### 🔹 Cross-Selling Opportunities
Users with similar behavior tend to purchase related products.

**Business Impact:**  
- Enables bundling strategies  
- Increases average order value  

---

### 🔹 Model Trade-off
Restricting analysis to top 100 products improves efficiency but limits recommendation diversity.

---

## 💼 Business Applications

This system can be applied in real-world scenarios such as:

- Homepage recommendations (“Recommended for You”)  
- Product pages (“Customers also bought”)  
- Email marketing campaigns (personalized suggestions)  

---

## 🛠️ Tech Stack

- Python  
- Pandas, NumPy  
- Scikit-learn (cosine similarity)  
- Matplotlib  
- SQLite  

---

## 🚀 Conclusion

This project demonstrates how data analytics and machine learning can be used to deliver personalized customer experiences. By leveraging user behavior, businesses can move beyond generic recommendations and implement **targeted, data-driven marketing strategies**.

---

## 🔮 Future Improvements

- Incorporate product metadata (category, price, ratings)  
- Use advanced recommendation techniques (matrix factorization)  
- Include real-time user activity  
- Expand beyond top 100 products  

---

## 📌 Author

Anaya Vaz

