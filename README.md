# Hotel Performance Analysis (2018-2020)
---
# Table of Contents
---
- [Introduction](#introduction)
- [Problem Statement](#problem-statement)
- [Data Sourcing](#data-sourcing)
- [Data Transformation & Cleaning](#data-transformation-&-cleaning)
- [Data Modeling](#data-modeling)
- [Data Analysis](#data-analysis)
- [Data Visualization](#data-visualization)
- [Conclusion](#conclusion)
- [Recommendation](#recommendation)


---
## Introduction
---
This project analyzes hotel booking data from 2018 to 2020 to gain insights into booking patterns, revenue performance, guest distribution, and cancellations.
The goal is to provide hotel management with a clear, data-driven understanding of demand trends, key markets, and revenue risks in order to support better strategic and operational decisions.

The analysis is presented through an interactive Power BI dashboard that summarizes performance using KPIs, trends, and comparative visuals.


---
## Problem Statement
---
Hotel management needs to answer several critical business questions:

    How have bookings changed over time?

    Which markets and customer segments drive the most revenue?

    How significant are booking cancellations?

    Which countries contribute the highest booking volume?

    Is pricing aligned with demand patterns?

Without clear insights into these areas, decisions around pricing, marketing focus, and capacity planning risk being inefficient or reactive.


---
## Data Sourcing
---
The dataset used for this analysis is a hotel booking dataset, containing historical records of hotel reservations.
Key data fields include:

    Booking details (arrival dates, stay duration, cancellations)

    Customer attributes (market segment, country)

    Revenue indicators (ADR, total revenue drivers)

    Guest information (number of guests per booking)

The data spans three years (2018–2020), allowing for trend and seasonality analysis.



---
## Data Transformation & Cleaning
---
To ensure accuracy and reliability, the following steps were performed:

    Handled missing and blank values in ADR, guest counts, and booking fields

    Created standardized date fields to support monthly trend analysis

    Ensured numerical columns were correctly typed for aggregation

    Removed or filtered invalid booking records where necessary

    Normalized market segment and country labels for consistency

These steps helped prevent inflated metrics and ensured meaningful comparisons across time and categories.



---
## Data Modelling
---
A star schema data model was implemented for efficient analysis:

    Fact Table

        Hotel_Fact (bookings, revenue drivers, guests, cancellations)

    Dimension Tables

        Date_Dim (month, year)

        Market Segment

        Country / Location

Relationships were defined as one-to-many, with proper filter flow from dimensions to the fact table to support slicing by time, market segment, and geography.


---
## Data Analysis
---
Top 5 Countries with the Highest Bookings
🔍 Key Insights

    Portugal dominates booking volume with approximately 62K bookings, far exceeding all other countries.

    The United Kingdom, France, Spain, and Germany contribute significantly fewer bookings in comparison.

    Booking demand is highly concentrated in a single country, increasing exposure to market-specific risks.

    Other countries represent growth opportunities but are currently under-leveraged.


     Monthly Booking Trend
🔍 Key Insights

    Bookings show clear seasonality, with peaks occurring around July and October.

    Lower booking volumes are observed in early and late months of the year, indicating off-peak periods.

    The sharp mid-year increase suggests strong leisure or holiday-driven demand.

    Demand volatility highlights the need for proactive planning.


 Market Segments with the Highest Revenue
🔍 Key Insights

    Online Travel Agencies (OTAs) generate the largest share of revenue (over half of total revenue).

    Direct bookings and offline travel agents contribute moderately to revenue.

    Corporate and group segments generate the smallest revenue share.

    Heavy reliance on OTAs may increase commission costs and margin pressure.


How Much Booking Volume Is Lost to Cancellation?
🔍 Key Insights

    Approximately 37% of bookings are canceled, which represents a significant loss in potential revenue.

    A cancellation rate this high indicates booking uncertainty or customer commitment issues.

    Cancellations can disrupt forecasting, staffing, and inventory planning.

    High cancellation levels may be linked to long waiting times or flexible booking policies.


---
## Data Visualization
---
Top 5 Countries with the Highest Bookings
<img width="258" height="124" alt="Screenshot 2026-02-05 210345" src="https://github.com/user-attachments/assets/cce5625d-367c-4490-a4e3-89e1fe362e47" />


Monthly Booking Trend
<img width="250" height="129" alt="Screenshot 2026-02-05 210312" src="https://github.com/user-attachments/assets/f51aef4b-b234-44e4-839c-1d1a180aef5c" />


 Market Segments with the Highest Revenue
 <img width="129" height="103" alt="Screenshot 2026-02-05 210409" src="https://github.com/user-attachments/assets/2b7fc463-cbea-4fa3-9f1b-cff822076e48" />


  How Much Booking Volume Is Lost to Cancellation?
  <img width="119" height="103" alt="Screenshot 2026-02-05 210432" src="https://github.com/user-attachments/assets/5a03c620-b67e-4021-83e2-05c6d4f3ff1e" />











