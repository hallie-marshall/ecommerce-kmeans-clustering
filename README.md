# Cluster Segmentation with K-Means Clustering

## Project Background

This project is designed to assist a US-based e-commerce company in leveraging customer data for segmentation analysis. This project uses a two-year dataset of customer transactions to uncover key insights into customer purchasing behaviors, allowing for more personalized marketing and improved customer engagement.

The dataset includes detailed information on customer purchases, returns, and transaction frequency; providing a rich foundation for segmentation. By utilizing K-Means clustering, this project aims to group customers based on distinct spending patterns and purchase frequencies, identifying actionable segments for targeted engagement.

Identification of *six distinct customer groups* based on purchasing behaviors, including recency, purchase frequency, and transaction value, are detailed below. Recommendations are provided for each segment to foster customer engagement, maximize revenue, and strengthen customer loyalty. These include targeted discounts, upselling opportunities, and exclusive rewards for top customers. 

## Data Structure

The main table used for this project consists of over 143,000 rows of order information, including:

**OrderID:** unique identifier for confirmed customer orders

**ProductID:** unique identifier for products purchased on confirmed customer orders

**Quantity:** number of units ordered of the ProductID 

**UnitPrice:** price of each unit ordered of the ProductID

**InvoiceDate:** date the order is confirmed

**CustomerID:** unique identifier for customers who've placed the confirmed order

**Country:** country code of the customer. 

## Executive Summary

This project provides a comprehensive analysis of the customer base using K-Means clustering, uncovering distinct patterns in purchasing behaviors and engagement levels. By analyzing transaction data, the project reveals valuable insights into customer behavior, loyalty potential, and areas for strategic growth.

The clustering analysis highlights opportunities to tailor marketing efforts, improve customer retention, and maximize revenue. Key findings indicate a wide range of customer engagement behaviors - from frequent, high-value orders to infrequent purchases at lower spend rates - each representing unique opportunities for targeted strategies.

This analysis provides a foundation for the retail organization to:
- **Enhance Customer Loyalty:** Identifying characteristics of loyal customers enables the company to create targeted loyalty programs, strengthening brand power and increasing lifetime value.
- **Increase Engagement with Targeted Incentives:** Insights into customer spending patterns and purchase frequency suggest that personalized incentives can encourage more frequent purchases and higher transaction values.
- **Reduce Churn:** Understanding the traits of at-risk customer segments allows the company to proactively engage clusters with timely promotions and campaigns, mitigating churn risk.
- **Optimize Resource Allocation:** Segmenting the customer base allows for more efficient marketing spend by focusing efforts on the highest value opportunities and tailoring strategies to specific customer needs.

The insights from this project offer a data-driven approach to customer segmentation, enabling the organization to allocate resources more effectively and build stronger customer relationships. This analysis lays the groundwork for future initiatives, as highlighted in the [Recommendations](https://github.com/hallie-marshall/retail-kmeans-clustering/edit/main/README.md#recommendations) section below.

## Insights

The analysis identified *six key customer segments*, each with unique characteristics and engagement needs. These insights form the basis for specific recommendations aimed at driving engagement, increasing customer loyalty, and maximizing revenue.


![Cluster Visualization](KMeans%20Clustering%20Segments.png)


1. **RETAIN (28.9%):** These customers have made relatively recent purchases, with a moderate frequency of purchase, and they have a high annual spend. They're consistent spenders with a potential for long-term loyalty.

   **Recommendation:** Encourage continued engagement by offering loyalty rewards.
 
2. **ENCOURAGE (24.3%):** Customers in this segment have made recent purchases but at a low frequency and with a low annual spend. They may still be exploring the brand or need a nudge to purchase more regularly.

    **Recommendation:** Incentivize their next purchase by offering a discount for a limited time period.
   
3. **EXCITE (22.9%):** These customers haven't purchased recently, shop infrequently, and have a moderate annual spend. They may need a renewed reason to engage with the brand.

    **Recommendation:** Use urgency-based incentives, like flash sales, to prompt re-engagement.

4. **UPSELL (16.7%):** These customers have made recent purchases at a moderate frequency and demonstrate high annual spending. They're engaged but could be encouraged to spend more per transaction.

    **Recommendation:** Suggest complementary or premium products to increase their order value. Offer add-ons or subscriptions to enhance their purchase value and frequency.
   
5. **RE-ENGAGE (5.8%):** This segment consists of customers who made purchases a long time in the past, with low frequency and low annual spend. They may be at risk of churn and need a reason to return.

    **Recommendation:** Communicate during key events when they may be more likely to re-engage through an additional purchase.
   
6. **REWARD (1.3%):** These customers are the most engaged, with very recent and frequent purchases and the highest annual spend. They represent the brand's most valuable and loyal customers.
  
   **Recommendation:** Encourage referrals, even offering referral bonuses or rewards. Elevate their brand experience with exclusive access or events.

These insights support a range of targeted strategies, each designed to address the unique needs of different customer segments. The recommendations based on these insights aim to improve customer experience, reduce churn, and drive long-term profitability through targeted marketing and engagement efforts.

## Recommendations

There are several opportunities to further utilize these insights, optimize strategies and enhance operational capabilities. A few of these may include:

- **Implement Real-Time Segmentation:** Integrate real-time segmentation to dynamically adjust marketing and communications for each customer cluster. By tailoring messages based on the latest customer behaviors, the company can improve the relevance and timeliness of its interactions, leading to stronger engagement and conversion rates.
  
- **Build a Churn Prediction Model:** Develop a churn prediction model, particularly focused on "RE-ENGAGE" and "EXCITE" clusters. By identifying at-risk customers early, the company can proactively implement retention strategies, such as special offers of personalized outreach, to reduce churn and maintain revenue stability.
  
- **Estimate Customer Lifetime Value (CLV) by Segment:** Calculating CLV for each customer cluster can help the retailer efficiently allocate resources to high-value customers while nurturing other segments. Understanding the long-term value of each segment allows for more strategic planning around customer acquisitions, loyalty investments, and retention strategies.
  
- **Leverage A/B Testing and Multivariate Testing:** Use A/B testing or multi-variate testing to assess the performance of various marketing strategies across different segments. By gathering data on what resonates most with each cluster, the company can continuously refine its approach; optimizing content, offers, and communication channels to drive higher engagement and conversion rates.

These recommendations provide next steps on a pathway to further harness the power of the provided customer segmentation insights, enabling the organization to improve operational efficiency, boost customer satisfaction, and drive sustainable growth.

## Assumptions and Caveats

- Data was only used for US-based customers. Including foreign customer data may lead to differing results.
- The dataset consists of two years of orders, with Invoice Dates ranging from 10/29/2022 to 10/28/2024.
- Following data cleansing, 5% of the data was removed from the dataset.
