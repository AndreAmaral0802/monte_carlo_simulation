# monte_carlo_simulation
This is the Monte Carlo simulation for GBP vs USD

This is my approach to calculate the Monte Carlo simulation for FX (GBP vs USD) 

Here's a summary of the steps you followed:

Generate random numbers from a normal distribution using np.random.normal().
Calculate the exponential of the smallest value in the 'variation' column using np.min() and np.exp().
Create a new column called 'new_price' by multiplying the 'Close' column with the exponential value.
Iterate over the remaining rows and calculate the 'new_price' by multiplying the previous day's 'new_price' with the exponential of the current day's 'variation'.
Plot the simulated values using matplotlib. 



The concept: 
Monte Carlo simulation is a computational technique used to model and analyze complex systems or processes through repeated random sampling. It takes its name from the famous Monte Carlo casino in Monaco, known for its games of chance. This simulation method is widely used in various fields such as finance, engineering, physics, and computer science.

At its core, Monte Carlo simulation involves generating random numbers to simulate the behavior of a system. The system can be represented by a mathematical model or a set of rules. By repeating this random sampling process multiple times, the simulation produces a range of possible outcomes, allowing analysts to estimate the likelihood of different results and make informed decisions.

The Monte Carlo simulation process typically follows these steps:

Define the problem: Clearly state the objective of the simulation and the variables involved. Identify the key parameters and their distributions.

Build a model: Develop a mathematical or computational model that represents the system being analyzed. This model should capture the relevant interactions and uncertainties.

Generate random inputs: Determine the probability distributions for the input variables and use random number generators to generate samples from these distributions.

Run the simulation: Apply the model to the generated inputs and simulate the system's behavior. Repeat this process multiple times, using different sets of random inputs.

Analyze the results: Collect and analyze the output data from the simulations. Calculate statistics, such as means, standard deviations, and percentiles, to understand the range of possible outcomes and their probabilities.

Draw conclusions: Interpret the results and draw conclusions about the system being analyzed. Assess the risks and uncertainties associated with the system, and make informed decisions based on the simulation findings.

Monte Carlo simulation provides a powerful tool for decision-making under uncertainty. It allows analysts to account for variability and assess the impact of different factors on the system's behavior. By incorporating randomness and sampling, it provides a comprehensive and probabilistic understanding of complex systems, helping to inform strategic planning, risk assessment, and optimization efforts.
