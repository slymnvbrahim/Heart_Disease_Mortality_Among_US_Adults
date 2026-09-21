# Heart_Disease_Mortality_Among_US_Adults

Question. How much does age-adjusted heart disease mortality vary across US states and counties, and how large are the sex and race gaps compared with the geographic spread?

Data. CDC Heart Disease Mortality Data Among US Adults by State/Territory and County (data.cdc.gov, source: NVSS). Rates are age-adjusted deaths per 100,000 population. Source link / download date: https://catalog.data.gov/dataset/heart-disease-mortality-data-among-us-adults-35-by-state-territory-and-county-2019-2021

Approach. The raw file mixes county and state rows, two different rate definitions, several years, and "Overall" aggregates sitting next to the subgroups they summarise. Averaging across all of that gives meaningless numbers. So every analysis below works on one explicitly defined slice (one geographic level, one year, one rate definition), and the slice function warns if a slice is still mixed.
