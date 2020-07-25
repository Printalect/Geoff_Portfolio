<h1>Table of Contents<span class="tocSkip"></span></h1>
<div class="toc"><ul class="toc-item"><li><span><a href="#This-is-a-plot" data-toc-modified-id="This-is-a-plot-1"><span class="toc-item-num">1&nbsp;&nbsp;</span>This is a plot</a></span></li><li><span><a href="#This-is-a-pandas-dataframe" data-toc-modified-id="This-is-a-pandas-dataframe-2"><span class="toc-item-num">2&nbsp;&nbsp;</span>This is a pandas dataframe</a></span></li></ul></div>

# Testing

This is a written section


```python
x = 3 + 3
print('this is the value of x: ', x)
```

    this is the value of x:  6
    

## This is a plot


```python
import matplotlib
import matplotlib.pyplot as plt
import numpy as np

# Data for plotting
t = np.arange(0.0, 2.0, 0.01)
s = 1 + np.sin(2 * np.pi * t)

fig, ax = plt.subplots()
ax.plot(t, s)

ax.set(xlabel='time (s)', ylabel='voltage (mV)',
       title='About as simple as it gets, folks')
ax.grid()

fig.savefig("test.png")
plt.show()
```


![png](output_5_0.png)


## This is a pandas dataframe


```python
import pandas as pd

cars = {'Brand': ['Honda Civic','Toyota Corolla','Ford Focus','Audi A4'],
        'Price': [22000,25000,27000,35000]
        }

df = pd.DataFrame(cars, columns = ['Brand','Price'], index=['Car_1','Car_2','Car_3','Car_4'])

print (df)
```

                    Brand  Price
    Car_1     Honda Civic  22000
    Car_2  Toyota Corolla  25000
    Car_3      Ford Focus  27000
    Car_4         Audi A4  35000
    


```python

```
