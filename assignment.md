# Assignment

## Brief

Write the Python codes for the following questions.

## Instructions

Paste the answer as Python in the answer code section below each question.

### Question 1

Question: How do you create a 2x2 subplot grid in matplotlib and select the first subplot?

Answer:

```python

import matplotlib.pyplot as plt

# Create a 2x2 grid of subplots
fig, axes = plt.subplots(2, 2)

# Select the first subplot (top-left)
ax1 = axes[0, 0]

# Example: Plot something in the first subplot
ax1.plot([1, 2, 3], [4, 5, 6])
ax1.set_title("First Subplot")

# Show the figure
plt.show()
```

### Question 2

Question: How to plot a line and set the color to red and style to dash in a matplotlib plot?

```python
x = [1, 2, 3, 4]
y = [1, 4, 9, 16]
```

Answer:

```python
import matplotlib.pyplot as plt

x = [1, 2, 3, 4]
y = [1, 4, 9, 16]

# Plot the line with red color and dashed style
plt.plot(x, y, color='red', linestyle='--')

# Show the plot
plt.show()
```

### Question 3

Question: How to plot a histogram with 30 bins for `data` in matplotlib?

```python
data = np.random.randn(1000)
```

Answer:

```python
import matplotlib.pyplot as plt
import numpy as np

data = np.random.randn(1000)

# Plot the histogram with 30 bins
plt.hist(data, bins=10)

# Show the plot
plt.show()
```

### Question 4

Question: How can you set the x-axis and y-axis labels in a matplotlib plot?

Answer:

```python
import matplotlib.pyplot as plt

x = [1, 2, 3, 4]
y = [1, 4, 9, 16]

# Create a plot
plt.plot(x, y)

# Set the x-axis and y-axis labels
plt.xlabel("X-axis Label")
plt.ylabel("Y-axis Label")

# Show the plot
plt.show()
```

### Question 5

Question: How do you create a bar plot in seaborn using the `tips` dataset to show the average tip amount per day?

```python
import seaborn as sns
tips = sns.load_dataset('tips')
```

Answer:

```python
import seaborn as sns

# Load the tips dataset
tips = sns.load_dataset('tips')

# Create a bar plot for the average tip amount per day
sns.barplot(x='day', y='tip', data=tips,errorbar=None)

```

### Question 6

Question: How to create a box plot for total_bill categorized by day in the `tips` dataset using seaborn?

Answer:

```python
import seaborn as sns
import matplotlib.pyplot as plt

# Load the tips dataset
tips = sns.load_dataset('tips')

# Create a box plot for total_bill categorized by day
sns.boxplot(x='day', y='total_bill', data=tips)

# Show the plot
plt.show()
```

## Submission

- Submit the URL of the GitHub Repository that contains your work to NTU black board.
- Should you reference the work of your classmate(s) or online resources, give them credit by adding either the name of your classmate or URL.
