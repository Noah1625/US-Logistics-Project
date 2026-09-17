# U.S. Logistics Performance Analysis

## Overview

A logistics analytics project analyzing 2,000 U.S. shipments to evaluate
shipment volume, carrier performance, warehouse performance, delivery
status, transit time, and shipping costs.

Built as a portfolio project to demonstrate Power BI and business analysis skills.


## Business Questions

- How does shipment volume change over time?
- Which carriers have the shortest average transit times?
- How does delivery performance vary by warehouse?
- What percentage of shipments are delivered, delayed, lost, in transit, or returned?
- How does shipping cost relate to distance and shipment weight?
- Where are potential operational outliers?

## Data

The dataset contains 2,000 shipment records with information including:

- Shipment ID
- Origin warehouse
- Destination
- Carrier
- Shipment date
- Delivery date
- Weight
- Distance
- Cost
- Transit time
- Shipment status

## Data Preparation

Before building the dashboard, I performed:

- Data profiling
- Missing-value analysis
- Duplicate checks
- Outlier analysis using IQR
- Data type validation
- Dimension/fact table modeling

## Data Model

[Insert data model screenshot here]

The Power BI model uses a fact/dimension structure:

Fact_Shipments
- Shipment_ID
- Shipment_Date
- Delivery_Date
- Carrier_Key
- Warehouse_Key
- Destination_Key
- Status_Key
- Cost
- Distance
- Weight
- Transit_Days

Dimension tables:
- dim_date
- dim_carrier
- dim_warehouse
- dim_destination
- dim_status

## Dashboard

[Insert dashboard screenshot here]

The dashboard provides:

- Monthly shipment volume
- Shipment status breakdown
- Carrier performance
- Warehouse performance
- Cost vs. distance analysis
- Transit-time distribution

## Key Findings

- For Carriers, LaserShip has the quickest shipping, while Amazon Logistics has the slowest
- The New York City Warehouse has the highest delivery rate, while the Miami Warehouse has the lowest.
- Total shipments take a big dip in the winter but are at their peak around August/September
  
