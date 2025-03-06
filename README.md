# Credit Card Customer Segmentation

## 📊 Project Overview
This project focuses on clustering credit card customers into distinct segments based on their spending and repayment behaviors. The goal is to help financial institutions better understand their customer base, mitigate credit risk, and personalize their offerings. By leveraging unsupervised machine learning techniques, we identified actionable insights to optimize credit portfolio management.

## 🔥 Problem Statement
Financial institutions face challenges in identifying high-risk customers and offering tailored credit solutions. Our task was to segment credit card holders based on their transaction patterns, helping banks:
- Identify potential defaulters early.
- Offer personalized financial products.
- Balance risk across their customer portfolio.

## 📦 Dataset Description
The dataset contains anonymized information about customers’ credit behavior, including:
- **Balance:** The amount owed by the customer.
- **Credit Limit:** The maximum credit available.
- **Payments:** History of payments made.
- **Purchases:** Customer spending patterns.
- **Cash Advance:** Cash withdrawals using credit cards.

## 🔬 Approach
Our approach involved several critical steps:

1. **Data Exploration and Cleaning:**
   - Handled missing values and outliers.
   - Scaled numerical features using StandardScaler.
2. **Feature Engineering:**
   - Derived new metrics like credit utilization ratio and repayment ratio.
   - Created aggregated features to capture spending behavior.
3. **Dimensionality Reduction:**
   - Used Principal Component Analysis (PCA) to reduce feature space.
   - Compared models using both 2 and 3 principal components.
4. **Clustering Models:**
   - Implemented K-Means clustering.
   - Determined the optimal number of clusters using Elbow Method and Silhouette Score.
5. **Model Evaluation:**
   - Finalized the 2-component model based on multiple metrics:
     - **Silhouette Score:** 0.4769 (2D PCA) vs. 0.4531 (3D PCA)
     - **Calinski-Harabasz Index:** 12116.50 (2D PCA) vs. 8428.98 (3D PCA)
     - **Davies-Bouldin Score:** 0.6818 (2D PCA) vs. 0.7921 (3D PCA)

## 📈 Final Clusters
We identified 5 customer segments:

- **Stable Credit Users:** Low risk, disciplined repayment patterns, optimal credit usage.
- **Emerging Risk Users:** Moderate risk, inconsistent payment compliance but manageable.
- **Prime Borrowers:** Exemplary users with high compliance and low risk.
- **Chronic Defaulters:** High risk, poor compliance, and over-leveraged.
- **Potential Defaulters:** At-risk group with warning signs of default.

## 🚀 Innovative Business Ideas

1. **Targeted Credit Line Adjustments:**
   - Increase credit limits for **Prime Borrowers** and **Stable Credit Users**.
   - Implement conditional increases for **Emerging Risk Users**.
2. **Behavior-Based Rewards Program:**
   - Cashback or loyalty points for consistent repayments.
   - Interest rate discounts for low credit utilization.
3. **Custom Credit Products:**
   - Installment loans for **Emerging Risk Users**.
   - Prepaid credit options for **Chronic Defaulters**.
4. **AI-Driven Alerts & Recommendations:**
   - Real-time notifications for risky behaviors like high utilization.
   - Payment strategies tailored to user profiles.
5. **Predictive Risk Management:**
   - Use clustering data to train models predicting future defaulters.
   - Offer financial counseling to **Potential Defaulters**.
6. **Portfolio Risk Balancing:**
   - Attract more **Stable Credit Users** and **Prime Borrowers** through strategic marketing.

## 🌟 Impact and Future Scope
This project empowers financial institutions to:

- Reduce credit risk by identifying high-risk customers.
- Boost profitability with targeted offers.
- Enhance customer satisfaction through personalized products.

**Future enhancements:**
- Integrate time-series data for dynamic customer segmentation.
- Experiment with advanced clustering techniques like DBSCAN and Hierarchical Clustering.
- Build predictive models using clustering insights to forecast customer behavior.

## 📚 How to Run
1. Clone the repository:
```bash
git clone <repo_url>
```
2. Install dependencies:
```bash
pip install -r requirements.txt
```
3. Run the Jupyter Notebook to train the clustering model:
```bash
jupyter notebook Credit_Card_Clustering.ipynb
```
4. Visualize cluster outputs and insights directly in the notebook.

## 📧 Contact
For any questions or collaborations, feel free to reach out!

---
Let's build smarter financial solutions together! 🚀

