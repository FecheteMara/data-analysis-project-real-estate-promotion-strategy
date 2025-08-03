# Real Estate Listing Promotion Strategy

## Overview
This project simulates a real-world data analysis scenario for Nova Holdings, a major real estate agency in the U.S. The task was to develop a data-driven promotional strategy to select 1,000 out of 10,000 property listings to promote on Zillow—America’s largest real estate platform.

The analysis aims to maximize visibility and accelerate sales by identifying the most promising locations and listings based on consumer interest and investment potential.

## Objectives
- Identify Top 10 Sought-After Locations using search volume and lead activity.
- Determine Top 10 Investment Locations using price and buyer engagement.
- Select Top 50 Listings that deserve promotion based on combined metrics.
- Define removal criteria for underperforming or overpriced listings.

## Data Description
The project uses three datasets:
- traffic	- Shows search volume by location, purpose, and bedroom count.
- leads	- Shows user intent to transact, measured via phone calls or messages per listing.
- inventory	- Full list of 10,000 properties with price, purpose, and location info.

## Key Columns
City, Neighborhood, Section - Combined into unified Location

Searches and Leads - Key engagement indicators

Price - Used for affordability/investment scoring

Purpose - Sale vs Rental

## Methodology
#### Data Cleaning:
- Standardized and merged location fields.
- Removed duplicates and invalid entries.

#### Search Analysis:
- Aggregated search volume by location.
- Identified top 10 high-traffic areas.

#### Investment Analysis:
- Focused on properties for sale.
- Created Investment Score = Leads per $100K.
- Ranked locations by highest return potential.

#### Listing Selection:
- Merged all datasets.
- Selected listings with high engagement + low prices.

#### De-Promotion Criteria:
- Removed listings with:
- Zero leads or searches.
- Pricing 50%+ above location average.

### Tools Used
- Python (Pandas, NumPy, Matplotlib, Seaborn)
- Jupyter Notebook for EDA and reporting
- ChatGPT for presentation refinement and ideation

### Key Results
- Top 10 Locations revealed concentrated buyer demand in major metros like New York.
- Top 10 Investment Zones identified affordable but active locations with high buyer intent.
- 50 Listings Selected based on visibility, affordability, and buyer interest.
- Removal Logic introduced to keep promotions agile and relevant.

### How to Use This Notebook
1.Clone this repository.

2.Install requirements: pip install pandas matplotlib seaborn

3.Run the notebook: Real_Estate_Promotion_Strategy.ipynb

4.Review charts and logic in each section.
