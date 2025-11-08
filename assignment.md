# Assignment

## Brief

Write the Python codes for the following questions.

## Instructions

Paste the answer as Python in the answer code section below each question.

### Question 1

Question: How do you create a 2x2 subplot grid in matplotlib and select the first subplot?

Answer:

```python
import matplotlib.pypolt as plt

fig = plt.figure()
ax1 = fig.add_subplot(2, 2, 1)
```

### Question 2

Question: How to plot a line and set the color to red and style to dash in a matplotlib plot?

```python
x = [1, 2, 3, 4]
y = [1, 4, 9, 16]
```

Answer:

```python
plt.plot(x, y, color='red', linestyle='dashed')
```

### Question 3

Question: How to plot a histogram with 30 bins for `data` in matplotlib?

```python
import numpy as np
data = np.random.randn(1000)
```

Answer:

```python
plt.hist(data, bins=30)
plt.show()
```

### Question 4

Question: How can you set the x-axis and y-axis labels in a matplotlib plot?

Answer:

```python
plt.hist(data, bins=30)
plt.xlabel('Value')
plt.ylabel('Frequency')
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
avg_tip = tips.groupby('day')['tip'].mean().reset_index()
sns.barplot(x='day', y='tip', data=avg_tip)
plt.show()
```

### Question 6

Question: How to create a box plot for total_bill categorized by day in the `tips` dataset using seaborn?

Answer:

```python
sns.catplot(x='total_bill', y='day', kind='box', data=tips)
```

## Submission

- Submit the URL of the GitHub Repository that contains your work to NTU black board.
- Should you reference the work of your classmate(s) or online resources, give them credit by adding either the name of your classmate or URL.
