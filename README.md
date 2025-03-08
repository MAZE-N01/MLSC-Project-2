# 📌 E-commerce Customer Segmentation

##  Project Overview
This project aims to segment e-commerce customers based on their **coupon usage behavior** using **unsupervised machine learning** techniques such as **K-Means** and **DBSCAN**. The goal is to identify customer groups and recommend strategies to improve customer engagement and retention.

##  Dataset Overview
The dataset consists of multiple tables containing:
- **Customer demographics** (gender, city, join date)
- **Coupon transaction history** (claim & burn status, branch usage)
- **Branch & Merchant information**

##  Methodology
### 1️⃣ **Feature Engineering & Preprocessing**
- Extracted **total transactions, burn rate, and days since joining**.
- Encoded categorical variables (gender, city).
- Standardized data for clustering.

### 2️⃣ **Clustering Algorithms Used**
- **K-Means Clustering**: Optimized using **Elbow Method & Silhouette Score**.
- **DBSCAN**: Used for identifying **outliers and unique behaviors**.

### 3️⃣ **Evaluation Metrics**
- **Inertia** (for K-Means cluster compactness).
- **Silhouette Score** (for cluster quality assessment).

##  Customer Segmentation Insights
Based on clustering results, we identified **five key customer segments**:

### ** Segment 1: High-Value Loyal Customers**
- **Frequent coupon users** with high transactions.
- **Low burn rate** (claim but don’t always redeem).
- **Long-term customers**.
- ✅ **Recommendation**: Offer premium loyalty rewards & exclusive coupons.

### ** Segment 2: Inactive Customers**
- **Rarely use coupons**.
- **Never redeem claimed coupons**.
- ✅ **Recommendation**: Reactivation campaigns, reminder emails, & limited-time discounts.

### ** Segment 3: Occasional Users**
- **Moderate transactions & burn rates**.
- **New customers testing out coupons**.
- ✅ **Recommendation**: Targeted discount offers & cashback rewards.

### ** Segment 4: New & Experimental Users**
- **Recently joined, low transaction history**.
- **Potential future loyal customers**.
- ✅ **Recommendation**: Welcome incentives & educational campaigns on savings.

### ** Segment 5: Deal Seekers**
- **High burn rate but low engagement outside discounts**.
- ✅ **Recommendation**: Limited-time flash sales & exclusive deals.

##  Visualizations & Business Recommendations
- **Pie Charts**: Gender & city distributions.
- **Time-series Line Charts**: Coupon transaction trends.
- **Heatmaps**: Branch-wise & city-wise burn rates.
- **Boxplots & Bar Charts**: Customer retention & segment behavior.

##  How to Run the Project
###  **Prerequisites**
Install the required libraries:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

###  **Run the Jupyter Notebook**
```bash
jupyter notebook notebook/customer_segmentation.ipynb
```

##  Repository Structure
```
E-commerce-Customer-Segmentation/
│-- data/                  # (Optional) Dataset folder
│-- notebook/              # Jupyter Notebook for analysis
│   ├── customer_segmentation.ipynb
│-- visuals/               # (Optional) Folder for saved visualizations
│-- README.md              # Project documentation
│-- requirements.txt       # Dependencies list
│-- .gitignore             # Ignore unnecessary files
```

##  Author
**[Your Name]** – Data Scientist

##  License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---
 *Feel free to fork, contribute, or raise issues!* 🚀

