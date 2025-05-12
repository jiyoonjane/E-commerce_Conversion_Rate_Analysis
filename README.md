# E-commerce_Conversion_Rate_Analysis
# Introduction

## Project Overview
I’m on the Partner Analytics team at a leading cosmetics e-commerce platform, where I help partner brands grow through data-driven insights. Recently, Grattol—the second highest-earning brand on our site—asked me to analyze their performance and recommend ways to boost their sales.

Although Grattol already ranks #2 in revenue, its purchase conversion rate lags behind competitors. It remains unclear whether low conversion is the primary driver of unrealized revenue. This project seeks to diagnose the root causes of under-optimized sales for Grattol and to recommend actionable, data-backed improvements.

---

## Background: Grattol’s Situation & Problem Statement
  
> **Goal:** Analyze the full revenue funnel—including conversion rate issues—and deliver practical growth strategies for Grattol.

### EDA Workflow & Problem Definition

#### 👀 Step 1: Understand Platform Revenue

![image](https://github.com/user-attachments/assets/41e654a0-92c2-4dfb-b2b8-13d20cd31a0c)

> The platform hosts over 1,000 brands. Since the top four brands together account for more than 30% of total revenue, our comparisons focus on those leading brands.

#### 👀🧭 Step 2: Questioning the Phenomenon  
- **Observation:** Grattol ranks #2 in total sales but shows a disproportionately low conversion rate.  
- **Why It Matters:** High traffic and brand interest fail to translate into purchases, revealing clear opportunities for optimization.

![제목 없음](https://github.com/user-attachments/assets/2acc38c0-4402-49aa-8b72-90ffa058c77a)


### Problem Definition
- **Discrepancy:** High page views vs. low purchase conversion.  
- **Paradox:** Strong revenue performance (#2 overall) but a conversion gap compared to peers.  
- **Improvement Opportunity:** Excessive drop-off in the funnel indicates actionable areas to raise conversions.

---

## Analysis Focus
1. **Funnel Diagnostics**  
   - Measure conversion rate, average order value, and buyer count vs. visitor count to pinpoint revenue drag.  
2. **Event-Log Behavior Mapping**  
   - Reconstruct the customer journey through clickstream data to identify where and why drop-offs occur.

> **Key Finding:**  
> Grattol’s conversion rate is up to **6.7 percentage points** lower than competitors despite high sales volume.

![image](https://github.com/user-attachments/assets/6afb912f-44af-4019-85b4-05a3b225abd7)

- vs. Runail (−6.7 pp)  
- vs. Irisk (−6.4 pp)  
- vs. Uno (−3.5 pp)  
- vs. Top 4 average (−4.0 pp)

- ## Monthly Revenue Trend
- Grattol remains the #2 monthly revenue brand, but as of **February 2020**, the gap between top competitors is narrowing.
- Although Grattol experienced a sharp month-over-month revenue decline (mirroring other brands), **Irisk** actually **grew** its revenue during the same period—hinting at a possible overtake in the near future.

![image.png](attachment:c644fee0-6810-4296-9ad7-74e6dd3e2edc:image.png)

## Daily Revenue Trend
- Aside from event-driven sales spikes, all brands except Runail trail behind Irisk on a day-to-day basis.

![image.png](attachment:28945e5d-b0e8-4a3f-8156-5b25251d06fe:image.png)

> **Note: How Is Revenue Calculated?**  
> Revenue = Number of Purchasers × ARPPU  
> = Visitors × Conversion Rate × ARPPU (Average Revenue Per Paying User)

- **Visitors**: Total unique users landing on the brand page  
- **Conversion Rate**: Percentage of visitors who make a purchase  
- **ARPPU**: Average revenue per paying user

## 👀🧭 Step 3: Analyze Grattol’s February 2020 Decline

![image.png](attachment:788608c3-1590-400e-93b4-ef9f2a246c0f:image.png)

| Brand   | Visitors ↓ | Conversion Rate ↓ | ARPPU ↑ | Revenue ↓  |
|---------|------------|-------------------|---------|------------|
| Runail  | Yes        | Yes               | Yes     | Significant ↓ |
| Grattol | Yes        | **Yes**           | Yes     | ↓          |
| Irisk   | Yes        | ↑                 | ↑       | ↑          |
| Uno     | Yes        | Yes               | ↑       | ↓          |

1. **Why did Grattol’s revenue drop?**  
   - **Visitors ↓**: Platform-wide slowdown (common trend)  
   - **Conversion Rate ↓**: Fewer visitors converted—👈 **the core issue**  
   - **ARPPU ↑**: Those who did buy spent more on average  

   _Although traffic fell, Grattol lost a disproportionate share of buyers, driving its revenue decline._

2. **Why did Irisk grow?**  
   Despite traffic decline, Irisk **improved** its conversion rate, resulting in overall revenue growth.

3. **Next Steps**  
   Close Grattol’s **opportunity cost gap**:  
   - Grattol’s conversion rate lags the top-4 average by ~4 pp, indicating significant lost revenue potential on high traffic.  
   - **Immediate focus**: Boost conversion rate to defend and grow monthly revenue.

## Project Objective
- Diagnose the **root causes** of Grattol’s under-optimized sales by examining conversion rate, ARPPU, and buyer counts.  
- Deliver **data-driven insights** and tactical recommendations by analyzing user behavior across funnel stages, time of day, price tiers, and weekdays to pinpoint key growth levers.

