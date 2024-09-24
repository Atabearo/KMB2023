- _causal_ diagram representing variables in a population
	Variables impacting relationship
	- exposure/outcome
	- suspected confounders
	- includes measured and unmeasured variables
- stated conceptual model
- Purpose: used to evaluate **confounding**, selection bias, info bias

#### Components
- causal, not deterministic
- Downstream
- Bi-directional, using time?
	- E1 -> O1 -> E2 -> O2
- Collider
	- Common child (when you condition the child there is an opening for association between parent variables)
	- Types of association-- non-causal association is typically a confounder when sharing a common parent
- ![[Pasted image 20240213141627.png]]
#### Path classifications
- the goal in DAG is to have **open** causal paths AND **close** non-causal paths
- Paths can be closed to have colliders and conditioned on
##### Directed/Causal:
Directed/Causal
Non-causal/not directed: mixed arrows
![[Pasted image 20240213143242.png]]
- Non-causal ***association*** between E and O
- X would make a better exposure 
###### Door:
**Front**: E ->
Back: E <-
- Typically a CONFOUNDER
##### Open:
**Open: association expected**
- no conditions to close off path
- no colliders
	- Do NOT condition a collider, it is already closed. If you condition a collider an association will be found (collider bias)
		- There will be an association that is not real (creating a confounding) ![[Pasted image 20240213145958.png]]![[Pasted image 20240213150037.png|300]] 
Closed: expect no association
![[Pasted image 20240213145156.png]]
- there is NO open path for E to get to O

#### Confounder evaluation
- unblocked backdoor path between E and O
- ![[Pasted image 20240213152712.png]]
	- Traditional confounding
		- C causes E and O, and C is not caused by E or O
		- would change magnitude![[Pasted image 20240213152949.png]]
- The true confounder is U because it **causes E and O**
- The block is on what we can measure
	- NOT confounded
![[Pasted image 20240213153224.png]]
- X is caused by E, an intermediary