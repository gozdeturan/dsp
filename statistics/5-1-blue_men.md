[Think Stats Chapter 5 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2006.html#toc50) (blue men)

```python
# Import needed libraries
import scipy.stats

# Set values for the given mean and standard deviation
mu    = 178
sigma = 7.7

# Create a normal distribution by using scipy.stats.norm 
dist = scipy.stats.norm(loc=mu, scale=sigma)

# Convert heights for the given height range 5′10″ and 6′1″
lowest  = 177.8 	# 5'10"
highest = 185.4 	# 6'1"	

# Determine percentage of people below 5'-10"
low = dist.cdf(lowest) 

# Determine percentage of people below 6'-1"   
high = dist.cdf(highest)  

# Determine percentage of people between 5'-10" & 6'-1" by subtracting  
result = high-low
print("Percentage of the U.S. male population between 5’10” and 6’1 is:", result)
```
Percentage of the U.S. male population between 5’10” and 6’1 is: 0.34209468294595308
