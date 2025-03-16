- When you need to adjust for multiple variables (confounders) in associations between IV (exposure) and DV (outcome)

#### Outcome types
- Quantitative outcome: continuous/discrete
- Qualitative outcomes: 
	- Nominal
		- dead/alive, disease status
	- Ordinal (ranking, has true order)
		- Breast cancer grade, income, Likert 

#### Types of regression : data
**Linear** : continuous (binary)
	Unique, as *regression coefficient* is in the *same units* as original outcome
**Logistic** : categorical with more than 2 categories
	Odds ratio
**Cox** : time-to-event (TTE) data (ex: the time it takes from diagnosis to die), survival analysis
	Hazard ratio
**Poisson** : rate per outcome (count or rate)
	Rate ratios, incidence rate ratios

##### Simple Linear Regression
- between two continuous variables
- *Pearson Linear Correlation Coefficient*
	- How correlated are these variables?
	- Not strength, but predict rate of influence
- Units
	*Intercept* (B0)
		Not always meaningful (measures at 0)
	*Slope* (B1)
		Unit change Y per unit change X

##### Multiple Linear Regression
- continuous but more risk factors (independent variables)
- More efficient than strata-based when data is sparse
- If it improves your prediction model you could put it in -- BUT is the variable relevant. What should be included?  
	- *Stepwise regression*: when controlling for X,Y,Z, the effect of exposure on outcome is/is no longer significant
	- Does not account for theoretical modelling

##### Logistic Regression
- The probability of y given x = VALUE
Categorical values are forced
- continuous variable --> binary categories
	- Ex: height/weight --> BMI = Normal/Overweight/Obese
- Not a Normal distribution
- Popular multiple variable regression => can turn into an *odds ratio*!

- If variables are too correlated (multicollinearity) it messes with the model

##### Cox Proportional Hazard Regression
- Technique for using TTE and censored data
- Most used multivariable approach for survival data
- The probability that if a person survives to time *t*, that they will experience the outcome in that instant 
	- h(t) given t
- phreg 
	- Pr > X^2 tells whether variable effect is significant (in slide example, gender is not, age is (= 0.5))
	- Interpret: At any point in time, [CATEGORICAL] have 0.### times the hazard of [EVENT] than [CATEGORICAL2].
	- Interpret: At any point in time, for every increase in [CONT. VARIABLE] the hazard of [EVENT] is increased by 0.####.
- If there is a violation that the effect changes over the duration of the study, *stratification* of that variable (like age) may be more viable

##### Poisson Regression
- Count ONLY if there is same f/u time
- Rate if it is different, include denominator to standardize effect size
- Interpret: [A] has more/less XX times per [time unit] than [B].

