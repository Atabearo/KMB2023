
Cumulative survival - not necessarily mortality, but disease-free 
- Inverse of cumulative incidence

Incidence rate (censorship)
- Crude incidence is min IR
- Max IR is when we assume the censored subjects would have gotten condition
	**How to calculate censored observations** for incidence
		Classic Life Table Approach (cumulative incidence, used censored data and don't have person-time data)
		- censored observations contribute 1/2 the person risk in denom
			q = d/Ic
				q= CI
				d= condition events (#)
				I= initial population
				c=correction for censored observations (# of censored indivs * .05)
		Kaplan Meier method
			q=d/n
				q= incidence
				d= condition events (#)
			Only includes number under observation (actuarial halves censored #)
Assumptions in Survival Anlaysis
- no birth/period effects affecting survival
- Events/withdrawals occur uniformly
- Censoring is independent of survival
**Incidence based on person-time**

***Relative measures***
2x2 table
	RR: Ie/Ine
	OR: Oe/One
		OR is used to approximate of RR when we don't have the data to calc RR. If disease/outcome is rate, OR is good approximation
AR (attributable risk): Ie - Ine 
	Interpretation: there is a #.#% excess incidence of ... among those with exposure.
%AR: Ie - Ine / Ie * 100
	##.#% of risk of condition among those with exposure is attributable to exposure
Absolute Risk Reduction
	Inverse of attributable risk (used when exposure is protective)  
	Ine - Ie (Or, incidence among control - incidence among intervention)
Efficacy
	Grade: how well did it perform in the study population? (inverse of %AR)
	Ine - Ie / Ine 
(number needed to treat:) NNT = 1/ARR
	To prevent one condition, we need to treat approx # people with exposure
		Usually used for cost analysis

Relative vs absolute measures
	Relative: strength of relationship between two variables
	Absolute: better for understanding PUBH impact of disease