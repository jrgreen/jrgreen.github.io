---
layout: page
title: Thermodynamic entropy
description: Notes
parent: pages
---

- In thermodynamics, we often focus on a system of interest. What remains is the surroundings. Together, the system and surroundings comprise the universe.
- Let's consider the system, surroundings, and total entropy changes for a __closed system__. Isolating the system is then synonymous with making the boundary adiabatic.
- **System**
	- A definition of entropy changes for the system
	  $$dS_{\text{sys}}=dS_{\text{prod}}+dS_{\text{flow}}=dS_{\text{prod}}+\displaystyle\frac{\delta q_{\text{sys}}}{T}$$
		- There can be an increase in the entropy due to the system being away from equilibrium and changing spontaneously: the "entropy production" or $$dS_{\text{prod}}$$.
			- We have not said yet how we might calculate the entropy production. We will see that it depends on the process.
			- As an example, this extra entropy can be "produced" by local hot spots in the system that dissipate as the system relaxes to thermodynamic equilibrium.
			- In an {{alias ((3a474551-bcfc-47df-9728-dc6c6377f1ac))isolated}} system, this type of process is the only way the entropy of the system can increase.
		- If the system is not isolated, there can also be a change in the entropy of the system caused by energy exchange with the surroundings as heat: the "entropy flow" $$dS_{\text{flow}}$$.
			- If the closed system is isolated, $$dS_{\text{flow}}=0$$.
			- Otherwise, the entropy flow is $$dS_{\text {flow}} = \delta q_{\text{sys}}/T$$.
	- The entropy $$S_{\text{sys}}$$ is a state function; the entropy production and flow are not.
		- If the system goes from state A to state B, the change in entropy of the system $$dS_{\text{sys}}$$ does not depend on whether the path was reversible or irreversible - the entropy change of the system will be same.
		- Because the entropy production and flow are path functions, their values will depend on whether the process connecting states A and B is reversible or irreversible.
		- The amount of entropy production and entropy flow add to give the same change in entropy of the system between A and B, regardless of the process.
		- Since entropy is a state function, we can choose any path we like to calculate the change from A to B. The entropy change must be the same for all paths that start at A and end in B.
	- The entropy production (and entropy flow) depend on the path, i.e., whether the process is reversible or not.
		- Even though they are path functions $$dS_{\text{sys}}=dS_{\text{prod}}+dS_{\text{flow}}$$. Recall, $$U$$ is a state function; heat and work are not. Still, $$dU=\delta q + \delta w$$.
		- I use $$dS_{\text{prod}}$$ and $$dS_{\text{flow}}$$ instead of $$\delta S_{\text{prod}}$$ and $$\delta S_{\text{flow}}$$.
	- For an idealized, reversible process, the system is at equilibrium at every point along the path.
		- $$dS_{\text{prod}}=0$$ since $$dS_{\text{total}} =0$$ and
		  $$dS_{\text{sys}}=dS_{\text{prod}}+\displaystyle\frac{\delta q_{\text{sys,rev}}}{T_{\text{sys}}}=-dS_{\text{surr}}=-\displaystyle\frac{\delta q_{\text{surr}}}{T_{\text{surr}}}$$
		- The relationship between the entropy change of the system and surroundings here is true only for reversible processes.
		- For $$dS_{\text{sys}}=-dS_{\text{surr}}$$, the entropy production must be zero and the system and surroundings must maintain thermal equilibrium, $$T_{\text{sys}}=T_{\text{surr}}$$.
		- We choose the reversible path for calculations of entropy changes of the system because it is well defined and can be calculated. And, since the entropy change of the system is a state function, we need only calculate it once. The same entropy change of the system will occur for irreversible processes too.
	- For an irreversible process, the system will not be at equilibrium between the initial and final equilibrium states.
		- The entropy flow depends on the path because the amount of energy transferred as heat $$\delta q_{\text{sys}}$$ depends on the path.
			- From the general definition of the entropy of the system,
			  $$dS_{\text{sys}}-dS_{\text{prod}}=\displaystyle\frac{\delta q_{\text{sys}}}{T_{\text{sys}}}=dS_{\text{flow}}$$.
		- The entropy production depends on the path because the amount of energy transferred as heat $$\delta q_{\text{sys}}$$ depends on the path.
			- The spontaneous changes inside the system mean $$dS_{\text{prod}} > 0$$.
				- Solving for the entropy production:
				  $$dS_{\text{prod}}=dS_{\text{sys}}-\displaystyle\frac{\delta q_{\text{sys}}}{T_{\text{sys}}}\geq 0$$.
			- Since the entropy production is positive, we can drop it to find the [[Clausius inequality]]:
			  $$dS_{\text{sys}}\geq\displaystyle\frac{\delta q_{\text{sys}}}{T_{\text{sys}}}=dS_{\text{flow}}$$
				- The entropy production rectifies the inequality and quantifies the entropy increase from irreversible changes in the system.
			- In other words,
			  $$dS_{\text{prod}}=dS_{\text{sys}} - \displaystyle\frac{\delta q_{\text{sys}}}{T_{\text{sys}}}\geq 0$$.
- **Surroundings**
	- The entropy change is related to the amount of energy that enters the surroundings in the form of heat divided by the temperature of the surroundings.
	  $$dS_{\text {surr}}=\displaystyle\frac{\delta q_{\text {surr}}}{T_{\text {surr}}}$$
	- Since we typically give heat a sign based on the perspective of the system, the heat gained/lost by the surroundings is equal to the heat lost/gained of the system: $$\delta q_{\text{sys}} = -\delta q_{\text{surr}}$$
	- Energy flowing as heat out of the system is gained by the surroundings. Then entropy change of the surroundings is
	  $$dS_{\text {surr}}=\displaystyle\frac{\delta q_{\text {surr}}}{T_{\text {surr}}}=-\displaystyle\frac{\delta q_{\text {sys}}}{T_{\text {surr}}}$$
	- If the temperature of the system and the surroundings are the same $$T$$
	  $$dS_{\text {surr}}=\displaystyle\frac{\delta q_{\text{surr}}}{T}=-\displaystyle\frac{\delta q_{\text {sys}}}{T}$$
	- The numerical values of $$\delta q$$ may be positive or negative depending on the direction of energy exchange.
- **Total entropy**
	- The total entropy is not a state function.
	- The second law of thermodynamics is:
	  $$dS_{\text{total}}=dS_{\text {sys}}+dS_{\text{surr}} \geq 0$$
		- If there is a "spontaneous change" $$dS_{\text{tot}} > 0$$ or there is not and the universe is at equilibrium $$dS_{\text{tot}} = 0$$
		- The entropy change of the system can be positive or negative; the entropy change of the surroundings can be positive or negative.
		- The sum of these positive/negative changes must be nonnegative.
	- If the system is isolated, then $$dS_{\text{surr}}=0$$ and $$dS_{\text{total}}=dS_{\text {sys}}$$. No heat can be exchanged between the system and the surroundings.
	  id:: 3a474551-bcfc-47df-9728-dc6c6377f1ac
		- An isolated system is not able to exchange energy with the surroundings as heat or work. That is, $$\delta q_{\text{sys}}=0$$.
		- $$dS_{\text{total}}=dS_{\text {sys}}\geq 0$$
			- If $$dS_{\text{sys}} = 0$$, the system is at equilibrium and the entropy cannot change.
				- $$dS_{\text{prod}} = 0$$ because $$dS_{\text{sys}}=0$$ and $$\delta q_{\text{sys}}/T_{\text{sys}}=0$$
			- If $$dS_{\text{sys}} > 0$$, the system is not at equilibrium and the entropy increases.
				- Examples
					- A gas confined to a small volume and allowed to expand to a larger volume at fixed $$n$$ and $$V$$.
					- One side of the system has a higher temperature than the other side and the two sides equilibrate to the same temperature.
				- The system is isolated so $$\delta q_{\text{sys}}/T_{\text{sys}}=0$$, which means $$dS_{\text{sys}}=dS_{\text{prod}}=dS_{\text{total}} >0$$
				- This entropy change of the irreversible process is the entropy production.
	- If the system is not isolated, it interacts with the surroundings exchanging energy via heat and work. That is, $$\delta q_{\text{sys}}\neq 0$$.
		- The change in the surroundings due to exchange of energy as heat is exactly equal and opposite to the change in the system due to the exchange of energy as heat, $$\delta q_{\text {sys}}=-\delta q_{\text {surr}}$$.
			- There are no losses of energy; the system and surroundings together make up the universe.
		- The total entropy change for the system is:
		  $$d S_{\text {system}}=d S_{\text {prod}}+dS_{\text {flow}}$$
		- Putting this all together,
		  $$dS_{\text{total}}=dS_{\text{sys}}+dS_{\text{surr}}$$
		  $$dS_{\text{total}}=\left(dS_{\text {prod}}+dS_{\text {flow}}\right)+dS_{\text{surr}}$$
		  $$dS_{\text{total}}=\left(dS_{\text{prod}}+\displaystyle\frac{\delta q_{\text{sys}}}{T_{\text{sys}}}\right)+\displaystyle\frac{\delta q_{\text{surr}}}{T_{\text{surr}}}$$
		  $$dS_{\text{total}}=\left(dS_{\text{prod}}+\displaystyle\frac{\delta q_{\text{sys}}}{T_{\text{sys}}}\right)-\displaystyle\frac{\delta q_{\text{sys}}}{T_{\text{surr}}}\geq 0$$
		- If $$T_{\text{sys}}=T_{\text{surr}}$$, the total entropy change is the entropy production $$dS_{\text{total}}=dS_{\text{prod}}\geq 0$$
		- If $$T_{\text{sys}}\neq T_{\text{surr}}$$, then the total entropy change is not just the entropy production
		  $$dS_{\text{total}}=dS_{\text{prod}}+\delta q_{\text{sys}}\left(T_{\text{sys}}^{-1}-T_{\text{surr}}^{-1}\right)\geq 0$$
			- Or, $$dS_{\text{prod}}\geq \delta q_{\text{sys}}\left(T_{\text{surr}}^{-1}-T_{\text{sys}}^{-1}\right)$$
			- The entropy production is nonnegative; the term on the right may be positive or negative.
			- If $$T_{\text{sys}}=T_{\text{surr}}$$, we can see that the entropy production is nonnegative.
- __Reversible processes__: if the system is at equilibrium, then there is no spontaneous change.
	- The total change in the entropy should be zero $$dS_{\text{total}}=dS_{\text{prod}}+\delta q_{\text{sys}}\left(T_{\text{sys}}^{-1}-T_{\text{surr}}^{-1}\right)= 0$$
	- Since there are no irreversible processes inside the system
	  $$dS_{\text{prod}} = 0$$
	- Since the system and surroundings are always in thermal equilibrium $$\delta q_{\text{sys}}\left(T_{\text{sys}}^{-1}-T_{\text{surr}}^{-1}\right)= 0$$
	- The change in the system and surroundings may not be zero, they will be equal in amplitude with opposite sign:
	  $$dS_{\text{sys}}=-dS_{\text{surr}}$$
	- If the system is not at equilibrium, then $$dS_{\text{prod}}>0$$ and $$dS_{\text{total}}>0$$ indicating spontaneous change
- __Irreversible processes__: the system is not at equilibrium and there are spontaneous changes.
	- The entropy change in the system is the same for the reversible and irreversible paths
		- __However, the entropy change of the system is divided differently between the entropy production (from spontaneous changes in the system) and the entropy flow (associated with energy exchanged as heat with the surroundings).__
			- For reversible processes, $$dS_{\text{prod}} = 0$$, so $$dS_{\text{sys}} = \delta q_{\text{sys}}/T_{\text{sys}}$$
			- For irreversible processes, $$dS_{\text{prod}} > 0$$ and $$dS_{\text{sys}} > \delta q_{\text{sys}}/T_{\text{sys}}$$
			- The value of $$dS_{\text{sys}}$$ is the same for reversible and irreversible processes.
			- The entropy production $$dS_{\text{prod}}$$ and flow $$\delta q_{\text{sys}}$$ are not the same.
			- We have not yet considered the surroundings.
	- The entropy change of the surroundings is different for reversible and irreversible paths.
		- The change depends on the path because it is related to the entropy flow and the entropy flow depends on the path.
			- For reversible processes, $$dS_{\text{prod}} = 0$$, so $$dS_{\text{sys}} = -\delta q_{\text{surr}}/T_{\text{sys}}$$
				- If $$T_{\text{sys}}=T_{\text{surr}}$$, then $$dS_{\text{sys}} = -\delta q_{\text{surr}}/T_{\text{surr}} = -dS_{\text{surr}}$$
				- The entropy changes of the system and surroundings are equal in magnitude
			- For irreversible processes, $$dS_{\text{prod}} > 0$$ and $$dS_{\text{sys}} > -\delta q_{\text{surr}}/T_{\text{sys}}$$
				- If $$T_{\text{sys}}=T_{\text{surr}}$$, then $$dS_{\text{sys}} > -\delta q_{\text{surr}}/T_{\text{surr}} = -dS_{\text{surr}}$$
				- The entropy changes of the system and surroundings are not equal in magnitude
		- The entropy change of the surroundings depends on the path because the total entropy change depends on the path
			- The second law $$dS_{\text{total}}=dS_{\text{sys}}+dS_{\text{surr}}\geq 0$$ says that the total entropy change depends on the path
			- If $$S_{\text{sys}}$$ is a state function, then $$dS_{\text{surr}}$$ must depend on the path for the second law to be true.
		- Example
			- Consider when energy is absorbed as heat by the system, $$\delta q_{\text{sys}}>0$$, $$\delta q_{\text{surr}}<0$$.
			- When energy flows as heat from the surroundings to the system, the entropy of the surroundings decreases, $$dS_{\text{surr}}<0$$.
			- The change in the entropy of the system increases;  energy is gained as heat so it will be positive $$dS_{\text{sys}}>0$$. The increase is the same in the reversible and irreversible processes.
			- The total change in entropy $$dS_{\text{total}}\geq 0$$ by the second law.
			- Now we can compare reversible and irreversible processes when $$T_{\text{sys}}=T_{\text{surr}}=T$$
				- The entropy change $$dS_{\text{sys}}$$ is the same in the reversible and irreversible process because $$S_{\text{sys}}$$ is a state function.
				- The entropy change of the surroundings $$dS_{\text{surr}}$$ changes less in an irreversible process than in a reversible process
				  $$dS_{\text{sys}}\geq \displaystyle\frac{\delta q_{\text {sys}}}{T}=-\displaystyle\frac{\delta q_{\text {surr}}}{T}=-dS_{\text{surr}}$$
				  or
				  $$dS_{\text{sys}}+dS_{\text{surr}}\geq 0$$
				  which can only be true when $$|dS_{\text{sys}}|\geq |dS_{\text{surr}}|$$.
					- $$|dS_{\text{sys}}|$$ is the same in reversible and irreversible processes. It is only equal to $$|dS_{\text{sys}}|$$ for a reversible process because $$|dS_{\text{sys}}|$$ depends on the path.
				- The entropy of the system increases more than the surroundings for irreversible processes because $$dS_{\text{prod}} \geq 0$$.
					- Remember the entropy production is $$dS_{\text{sys}}-\delta q_{\text {sys}}/T\geq 0$$ so $$dS_{\text{total}} = dS_{\text{prod}} = dS_{\text{sys}}+dS_{\text{surr}}\geq 0$$.
				- When energy is transferred irreversibly as heat, there is a nonzero entropy production. How do we interpret a nonzero entropy production?
					- The energy transferred as heat disturbs the system from a state of equilibrium. The equilibration of the system (spreading of energy throughout the system) adds a contribution to the entropy change of the system.
				- In the irreversible process, less energy is needed as heat from the surroundings to increase the entropy of the system, $$dS_{\text{sys}}$$, at a temperature $$T$$
					- $$TdS_{\text{sys}}=\delta q_{\text {sys,rev}}\geq \delta q_{\text{sys}}$$
					- $$TdS_{\text{prod}} = TdS_{\text{sys}} - \delta q_{\text{sys}} = \delta q_{\text {sys,rev}}- \delta q_{\text{sys}}\geq 0$$
					- In this example, both $$\delta q > 0$$, so more energy is transferred as heat in the reversible process than the irreversible process.
					- More energy is needed to increase the entropy of the system by a fixed amount in the reversible process because there are not spontaneous, irreversible changes inside the system.
