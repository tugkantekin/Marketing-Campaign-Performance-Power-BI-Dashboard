# Marketing-Campaign-Performance-Power-BI-Dashboard

## Overview

This project is a Power BI dashboard built to help a marketing team understand which channels and audience segments deliver the best ROI and engagement. The dashboard compares five campaign types (Influencer, Search, Display, Email, Social Media) and five customer segments (Foodies, Outdoor Adventurers, Fashionistas, Tech Enthusiasts, Health & Wellness).

## Approach
Four visualization types were used, each chosen for a specific purpose:

* **Horizontal bar chart — Average ROI by Campaign Type:** A bar chart was used to compare a categorical variable (5 campaign types); horizontal orientation keeps the category labels readable.

* **Vertical bar chart — Average Conversion Rate by Campaign Type:** The same categorical structure is shown vertically for a different metric (conversion rate), making the two charts easy to scan side by side.

* **KPI cards (Total Impressions, Total Clicks, Average Conversion Rate):** Cards were used for top-level metrics that need to be communicated as a single number at a glance, without requiring the viewer to interpret a chart.

* **Donut chart — Average Engagement Score by Customer Segment:** A donut chart was chosen to show each segment's share of the total (as a %), with both the absolute score and the percentage labeled per segment.

* **Slicer — Campaign Type:** An interactive control that lets the user filter the other visuals by a single campaign type.

<img width="320" height="164" alt="Image (1)" src="https://github.com/user-attachments/assets/343e95ad-d3b7-4ee1-9d80-c75b6d4c0512" />

## Findings

I rasterized the dashboard page and measured the bar lengths at the pixel level, since text extraction alone doesn't capture bar heights:

* **ROI:** All five campaign types (Influencer, Search, Display, Email, Social Media) have essentially identical bar lengths — the measured pixel differences are under 1%, i.e. within visual noise. There is no clear ROI leader in this dataset; all five cluster around ~4.7–4.8 (on a 0–6 scale).
* **Conversion rate:** The same pattern holds — all five campaign types' bars are nearly the same height (~0.08). Again, no meaningful difference.
* **Engagement score (by segment):** Foodies has the highest average engagement score at 5.51 (20.06%), followed by Outdoor Adventurers at 5.50 (20.03%), Fashionistas at 5.49 (19.98%), Tech Enthusiasts at 5.49 (19.97%), and Health & Wellness at 5.48 (19.96%). The spread between segments is only 0.03 points (about 0.5%) — practically negligible.
* **Totals:** 1 billion impressions, 110 million clicks, 0.08 average conversion rate.

## Limitations
* There is no time dimension in this dataset, so trend analysis over time is not possible.
* ROI is a single number per campaign type with no cost breakdown (media spend, creative production cost, etc.), so how ROI was calculated cannot be verified.
* Customer segments appear to be pre-assigned rather than behavioral; the dashboard does not explain how segments were determined.

## Tool Used
Power BI Desktop.
