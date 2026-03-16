#  Mean and variance of a discrete  distribution


# Aim : 

To find mean and variance of arrival of objects from the feeder using probability distribution


# Software required :  

Python and Visual components tool

# Theory:

The expectation or the mean of a discrete random variable is a weighted average of all possible
values of the random variable. The weights are the probabilities associated with the corresponding values. 
It is calculated as,

![image](https://user-images.githubusercontent.com/103921593/192938463-e34177f4-f188-48a0-bda2-8f6d1d660ed2.png)

The variance of a random variable shows the variability or the scatterings of the random variables.
It shows the distance of a random variable from its mean. It is calcualted as

![image](https://user-images.githubusercontent.com/103921593/192938695-99fedc01-34d5-4d36-84df-5880e766ed0c.png)


# Procedure :

1. Construct frequency distribution for the data

2. Find the  probability distribution from frequency distribution.

3. Calculate mean using 
   
   ![image](https://user-images.githubusercontent.com/103921593/192940431-03b81777-c54d-4286-b4f4-82dfe7666b4c.png)

4. Find  
   
      ![image](https://user-images.githubusercontent.com/103921593/192940255-2d9dd746-6875-4a6d-877b-6da6cdb96ab1.png)

5.  Calculate variance using 
  
      ![image](https://user-images.githubusercontent.com/103921593/192942852-913550a9-fabe-4a55-b956-0487b18bbd97.png)


# Program :
```
# Program to find mean and variance of a discrete random variable
# and print x and probability values

# Step 1: Get number of values
n = int(input("Enter number of values: "))

# Step 2: Create empty lists
x_values = []
p_values = []

# Step 3: Get x and p from user
for i in range(n):
    print("\nFor value", i+1)
    x = float(input("Enter value of x: "))
    p = float(input("Enter probability of x: "))
    
    x_values.append(x)
    p_values.append(p)

# Step 4: Print x and probability values
print("\nEntered Values:")
for i in range(n):
    print("x =", x_values[i], " , p =", p_values[i])

# Step 5: Calculate Mean
mean = 0
for i in range(n):
    mean = mean + (x_values[i] * p_values[i])

# Step 6: Calculate Variance
variance = 0
for i in range(n):
    variance = variance + ((x_values[i] - mean) ** 2 * p_values[i])

# Step 7: Print results
print("\nMean =", mean)
print("Variance =", variance)
```


# Output : 
<img width="805" height="704" alt="image" src="https://github.com/user-attachments/assets/93cbb75d-2a1b-4f04-83f1-bb7aa9d8db99" />


# Results :
The mean and variance of arrivals of objects from feeder using probability distribution are calculated.

