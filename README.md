# Agent-Base-Modeling-for-Reproducible-Final-Market-Share

In both agent-based models and other sufficiently complicated economic models, there may be path-dependent effects: The trajectory or outcome of individual replications may depend strongly on random effects that occur early in the computation. This creates obstacles for good research with reproducible results. Here the main interest is in the final market share of the second-most widely used technology (after 5000 time periods as is the default).

**Focus:**

The output value of interest ( market share of the second-most widely used technology ) is not reproducible in individual runs because of randomness. In order to get a reproducible result, we need to run a series of simulations, collect the target values, and analyze them. We can also plot the target value to figure out if it has a common pattern or distribution.

### 1. Experiment
The following experiment is designed:

- **Experimental units:** The experimental unit is replication runs of the ABM. 100 replications will be used (other default values remain unchanged).

- **Hypotheses:**  
  The final market share of the second most widely used technology should be lower than the final market share of the most widely used technology. Plot the market shares to find distributions.

- **Treatments:** The default values from the class Simulation remain unchanged.

- **Response:**  
  For each simulation run:  
  The final market share (after 5000 time periods as is the default) will be collected for the most and second-most widely used technology.

- **Scope parameter:**  
  All default values are used from the Simulation class. In the Experiment class, there are parameters to manipulate the network type and the number of agents of the Simulation class. Different numbers of replications can be chosen.

### 2. Approach
In the Experiment class, the entire experiment is defined. The final market share of the most and second-most widely used technology is collected and analyzed (a function is defined to compute the market share of the most and second-most widely used technology).

### 3. How to run the code
The script can be executed directly. It will print the resulting means and standard deviations into the interpreter and show a histogram when the experiment is complete.

### 4. Code
Please see the `.py` file.

### 5. Results
- **Largest Market Share:** 0.93 ± 0.088  
- **Second Largest Market Share:** 0.05 ± 0.08  

### 6. Interpretation
The output value of interest (market share of the second-most widely used technology) is not reproducible in individual runs because of randomness.  
To get a reproducible result, we need to run a series of simulations, collect the target value, and analyze them. We can also plot the target value to determine if it has a common pattern or distribution. From the figure we can see that the final market share of the second-most widely used technology mostly lies in the range 0 to 0.2.  Second largest market share closely follows logarithmic distribution in the range 0.0 to 0.2.

![Random Output](https://github.com/MohidulHaqueTushar/Agent-base-Modeling-for-Reproducible-Result/blob/main/Image/Largest%20and%20Second%20Largest%20Market%20Share.JPG)
