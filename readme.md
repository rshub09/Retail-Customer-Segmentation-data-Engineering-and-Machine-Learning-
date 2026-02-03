# Customer Segmentation using Predictive Analytics

## 📌 Project Overview
This project applies **predictive analytics and machine learning** techniques to segment retail customers based on their **transactional behaviour and campaign engagement**.  
The objective is to identify meaningful customer groups and translate analytical insights into **actionable marketing strategies** that improve customer engagement, loyalty, and revenue.

The analysis combines:
- **Unsupervised learning (K-Means clustering)** for value-based segmentation  
- **Supervised learning (Classification Tree)** for product-level and coupon engagement insights  

📄 *Full academic report available in this repository* :contentReference[oaicite:0]{index=0}

---

## ❓ Problem Statement
Retailers collect large volumes of customer transaction and campaign data, but often face challenges in:
- Understanding heterogeneous customer behaviour
- Identifying which customers respond to promotions
- Designing targeted campaigns instead of generic marketing

The core problem is to **extract patterns from transactional and campaign data** and segment customers in a way that supports **data-driven decision-making**.

---

## 📊 Data & Feature Engineering
Customer-level features were engineered from transactional and campaign datasets:

- **Purchase Frequency** – number of baskets per household  
- **Total Spending** – actual spend after discounts  
- **Campaign Response Rate** – ratio of redeemed campaigns to campaigns received  

For deeper behavioural insights, product-category spending features were created (e.g. grocery, health & wellness, automotive) and linked with coupon redemption behaviour.

---

## 🧠 Methodology

### 1️⃣ K-Means Clustering (Unsupervised)
- Features were **standardised** to avoid scale bias
- Optimal number of clusters identified using:
  - Elbow Method
  - Silhouette Score
- **Three clusters** selected for best cohesion and separation

Used to segment customers by **value and marketing susceptibility**.

---

### 2️⃣ Classification Tree (Supervised)
- Target variable: **Coupon Redemption Frequency**
  - Q0: No coupons redeemed  
  - Q1: 1–3 coupons  
  - Q2: 4–35 coupons  
- Entropy used as split criterion
- Tree depth limited to reduce overfitting
- Balanced class weights applied

Used to understand **which product categories drive promotion engagement**.

---

## 📈 Key Results

### 🔹 K-Means Customer Segments
1. **Low-Value, Low-Susceptibility Customers**  
   - Lowest spend and purchase frequency  
   - Minimal response to campaigns  
   - Low engagement and brand loyalty  

2. **Moderate-Value, High-Susceptibility Customers**  
   - Moderate spending  
   - Highest campaign response rate (~56%)  
   - Strong potential for targeted marketing  

3. **High-Value, Moderate-to-Low Susceptibility Customers**  
   - Highest spending and purchase frequency  
   - Less dependent on promotions  
   - Core revenue-driving customers  

---

### 🔹 Classification Tree Insights
- Grocery spending is the strongest predictor of coupon usage  
- Q0 customers show low category engagement  
- Q1 customers redeem coupons opportunistically  
- Q2 customers are high spenders with strong promotion engagement across categories  

---

## 💡 Business Recommendations
- **Low-Value Customers**: Introductory offers and simple discounts  
- **Moderate-Value Customers**: Loyalty programs, points-based rewards, cross-category bundles  
- **High-Value Customers**: VIP programs, exclusive offers, early product access  
- Simplify coupon redemption to reduce friction  
- Replace generic campaigns with **segment-specific promotions**

---

## ✅ Conclusion
By combining **K-Means clustering** with **Classification Trees**, this project delivers a structured and interpretable approach to customer segmentation.  
The results enable retailers to:
- Identify high-impact customer groups  
- Personalise marketing strategies  
- Improve customer retention and revenue growth  

This framework provides a strong foundation for **data-driven retail analytics** and personalised marketing strategies.

---

## 🛠️ Tools & Techniques
- Python  
- Pandas & NumPy  
- Scikit-learn  
- K-Means Clustering  
- Classification Trees  
- Data Standardisation & Feature Engineering  

---

## 📁 Repository Structure
- `Customer Segmentation.pdf` – Full academic report  
- `README.md` – Project summary and insights  

---

