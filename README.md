# RentalPropertyOptimization
An optimization + ML approach to finding the best rental property investment.

Assumptions
- Capital Expense assumptions
  - Down payment- 25% down payment
  - Refurnishing costs- Fixed expenses based on property size.
    
- Operating expense assumptions
  - Mortgage (estimate) - Use mortgage payment estimates from Zillow.
  - Airbnb property manager charges (probabilistic) - A full-service fee % (excluding listing creation and optimization services).
  - Airbnb host fees (deterministic) - AirBnb charges a flat service fee of 3% on the booking subtotal.
  - Restocking and cleaning expenses (deterministic) - Cleaning fees will cover these expenses.
  - Utilities (probabilistic) - Sample electricity and gas from RECs data and use 20% to 30% of (gas + electricity) as the water bill.
  - Airbnb insurance (estimate) AirCover + Home insurance estimate from zillow a fixed % of surcharge for STR add-on. 
  - Appliance and property maintenance - 1-3% rule stated here: https://www.thebalancemoney.com/home-maintenance-budget-453820
  - Property taxes (estimate) - Tax rate estimates from Zillow.
    
- Occupancy and Nightly rate
  - Granularity of simulations and seasonal variations is limited to a monthly level.
  - Cleaning fee will be included.
