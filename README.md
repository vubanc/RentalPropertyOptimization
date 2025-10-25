# RentalPropertyOptimization
Finding the best market for short term rental investment using bayesian hierarchical modeling.

Data Sources/Assumptions
- Capital Expense Components
  - [x] Down payment (deterministic) - 20% down payment.
  - Closing Costs (estimate) - Estimate from Zillow.
  - Refurnishing/Home Improvement costs (estimate) - TBD (most likely using RECS data)
    
- Operating Expense Components
  - [x] Mortgage (estimate) - Calculated based on Zillow property price (assuming 6% interest rate and 30-year loan).
  - [x] HOA fees- (estimate) - Estimate from Zillow.
  - [x] Airbnb property manager charges (deterministic) - Assuming actively managed property
  - Airbnb host fees (deterministic) - a flat service fee of 3%.
  - Restocking and cleaning expenses (deterministic) - Cancelled out by cleaning fee.
  - Utility bill/sqft (probabilistic) - Electricity and gas sampled from RECs data. 20% to 30% of (gas + electricity) is considered as the water bill.
  - STR insurance (estimate) - Home insurance estimate from zillow (plus a fixed % surcharge for STR add-on). 
  - [x] Appliance and property maintenance (estimate) - 1-3% rule stated here: https://www.thebalancemoney.com/home-maintenance-budget-453820
  - [x] Property taxes (estimate) - Tax rate estimate from Zillow.
    
- Revenue Components
  - Occupancy (probabilistic)- Modeled as a function of market and season
  - Nightly Rate (probabilistic)- Modeled as a function of market, season, bedroom count, distance to POIs, and amenities.
