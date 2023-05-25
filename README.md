# monte_carlo_simulation
This is the Monte Carlo simulation for GBP vs USD

This is my approach to calculate the Monte Carlo simulation for FX (GBP vs USD) 

Here's a summary of the steps you followed:

Generate random numbers from a normal distribution using np.random.normal().
Calculate the exponential of the smallest value in the 'variation' column using np.min() and np.exp().
Create a new column called 'new_price' by multiplying the 'Close' column with the exponential value.
Iterate over the remaining rows and calculate the 'new_price' by multiplying the previous day's 'new_price' with the exponential of the current day's 'variation'.
Plot the simulated values using matplotlib.
