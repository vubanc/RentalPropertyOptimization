# RentalPropertyOptimization
An optimization + ML approach to finding the best rental property investment.

Assumptions
- Capital Expense assumptions
  - Down payment (deterministic) - 20% down payment.
  - Closing Costs (estimate) - Estimate from Zillow.
  - Refurnishing costs (estimate) - Fixed expense based on property size.
    
- Operating expense assumptions
  - Mortgage (estimate) - Calculated based on Zillow property price (assuming 6% interest rate and 30-year loan).
  - HOA fees- (estimate) - Estimate from Zillow.
  - Airbnb property manager charges (deterministic) - A % fee (excluding listing creation and optimization services).
  - Airbnb host fees (deterministic) - a flat service fee of 3%.
  - Restocking and cleaning expenses (deterministic) - Cancelled out by cleaning fee.
  - Utility bill/sqft (probabilistic) - Electricity and gas sampled from RECs data. 20% to 30% of (gas + electricity) is considered as the water bill.
  - Airbnb insurance (estimate) - AirCover + home insurance estimate from zillow (plus a fixed % surcharge for STR add-on). 
  - Appliance and property maintenance (estimate) - 1-3% rule stated here: https://www.thebalancemoney.com/home-maintenance-budget-453820
  - Property taxes (estimate) - Tax rate estimate from Zillow.
    
- Occupancy and Nightly rate
  - Granularity of simulations and seasonal variations is limited to a monthly level.
  - Cleaning fee will be included.
