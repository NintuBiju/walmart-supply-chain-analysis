# Dataset Description

## Source
Walmart Supply Chain Dataset (synthetic, for analytical purposes)

## File
`walmart_supply_chain_500k_clean11.xlsx`  
⚠️ File not included in this repository due to size (500,000 rows).

## Size
- **Rows:** 500,000
- **Columns:** 39

## Time Period
January 2016 – January 2026

## Column Reference

| Column | Type | Description |
|---|---|---|
| event_id | string | Unique identifier for each supply chain event |
| event_ts | datetime | Timestamp of the event |
| event_type | string | Type of event (e.g. SHIPPED, DELIVERED, RESTOCKED) |
| lifecycle_stage | string | Stage in the supply chain (e.g. FORWARD_LOGISTICS, SHIPMENT) |
| scenario_name | string | Business scenario driving the event |
| channel_path | string | Route the product takes (e.g. SUPPLIER>DC>STORE>CUSTOMER) |
| supplier_name | string | Name of the supplier |
| sku_id | string | Product SKU identifier |
| product_category | string | Category (Grocery, Electronics, Apparel, etc.) |
| warehouse_region | string | Region of the warehouse (Northeast, Southeast, Central, West) |
| qty | integer | Quantity of units involved in the event |
| unit_cost | float | Cost per unit to Walmart |
| sell_price | float | Retail selling price per unit |
| on_time_flag | float | 1 = on time, 0 = delayed (null if not applicable) |
| delay_days | float | Number of days delayed (0 = no delay) |
| actual_cycle_days | float | Total days to complete the event cycle |
| anomaly_flag | integer | 1 = anomalous event, 0 = normal |
| revenue_leakage_flag | integer | 1 = revenue lost, 0 = no leakage |
| customer_impact_score | integer | Score representing impact on customer (0–88) |
| exception_code | string | Code describing the exception/failure (null if no exception) |
| root_cause_category | string | Category of the root cause (null if no exception) |
| inventory_delta | integer | Change in inventory quantity after the event |

## Key Notes for Analysis
1. Nulls are structural — many columns only apply to specific event types
2. Grocery dominates — 56% of events, so segment before generalising
3. on_time_flag has 13.7% nulls — events where delivery timing is not applicable
4. anomaly_flag = 1 in 37.4% of events — central to root cause analysis