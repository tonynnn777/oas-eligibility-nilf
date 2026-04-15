
Causal Effect of OAS Eligibility on Retirement in Canada
Difference-in-Differences (DiD) analysis estimating the causal effect of Old Age Security (OAS) eligibility on labour force exit, using 2021 Canadian Census data.
Overview
Canada's Old Age Security program provides monthly payments to eligible individuals aged 65+. Eligibility requires Canadian citizenship or at least 10 years of residency, meaning recent immigrants who arrived after age 60 cannot qualify. This creates a natural experiment: two groups of similar age face entirely different retirement incentives based solely on immigration history.
This project exploits that eligibility cliff to estimate how much OAS increases the probability of leaving the labour force at age 65.
Key Findings

OAS eligibility increases the probability of labour force exit by 2.5 percentage points (most robust specification)
The effect is positive and consistent across all four regression specifications
Results hold after controlling for gender, education, marital status, province, and language fluency

Data

Source: 2021 Canadian Census, Statistics Canada (accessed via Abacus Data Network, UBC)
Sample: Individuals aged 60 to 69, excluding non-permanent residents and those who never worked (118,362 observations)
Treatment group: Non-immigrants and immigrants who arrived before age 60 (OAS-eligible at 65)
Control group: Immigrants who arrived at age 60 or older (cannot meet 10-year residency requirement)

Methods

Design: Difference-in-Differences (DiD)
Outcome: Binary indicator for Not in Labour Force (NILF)
Treatment: Interaction of OAS eligibility x age 65+ threshold
Software: R

Four progressive specifications were estimated:
SpecificationControls1None (baseline DiD)2+ Gender, marital status, education3+ Province fixed effects4+ First official language spoken
Identification
The DiD estimate is valid under the conditional common trends assumption: absent OAS, both groups would have followed the same trend in labour force exit at age 65. This is plausible because ineligibility is determined by age at immigration, a decision made well before the sample window, and both groups face the same aging process and macroeconomic conditions.
Limitations

The control group is small (~2% of the sample), limiting statistical power
Cultural differences in retirement behaviour (e.g. family structure) are not fully controlled for
A placebo test at age 60 is proposed but not yet implemented

References
Government of Canada. (2026). Old Age Security. https://www.canada.ca/en/services/benefits/publicpensions/old-age-security.html
Statistics Canada. (2022). 2021 Census of Population. Abacus Data Network. https://abacus.library.ubc.ca
