# RentalPropertyOptimization
An optimization + ML approach to finding the best rental property investment.

Assumptions
- Capital Expense assumptions
  - Down payment- 25% down payment
  - Refurnishing costs- Fixed expenses based on property size.
    
- Operating expense assumptions
  - Mortgage (deterministic)- A mortgage calculator using current interest rate (6-7%)
  - Airbnb property manager charges (probabilistic)- A full-service fee % (excluding listing creation and optimization services) 
  - Airbnb host fees (deterministic)- AirBnb charges a flat service fee of 3% on the booking subtotal
  - Supply restocking expenses (deterministic)- A fixed amount per night that is determined by peroperty size
  - Utilities- TBD
  - Airbnb insurance- AirCover + a home insurance with an STR rider
  - Preventive maintenance- TBD
  - Property taxes- Tax rate for 2025
    
- Occupancy and Nightly rate
  - Granularity of simulations and seasonal variations is limited to a monthly level.
  - Cleaning fee will be included.
