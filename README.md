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
  - Supply restocking expenses (deterministic) - A fixed amount per night that is determined by peroperty size.
  - Utilities (probabilistic) - Sample electricity and gas from RECs data and use 20% to 30% of (gas + electricity).
  - Airbnb insurance (estimate) AirCover + Home insurance estimate from zillow a fixed % of surcharge for STR add-on. 
  - Cleaning 
  - Appliance and property maintenance - (https://www.census.gov/data/data-tools/ahs-table-creator.html)
  - Property taxes (estimate) - Tax rate estimates from Zillow.
    
- Occupancy and Nightly rate
  - Granularity of simulations and seasonal variations is limited to a monthly level.
  - Cleaning fee will be included.
