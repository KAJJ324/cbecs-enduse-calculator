cbecs-enduse-eui
Fuel-specific end use EUI by building type for any U.S. census division using 2018 CBECS microdata

What it does

Reads the EIA's 2018 CBECS public use microdata file, filters to a user-selected census division, and produces a wide summary table showing median electricity and natural gas Energy Use Intensity broken down by end use for all 20 commercial building types. Building types are ranked from most to least energy intensive by total EUI.

Input

2018 CBECS public use microdata file (cbecs2018_final_public.csv), available from the EIA website: https://www.eia.gov/consumption/commercial/data/2018/
The user is prompted at runtime to enter a census division code (1–9).

Census division codes

1 — New England | 2 — Middle Atlantic | 3 — East North Central | 4 — West North Central | 5 — South Atlantic | 6 — East South Central | 7 — West South Central | 8 — Mountain | 9 — Pacific

Output

A ranked table showing median EUI (kBtu/sq ft) per building type with columns for total EUI and fuel-specific end uses: electric lighting, cooling, heating, ventilation, and refrigeration; natural gas heating, water heating, and cooking.

Concepts demonstrated

Nested dictionaries, user-defined functions, safe value extraction with fallback, multi-column tuple storage and unpacking, in-place sorting with lambda, generator expression in sum(), f-string wide table formatting, input validation with exit()

Data source

U.S. Energy Information Administration — 2018 Commercial Buildings Energy Consumption Survey
https://www.eia.gov/consumption/commercial/data/2018/
