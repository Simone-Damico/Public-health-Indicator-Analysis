# Public Health Indicator Analysis
In this project the indicator *Breast tumor removal surgery 
within 60 days from the date of diagnosis* is defined. The 
indicator for each hospital structure present in the data 
is analyzed and the association at individual level between 
the level of education and the work and the value of the indicator is 
also assessed. [Here](https://simone-damico.github.io/Public-health-Indicator-Analysis/) the complete R code.

### Dataset description
Three simulated datasets are available, two extracts from population 
registers and one from an administrative health flow:

- extract from a health registry for the year 1984 
relating to a small town. The variables that compose it are t
he following:
    - **idnum**: identification code of the subject
    - **smoke** (yes or no): if the subject currently smokes
    - **sex** (Female or Male)
    - **married** (yes or no): if it is currently married
    - **kids** (yes or no): if the subject has children
    - **work** (yes or no): if it currently works
    - **education** (no / low <= middle school diploma; medium / high> = middle school diploma
    higher
    - **age** (numerical in years)

- Cancer Registry for the month of January 1984. The variables
 that make it up are the following:
    - **idnum**: identification code of the subject
    - **stage** (I, II, III, IV): stage of the tumor at diagnosis
    - **incidence**: date of diagnosis of the tumor
    - **type of tumor**: breast, lung, colon, other

- Hospital discharge sheets of subjects hospitalized between 
January 1984 and October 1984 for oncological treatments:
    - **idnum**: identification code of the subject
    - **performance**: type of treatment received during hospitalization (surgical, chemotherapy or radiotherapy)
    - **date of performance**: date of treatment
    - **discharge**: date of discharge from the hospital
    - **hospital**: unique code of the hospital
    
### Analysis
In the first phase, the data sets are cleaned up removing 
the inconsistencies, then the record linkage of the data 
sets is performed. The indicator is calculated globally and 
by individual healthcare facility.\
The odds ratio is calculated for both the education variable 
and the job variable, using the Mantel Haenszel method.
Estimate and interpret this effect measure, adjusted for all 
the available variables that you consider appropriate to 
include as potential confounders, using a logistic regression 
model.
