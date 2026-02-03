<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Customer Segmentation using Predictive Analytics</title>
</head>

<body>

<h1>Customer Segmentation using Predictive Analytics</h1>

<h2>Project Overview</h2>
<p>
This project applies predictive analytics and machine learning techniques to segment retail
customers based on their transactional behaviour and campaign engagement.
The objective is to identify meaningful customer groups and translate analytical insights into
actionable marketing strategies that improve customer engagement, loyalty, and revenue.
</p>

<p>The analysis combines:</p>
<ul>
    <li>Unsupervised learning using K-Means clustering for value-based segmentation</li>
    <li>Supervised learning using a Classification Tree for product-level and coupon engagement insights</li>
</ul>

<p>
A full academic report is available in this repository.
</p>

<hr>

<h2>Problem Statement</h2>
<p>
Retailers collect large volumes of customer transaction and campaign data, but often face challenges in:
</p>
<ul>
    <li>Understanding heterogeneous customer behaviour</li>
    <li>Identifying which customers respond to promotions</li>
    <li>Designing targeted campaigns instead of generic marketing</li>
</ul>

<p>
The core problem is to extract patterns from transactional and campaign data and segment customers
in a way that supports data-driven decision-making.
</p>

<hr>

<h2>Data and Feature Engineering</h2>
<p>
Customer-level features were engineered from transactional and campaign datasets:
</p>

<ul>
    <li>Purchase Frequency – number of baskets per household</li>
    <li>Total Spending – actual spend after discounts</li>
    <li>Campaign Response Rate – ratio of redeemed campaigns to campaigns received</li>
</ul>

<p>
For deeper behavioural insights, product-category spending features were created
(for example grocery, health and wellness, and automotive) and linked with coupon
redemption behaviour.
</p>

<hr>

<h2>Methodology</h2>

<h3>K-Means Clustering (Unsupervised)</h3>
<ul>
    <li>Features were standardised to avoid scale bias</li>
    <li>The optimal number of clusters was identified using the Elbow Method and Silhouette Score</li>
    <li>Three clusters were selected for best cohesion and separation</li>
</ul>

<p>
This approach was used to segment customers by value and marketing susceptibility.
</p>

<h3>Classification Tree (Supervised)</h3>
<p>
Target variable: Coupon Redemption Frequency
</p>

<ul>
    <li>Q0: No coupons redeemed</li>
    <li>Q1: 1 to 3 coupons redeemed</li>
    <li>Q2: 4 to 35 coupons redeemed</li>
</ul>

<ul>
    <li>Entropy used as the split criterion</li>
    <li>Tree depth limited to reduce overfitting</li>
    <li>Balanced class weights applied</li>
</ul>

<p>
This model was used to understand which product categories drive promotion engagement.
</p>

<hr>

<h2>Key Results</h2>

<h3>K-Means Customer Segments</h3>

<p><strong>Low-Value, Low-Susceptibility Customers</strong></p>
<ul>
    <li>Lowest spend and purchase frequency</li>
    <li>Minimal response to campaigns</li>
    <li>Low engagement and brand loyalty</li>
</ul>

<p><strong>Moderate-Value, High-Susceptibility Customers</strong></p>
<ul>
    <li>Moderate spending</li>
    <li>Highest campaign response rate (approximately 56 percent)</li>
    <li>Strong potential for targeted marketing</li>
</ul>

<p><strong>High-Value, Moderate-to-Low Susceptibility Customers</strong></p>
<ul>
    <li>Highest spending and purchase frequency</li>
    <li>Less dependent on promotions</li>
    <li>Core revenue-driving customers</li>
</ul>

<h3>Classification Tree Insights</h3>
<ul>
    <li>Grocery spending is the strongest predictor of coupon usage</li>
    <li>Q0 customers show low category engagement</li>
    <li>Q1 customers redeem coupons opportunistically</li>
    <li>Q2 customers are high spenders with strong promotion engagement across categories</li>
</ul>

<hr>

<h2>Business Recommendations</h2>
<ul>
    <li>Low-Value Customers: Introductory offers and simple discounts</li>
    <li>Moderate-Value Customers: Loyalty programmes, points-based rewards, and cross-category bundles</li>
    <li>High-Value Customers: VIP programmes, exclusive offers, and early product access</li>
    <li>Simplify coupon redemption to reduce friction</li>
    <li>Replace generic campaigns with segment-specific promotions</li>
</ul>

<hr>

<h2>Conclusion</h2>
<p>
By combining K-Means clustering with Classification Trees, this project delivers a structured
and interpretable approach to customer segmentation.
The results enable retailers to identify high-impact customer groups, personalise marketing
strategies, and improve customer retention and revenue growth.
</p>

<p>
This framework provides a strong foundation for data-driven retail analytics and
personalised marketing strategies.
</p>

<hr>

<h2>Tools and Techniques</h2>
<ul>
    <li>Python</li>
    <li>Pandas and NumPy</li>
    <li>Scikit-learn</li>
    <li>K-Means Clustering</li>
    <l
