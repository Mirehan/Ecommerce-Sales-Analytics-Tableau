# E-commerce Sales Analytics Dashboard

A multi-page Tableau dashboard analyzing e-commerce performance across four 
areas: sales trends, delivery/logistics performance, market/category 
performance, and customer feedback. Built for an Indonesian marketplace 
dataset spanning 2016–2018.

🔗 **Live interactive dashboard:** [Tableau Public link]

## Tools Used
- Tableau (dashboard design, calculated fields, parameter-driven insights)
- Excel / CSV / SQL for source data

## Dataset
62,188 orders (Mar 2016 – Dec 2018) covering revenue, order status, delivery 
timelines, seller performance, payment type, product category, customer 
state, and post-delivery feedback scores.

## Key Insights

**Sales Overview**
- Revenue reached 8,595,153,030 across 62,188 orders (avg order value 138,212), 
  with a 64.20% on-time delivery rate and a 4.09/5 avg feedback score.
- Monthly revenue grew from ~120M in Jan 2017 to a peak of ~1.01B in Nov 2017, 
  then stabilized around 850M–1B through Aug 2018 — worth cross-referencing 
  against marketing/promo calendars to confirm whether the Nov 2017 peak was 
  a one-off campaign effect.
- **Customer retention is critically low:** only 3.17% of customers ever place 
  a second order — the single biggest risk to sustainable growth, since 
  acquisition currently can't be relied on to convert into repeat revenue.
- Credit card is the dominant payment method (77.13%), far ahead of blipay 
  (19.76%), voucher (3.89%), and debit card (1.50%).
- 98.09% of orders reach "delivered" status, with cancellations minimal (0.46%).

**Delivery Status**
- On-time rate sits at 64.20%, with an average delay of 105 days on late 
  orders and 13.16 days average processing time across 2,794 tracked sellers.
- **Seller performance is highly uneven:** some sellers show on-time rates as 
  low as 0.04–0.06%, including one handling 92 orders and 60.1M in revenue — 
  these high-volume, low-reliability sellers are the clearest operational 
  priority.
- **Late delivery measurably hurts satisfaction:** on-time deliveries average 
  4.136/5 feedback vs. 3.996/5 for late ones — a direct, quantifiable link 
  between logistics performance and customer sentiment.
- Top 5 states by order volume (Banten, DKI Jakarta, Jawa Barat, Jawa Tengah, 
  Jawa Timur) all cluster tightly around a 20% on-time rate, suggesting the 
  delay problem is systemic rather than region-specific.

**Market Overview**
- Health & Beauty and Watches & Gifts lead category revenue (both approaching 
  800M), well ahead of the remaining categories — a concentration worth 
  protecting while investing in growth for lower-performing categories.
- **Revenue is geographically concentrated:** Banten alone generates ~3B, 
  nearly double DKI Jakarta and Jawa Barat (~1.8B each) — a small number of 
  states are carrying most of the business.
- Order values cluster heavily in the 100K–200K range, with a sharp drop-off 
  above 500K, indicating the customer base skews toward mid-value purchases 
  rather than high-ticket items.
- Category revenue trends show most top-5 categories rising and falling in 
  tandem through 2017–2018, rather than one category consistently outpacing 
  the others.

**Customer Feedback**
- Avg feedback score is 4.09/5, but with a notable split: 14.63% of all 
  reviews are 1–2 stars, and on-time vs. late feedback averages diverge 
  (4.22 vs. 3.86).
- Feedback is heavily skewed positive at the top: 5-star reviews vastly 
  outnumber every other rating, while 2-star reviews are the least common — 
  a bimodal pattern (mostly very happy, a meaningful minority very unhappy) 
  rather than a normal distribution.
- Books, CDs/DVDs, and food/drink categories score highest on average feedback, 
  while audio, construction tools, and diapers/hygiene score lowest — a 
  useful list for prioritizing quality or fulfillment review.

## Dashboard Pages
1. **Sales Overview** — revenue, orders, order status mix, payment type mix, 
   weekday order patterns, and new vs. returning customers
2. **Delivery Status** — on-time rate by state, feedback vs. delivery timing, 
   and lowest-performing sellers
3. **Market Overview** — top categories and states by revenue, order value 
   distribution, and category/payment trends over time
4. **Customer Feedback** — feedback score breakdown, highest/lowest-rated 
   categories, and response time metrics

## How to Use
1. View the live dashboard via the Tableau Public link above, or
2. Download the `.twbx` file from this repo and open in Tableau Desktop/Public
3. Use the filter icon (top right of each page) to slice by state, category, 
   or payment method
