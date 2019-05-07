---
title: "Visualization"
author: "WeizhouS"
date: "3/23/2019"
output: pdf_document
---

``` py
import matplitlib.pyplot as plt

# line plot
plt.plot(x, y)

# scatter plot
plt.scatter(x, y)

# change to log scale
plt.xscale('log')

# add labels
plt.xlabel('xlab')
plt.ylabel('ylab')
plt.title('a nice plot')

# Specify c and alpha inside plt.scatter(), alpha is opacity
plt.scatter(x = gdp_cap, y = life_exp, s = np.array(pop) * 2, c = col, alpha = 0.8)

# change ticks
plt.yticks([1,2,3], ['1b', '2b', '3b'])

# histogram
plt.hist(x, bins=10)





# show the plot
plt.show()

# clean up figure
plt.clf()












```




- pandas is built on numpy
- dataframe from dictionary

Dataframe square brackets
- Column access
- Row access only through slicing

loc:
- `brics.loc[["RU", "IN"]]`
- `brics.loc[:, ['country', 'capital']]`
- `brics.loc[['RU', 'CH'], ['country', 'capital']]`


```





```



















































