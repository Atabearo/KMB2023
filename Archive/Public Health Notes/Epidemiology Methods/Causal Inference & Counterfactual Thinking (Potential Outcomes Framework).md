Counterfactual: counter to reality: "what MIGHT have been" or "how could things be different"
- a work of imagination

There is an inherent causal question to association questions.
- our ultimate goal IS policy change
- If association --> if cause --> then change
###### Example
Question: Exposure to air pollution associated with increased risk of asthma?
- IF FOUND, policy change for reducing air pollution?
- Causal question: Does exposure to specific levels of air pollution cause an increase int he incidence of asthma among children compared to those exposed to lower levels of pollution?

![[Pasted image 20240220145041.png]]How to determine if it is an *individual-level* causal effect:
![[Pasted image 20240220145332.png]]

Average causal effects:
![[Pasted image 20240220145656.png]]
- IF probability is equal, then it is NOT causal (as there was no difference in whether they received the treatment anyway)

###### Identifiable conditions
- Consistency
	People who were assigned the treatment, the outcome would have been the same (had there been no study) if the same people were exposed
	Requires a well-defined intervention and outcome of interests
		SUTVA
- Positivity
	- Individuals in the population, all have a nonzero probability of (not) receiving treatment
- Exchangeability **(the only one we can analytically induce)**
	- The outcomes are independent of treatment assignment (the risk of outcome is same)
		- Randomization => *baseline comparability*
	- This is not often met, so researchers can condition on a set of covariates to analytically create exchangeability 
	- known as **conditional exchangeability
