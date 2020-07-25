<h1>Table of Contents<span class="tocSkip"></span></h1>
<div class="toc"><ul class="toc-item"><li><span><a href="#Context" data-toc-modified-id="Context-1"><span class="toc-item-num">1&nbsp;&nbsp;</span>Context</a></span></li><li><span><a href="#Content" data-toc-modified-id="Content-2"><span class="toc-item-num">2&nbsp;&nbsp;</span>Content</a></span></li><li><span><a href="#Acknowledgements" data-toc-modified-id="Acknowledgements-3"><span class="toc-item-num">3&nbsp;&nbsp;</span>Acknowledgements</a></span></li><li><span><a href="#Inspiration" data-toc-modified-id="Inspiration-4"><span class="toc-item-num">4&nbsp;&nbsp;</span>Inspiration</a></span></li><li><span><a href="#1.-Data-Info" data-toc-modified-id="1.-Data-Info-5"><span class="toc-item-num">5&nbsp;&nbsp;</span>1. Data Info</a></span><ul class="toc-item"><li><span><a href="#Pairplot" data-toc-modified-id="Pairplot-5.1"><span class="toc-item-num">5.1&nbsp;&nbsp;</span>Pairplot</a></span></li></ul></li><li><span><a href="#Correlation-Matrix" data-toc-modified-id="Correlation-Matrix-6"><span class="toc-item-num">6&nbsp;&nbsp;</span>Correlation Matrix</a></span></li><li><span><a href="#Building-machine-Learning-Models" data-toc-modified-id="Building-machine-Learning-Models-7"><span class="toc-item-num">7&nbsp;&nbsp;</span>Building machine Learning Models</a></span></li><li><span><a href="#Choosing-a-model" data-toc-modified-id="Choosing-a-model-8"><span class="toc-item-num">8&nbsp;&nbsp;</span>Choosing a model</a></span></li></ul></div>


```python
import os
filedir = '\\Users\MasterDK-Laptop\Desktop\Jupyter_Notebooks_1A\DataFiles\Craft-Beer\\'
files = os.listdir(filedir)
files
```




    ['beers.csv', 'breweries.csv']



# Initializing packages


```python
import numpy as np  
import pandas as pd
import os
import matplotlib.pyplot as plt
import seaborn as sns
import sklearn
```

# Importing datasets

# Description about Problem

## Context

It's a great time to be a craft beer fan in the U.S.! There are a ton of beer styles and brands to choose from and breweries have become very successful in the last several years. Breweries owe it all to beer lovers around the world! This dataset contains a list of 2,410 US craft beers and 510 US breweries. The beers and breweries are linked together by the "id". This data was collected in January 2017 from CraftCans.com. The dataset is an a tidy format and values have been cleaned up for your enjoyment.

## Content

beers.csv - Contains data on 2000+ craft canned beers

breweries.csv - Contains data for 500+ breweries in the United States

Abbreviation: ABV: ABV-Alcohol by volume , IBU: International Bitterness Units

## Acknowledgements

If you are interested in learning more about how this dataset was acquired, I wrote an extensive blogpost about it http://www.jeannicholashould.com/python-web-scraping-tutorial-for-craft-beers.html.

## Inspiration

Can you predict the beer type from the characteristics provided in the dataset?

What is the most popular beer in North Dakota?

Cheers to beer


![pintsender.jpg](attachment:pintsender.jpg)

# Understand the dataset


```python
## Craft Canned beer 

craft_canned_beer= pd.read_csv(filedir + files[0])
craft_canned_beer.head()
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Unnamed: 0</th>
      <th>abv</th>
      <th>ibu</th>
      <th>id</th>
      <th>name</th>
      <th>style</th>
      <th>brewery_id</th>
      <th>ounces</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>0</td>
      <td>0.050</td>
      <td>NaN</td>
      <td>1436</td>
      <td>Pub Beer</td>
      <td>American Pale Lager</td>
      <td>408</td>
      <td>12.0</td>
    </tr>
    <tr>
      <th>1</th>
      <td>1</td>
      <td>0.066</td>
      <td>NaN</td>
      <td>2265</td>
      <td>Devil's Cup</td>
      <td>American Pale Ale (APA)</td>
      <td>177</td>
      <td>12.0</td>
    </tr>
    <tr>
      <th>2</th>
      <td>2</td>
      <td>0.071</td>
      <td>NaN</td>
      <td>2264</td>
      <td>Rise of the Phoenix</td>
      <td>American IPA</td>
      <td>177</td>
      <td>12.0</td>
    </tr>
    <tr>
      <th>3</th>
      <td>3</td>
      <td>0.090</td>
      <td>NaN</td>
      <td>2263</td>
      <td>Sinister</td>
      <td>American Double / Imperial IPA</td>
      <td>177</td>
      <td>12.0</td>
    </tr>
    <tr>
      <th>4</th>
      <td>4</td>
      <td>0.075</td>
      <td>NaN</td>
      <td>2262</td>
      <td>Sex and Candy</td>
      <td>American IPA</td>
      <td>177</td>
      <td>12.0</td>
    </tr>
  </tbody>
</table>
</div>




```python
## dropping id column from beer dataset

craft_canned_beer.drop(['id'],axis=1,inplace=True)
```


```python
# Craft beer
craft_canned_beer.head()
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Unnamed: 0</th>
      <th>abv</th>
      <th>ibu</th>
      <th>name</th>
      <th>style</th>
      <th>brewery_id</th>
      <th>ounces</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>0</td>
      <td>0.050</td>
      <td>NaN</td>
      <td>Pub Beer</td>
      <td>American Pale Lager</td>
      <td>408</td>
      <td>12.0</td>
    </tr>
    <tr>
      <th>1</th>
      <td>1</td>
      <td>0.066</td>
      <td>NaN</td>
      <td>Devil's Cup</td>
      <td>American Pale Ale (APA)</td>
      <td>177</td>
      <td>12.0</td>
    </tr>
    <tr>
      <th>2</th>
      <td>2</td>
      <td>0.071</td>
      <td>NaN</td>
      <td>Rise of the Phoenix</td>
      <td>American IPA</td>
      <td>177</td>
      <td>12.0</td>
    </tr>
    <tr>
      <th>3</th>
      <td>3</td>
      <td>0.090</td>
      <td>NaN</td>
      <td>Sinister</td>
      <td>American Double / Imperial IPA</td>
      <td>177</td>
      <td>12.0</td>
    </tr>
    <tr>
      <th>4</th>
      <td>4</td>
      <td>0.075</td>
      <td>NaN</td>
      <td>Sex and Candy</td>
      <td>American IPA</td>
      <td>177</td>
      <td>12.0</td>
    </tr>
  </tbody>
</table>
</div>




```python
breweries= pd.read_csv(filedir + files[1])
breweries.head()
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Unnamed: 0</th>
      <th>name</th>
      <th>city</th>
      <th>state</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>0</td>
      <td>NorthGate Brewing</td>
      <td>Minneapolis</td>
      <td>MN</td>
    </tr>
    <tr>
      <th>1</th>
      <td>1</td>
      <td>Against the Grain Brewery</td>
      <td>Louisville</td>
      <td>KY</td>
    </tr>
    <tr>
      <th>2</th>
      <td>2</td>
      <td>Jack's Abby Craft Lagers</td>
      <td>Framingham</td>
      <td>MA</td>
    </tr>
    <tr>
      <th>3</th>
      <td>3</td>
      <td>Mike Hess Brewing Company</td>
      <td>San Diego</td>
      <td>CA</td>
    </tr>
    <tr>
      <th>4</th>
      <td>4</td>
      <td>Fort Point Beer Company</td>
      <td>San Francisco</td>
      <td>CA</td>
    </tr>
  </tbody>
</table>
</div>



# Joining breweries and canned beer dataset

The beers and breweries are linked together by the "id".




```python
## creating column name for unnnamed column both in breweries dataset
breweries.rename(columns = {'Unnamed: 0':'id'}, inplace = True) 
craft_canned_beer.rename(columns={'Unnamed: 0':'id'},inplace=True)
breweries.columns
breweries.head()
print(craft_canned_beer.head())

```

       id    abv  ibu                 name                           style  \
    0   0  0.050  NaN             Pub Beer             American Pale Lager   
    1   1  0.066  NaN          Devil's Cup         American Pale Ale (APA)   
    2   2  0.071  NaN  Rise of the Phoenix                    American IPA   
    3   3  0.090  NaN             Sinister  American Double / Imperial IPA   
    4   4  0.075  NaN        Sex and Candy                    American IPA   
    
       brewery_id  ounces  
    0         408    12.0  
    1         177    12.0  
    2         177    12.0  
    3         177    12.0  
    4         177    12.0  
    


```python
beer_breweries_join_dataset= pd.merge(craft_canned_beer,
                 breweries[['id', 'name', 'city','state']],
                 on='id', 
                 how='outer', 
                 indicator=True)

## columns of beer_breweries_joined_dataset
beer_breweries_join_dataset.columns
```




    Index(['id', 'abv', 'ibu', 'name_x', 'style', 'brewery_id', 'ounces', 'name_y',
           'city', 'state', '_merge'],
          dtype='object')




```python
beer_breweries_join_dataset.head()
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>id</th>
      <th>abv</th>
      <th>ibu</th>
      <th>name_x</th>
      <th>style</th>
      <th>brewery_id</th>
      <th>ounces</th>
      <th>name_y</th>
      <th>city</th>
      <th>state</th>
      <th>_merge</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>0</td>
      <td>0.050</td>
      <td>NaN</td>
      <td>Pub Beer</td>
      <td>American Pale Lager</td>
      <td>408</td>
      <td>12.0</td>
      <td>NorthGate Brewing</td>
      <td>Minneapolis</td>
      <td>MN</td>
      <td>both</td>
    </tr>
    <tr>
      <th>1</th>
      <td>1</td>
      <td>0.066</td>
      <td>NaN</td>
      <td>Devil's Cup</td>
      <td>American Pale Ale (APA)</td>
      <td>177</td>
      <td>12.0</td>
      <td>Against the Grain Brewery</td>
      <td>Louisville</td>
      <td>KY</td>
      <td>both</td>
    </tr>
    <tr>
      <th>2</th>
      <td>2</td>
      <td>0.071</td>
      <td>NaN</td>
      <td>Rise of the Phoenix</td>
      <td>American IPA</td>
      <td>177</td>
      <td>12.0</td>
      <td>Jack's Abby Craft Lagers</td>
      <td>Framingham</td>
      <td>MA</td>
      <td>both</td>
    </tr>
    <tr>
      <th>3</th>
      <td>3</td>
      <td>0.090</td>
      <td>NaN</td>
      <td>Sinister</td>
      <td>American Double / Imperial IPA</td>
      <td>177</td>
      <td>12.0</td>
      <td>Mike Hess Brewing Company</td>
      <td>San Diego</td>
      <td>CA</td>
      <td>both</td>
    </tr>
    <tr>
      <th>4</th>
      <td>4</td>
      <td>0.075</td>
      <td>NaN</td>
      <td>Sex and Candy</td>
      <td>American IPA</td>
      <td>177</td>
      <td>12.0</td>
      <td>Fort Point Beer Company</td>
      <td>San Francisco</td>
      <td>CA</td>
      <td>both</td>
    </tr>
  </tbody>
</table>
</div>



# Dropping some columns


```python
beer_breweries_join_dataset.drop(['_merge'],axis=1,inplace=True)

```


```python
beer_breweries_join_dataset.head()
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>id</th>
      <th>abv</th>
      <th>ibu</th>
      <th>name_x</th>
      <th>style</th>
      <th>brewery_id</th>
      <th>ounces</th>
      <th>name_y</th>
      <th>city</th>
      <th>state</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>0</td>
      <td>0.050</td>
      <td>NaN</td>
      <td>Pub Beer</td>
      <td>American Pale Lager</td>
      <td>408</td>
      <td>12.0</td>
      <td>NorthGate Brewing</td>
      <td>Minneapolis</td>
      <td>MN</td>
    </tr>
    <tr>
      <th>1</th>
      <td>1</td>
      <td>0.066</td>
      <td>NaN</td>
      <td>Devil's Cup</td>
      <td>American Pale Ale (APA)</td>
      <td>177</td>
      <td>12.0</td>
      <td>Against the Grain Brewery</td>
      <td>Louisville</td>
      <td>KY</td>
    </tr>
    <tr>
      <th>2</th>
      <td>2</td>
      <td>0.071</td>
      <td>NaN</td>
      <td>Rise of the Phoenix</td>
      <td>American IPA</td>
      <td>177</td>
      <td>12.0</td>
      <td>Jack's Abby Craft Lagers</td>
      <td>Framingham</td>
      <td>MA</td>
    </tr>
    <tr>
      <th>3</th>
      <td>3</td>
      <td>0.090</td>
      <td>NaN</td>
      <td>Sinister</td>
      <td>American Double / Imperial IPA</td>
      <td>177</td>
      <td>12.0</td>
      <td>Mike Hess Brewing Company</td>
      <td>San Diego</td>
      <td>CA</td>
    </tr>
    <tr>
      <th>4</th>
      <td>4</td>
      <td>0.075</td>
      <td>NaN</td>
      <td>Sex and Candy</td>
      <td>American IPA</td>
      <td>177</td>
      <td>12.0</td>
      <td>Fort Point Beer Company</td>
      <td>San Francisco</td>
      <td>CA</td>
    </tr>
  </tbody>
</table>
</div>



# Renaming columns


```python
beer_breweries_join_dataset.rename(columns = {'name_x':'name_of_beer','name_y':'name_of_brewery',}, inplace = True) 
beer_breweries_join_dataset.head()

```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>id</th>
      <th>abv</th>
      <th>ibu</th>
      <th>name_of_beer</th>
      <th>style</th>
      <th>brewery_id</th>
      <th>ounces</th>
      <th>name_of_brewery</th>
      <th>city</th>
      <th>state</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>0</td>
      <td>0.050</td>
      <td>NaN</td>
      <td>Pub Beer</td>
      <td>American Pale Lager</td>
      <td>408</td>
      <td>12.0</td>
      <td>NorthGate Brewing</td>
      <td>Minneapolis</td>
      <td>MN</td>
    </tr>
    <tr>
      <th>1</th>
      <td>1</td>
      <td>0.066</td>
      <td>NaN</td>
      <td>Devil's Cup</td>
      <td>American Pale Ale (APA)</td>
      <td>177</td>
      <td>12.0</td>
      <td>Against the Grain Brewery</td>
      <td>Louisville</td>
      <td>KY</td>
    </tr>
    <tr>
      <th>2</th>
      <td>2</td>
      <td>0.071</td>
      <td>NaN</td>
      <td>Rise of the Phoenix</td>
      <td>American IPA</td>
      <td>177</td>
      <td>12.0</td>
      <td>Jack's Abby Craft Lagers</td>
      <td>Framingham</td>
      <td>MA</td>
    </tr>
    <tr>
      <th>3</th>
      <td>3</td>
      <td>0.090</td>
      <td>NaN</td>
      <td>Sinister</td>
      <td>American Double / Imperial IPA</td>
      <td>177</td>
      <td>12.0</td>
      <td>Mike Hess Brewing Company</td>
      <td>San Diego</td>
      <td>CA</td>
    </tr>
    <tr>
      <th>4</th>
      <td>4</td>
      <td>0.075</td>
      <td>NaN</td>
      <td>Sex and Candy</td>
      <td>American IPA</td>
      <td>177</td>
      <td>12.0</td>
      <td>Fort Point Beer Company</td>
      <td>San Francisco</td>
      <td>CA</td>
    </tr>
  </tbody>
</table>
</div>




```python
##renaming the join dataset a new name

beer_breweries= beer_breweries_join_dataset


# head of dataset
print(beer_breweries.head())
```

       id    abv  ibu         name_of_beer                           style  \
    0   0  0.050  NaN             Pub Beer             American Pale Lager   
    1   1  0.066  NaN          Devil's Cup         American Pale Ale (APA)   
    2   2  0.071  NaN  Rise of the Phoenix                    American IPA   
    3   3  0.090  NaN             Sinister  American Double / Imperial IPA   
    4   4  0.075  NaN        Sex and Candy                    American IPA   
    
       brewery_id  ounces            name_of_brewery           city state  
    0         408    12.0         NorthGate Brewing     Minneapolis    MN  
    1         177    12.0  Against the Grain Brewery     Louisville    KY  
    2         177    12.0   Jack's Abby Craft Lagers     Framingham    MA  
    3         177    12.0  Mike Hess Brewing Company      San Diego    CA  
    4         177    12.0    Fort Point Beer Company  San Francisco    CA  
    


```python
# Tail of dataset
print(beer_breweries.tail())
```

            id    abv   ibu          name_of_beer                     style  \
    2405  2405  0.067  45.0             Belgorado               Belgian IPA   
    2406  2406  0.052   NaN         Rail Yard Ale  American Amber / Red Ale   
    2407  2407  0.055   NaN       B3K Black Lager               Schwarzbier   
    2408  2408  0.055  40.0   Silverback Pale Ale   American Pale Ale (APA)   
    2409  2409  0.052   NaN  Rail Yard Ale (2009)  American Amber / Red Ale   
    
          brewery_id  ounces name_of_brewery city state  
    2405         424    12.0             NaN  NaN   NaN  
    2406         424    12.0             NaN  NaN   NaN  
    2407         424    12.0             NaN  NaN   NaN  
    2408         424    12.0             NaN  NaN   NaN  
    2409         424    12.0             NaN  NaN   NaN  
    

# Preprocessing the joined dataset

## 1. Data Info


```python
# Shape of dataset

print(beer_breweries.shape)

# Dataset Info

beer_breweries.info()
```

    (2410, 10)
    <class 'pandas.core.frame.DataFrame'>
    Int64Index: 2410 entries, 0 to 2409
    Data columns (total 10 columns):
     #   Column           Non-Null Count  Dtype  
    ---  ------           --------------  -----  
     0   id               2410 non-null   int64  
     1   abv              2348 non-null   float64
     2   ibu              1405 non-null   float64
     3   name_of_beer     2410 non-null   object 
     4   style            2405 non-null   object 
     5   brewery_id       2410 non-null   int64  
     6   ounces           2410 non-null   float64
     7   name_of_brewery  558 non-null    object 
     8   city             558 non-null    object 
     9   state            558 non-null    object 
    dtypes: float64(3), int64(2), object(5)
    memory usage: 207.1+ KB
    


```python
### missing value info

print(beer_breweries.isnull().sum())


```

    id                    0
    abv                  62
    ibu                1005
    name_of_beer          0
    style                 5
    brewery_id            0
    ounces                0
    name_of_brewery    1852
    city               1852
    state              1852
    dtype: int64
    


```python
## Replacing missing values of abv and ibu

standard_abv= 0.05
ibu_mean=beer_breweries['ibu'].mean()
beer_breweries.fillna({'abv':standard_abv,'ibu':ibu_mean},inplace=True)
```


```python
# info about dataset after replacing values in nan fields
print(beer_breweries.info())

# looking head of dataset
print(beer_breweries.head())
```

    <class 'pandas.core.frame.DataFrame'>
    Int64Index: 2410 entries, 0 to 2409
    Data columns (total 10 columns):
     #   Column           Non-Null Count  Dtype  
    ---  ------           --------------  -----  
     0   id               2410 non-null   int64  
     1   abv              2410 non-null   float64
     2   ibu              2410 non-null   float64
     3   name_of_beer     2410 non-null   object 
     4   style            2405 non-null   object 
     5   brewery_id       2410 non-null   int64  
     6   ounces           2410 non-null   float64
     7   name_of_brewery  558 non-null    object 
     8   city             558 non-null    object 
     9   state            558 non-null    object 
    dtypes: float64(3), int64(2), object(5)
    memory usage: 207.1+ KB
    None
       id    abv        ibu         name_of_beer                           style  \
    0   0  0.050  42.713167             Pub Beer             American Pale Lager   
    1   1  0.066  42.713167          Devil's Cup         American Pale Ale (APA)   
    2   2  0.071  42.713167  Rise of the Phoenix                    American IPA   
    3   3  0.090  42.713167             Sinister  American Double / Imperial IPA   
    4   4  0.075  42.713167        Sex and Candy                    American IPA   
    
       brewery_id  ounces            name_of_brewery           city state  
    0         408    12.0         NorthGate Brewing     Minneapolis    MN  
    1         177    12.0  Against the Grain Brewery     Louisville    KY  
    2         177    12.0   Jack's Abby Craft Lagers     Framingham    MA  
    3         177    12.0  Mike Hess Brewing Company      San Diego    CA  
    4         177    12.0    Fort Point Beer Company  San Francisco    CA  
    


```python
## filter only missing values

beer_breweries[beer_breweries['state'].isnull()]
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>id</th>
      <th>abv</th>
      <th>ibu</th>
      <th>name_of_beer</th>
      <th>style</th>
      <th>brewery_id</th>
      <th>ounces</th>
      <th>name_of_brewery</th>
      <th>city</th>
      <th>state</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>558</th>
      <td>558</td>
      <td>0.047</td>
      <td>42.713167</td>
      <td>White Zombie Ale</td>
      <td>Witbier</td>
      <td>331</td>
      <td>12.0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>559</th>
      <td>559</td>
      <td>0.052</td>
      <td>42.713167</td>
      <td>Firewater India Pale Ale</td>
      <td>American IPA</td>
      <td>331</td>
      <td>12.0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>560</th>
      <td>560</td>
      <td>0.056</td>
      <td>42.713167</td>
      <td>Farmer Ted's Farmhouse Cream Ale</td>
      <td>Cream Ale</td>
      <td>331</td>
      <td>12.0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>561</th>
      <td>561</td>
      <td>0.048</td>
      <td>16.000000</td>
      <td>Whitecap Wit</td>
      <td>Witbier</td>
      <td>285</td>
      <td>16.0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>562</th>
      <td>562</td>
      <td>0.078</td>
      <td>16.000000</td>
      <td>Seiche Scottish Ale</td>
      <td>Scottish Ale</td>
      <td>285</td>
      <td>16.0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>2405</th>
      <td>2405</td>
      <td>0.067</td>
      <td>45.000000</td>
      <td>Belgorado</td>
      <td>Belgian IPA</td>
      <td>424</td>
      <td>12.0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>2406</th>
      <td>2406</td>
      <td>0.052</td>
      <td>42.713167</td>
      <td>Rail Yard Ale</td>
      <td>American Amber / Red Ale</td>
      <td>424</td>
      <td>12.0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>2407</th>
      <td>2407</td>
      <td>0.055</td>
      <td>42.713167</td>
      <td>B3K Black Lager</td>
      <td>Schwarzbier</td>
      <td>424</td>
      <td>12.0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>2408</th>
      <td>2408</td>
      <td>0.055</td>
      <td>40.000000</td>
      <td>Silverback Pale Ale</td>
      <td>American Pale Ale (APA)</td>
      <td>424</td>
      <td>12.0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>2409</th>
      <td>2409</td>
      <td>0.052</td>
      <td>42.713167</td>
      <td>Rail Yard Ale (2009)</td>
      <td>American Amber / Red Ale</td>
      <td>424</td>
      <td>12.0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
  </tbody>
</table>
<p>1852 rows × 10 columns</p>
</div>




```python
## replacing the nan values of columns name_-f_brewery,city,state,style with mode() values

beer_breweries['name_of_brewery'].fillna(beer_breweries['name_of_brewery'].mode()[0], inplace=True)
beer_breweries['state'].fillna(beer_breweries['state'].mode()[0], inplace=True)
beer_breweries['city'].fillna(beer_breweries['city'].mode()[0], inplace=True)
beer_breweries['style'].fillna(beer_breweries['style'].mode()[0], inplace=True)

```


```python
beer_breweries.info()
```

    <class 'pandas.core.frame.DataFrame'>
    Int64Index: 2410 entries, 0 to 2409
    Data columns (total 10 columns):
     #   Column           Non-Null Count  Dtype  
    ---  ------           --------------  -----  
     0   id               2410 non-null   int64  
     1   abv              2410 non-null   float64
     2   ibu              2410 non-null   float64
     3   name_of_beer     2410 non-null   object 
     4   style            2410 non-null   object 
     5   brewery_id       2410 non-null   int64  
     6   ounces           2410 non-null   float64
     7   name_of_brewery  2410 non-null   object 
     8   city             2410 non-null   object 
     9   state            2410 non-null   object 
    dtypes: float64(3), int64(2), object(5)
    memory usage: 207.1+ KB
    


```python
beer_breweries.tail()
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>id</th>
      <th>abv</th>
      <th>ibu</th>
      <th>name_of_beer</th>
      <th>style</th>
      <th>brewery_id</th>
      <th>ounces</th>
      <th>name_of_brewery</th>
      <th>city</th>
      <th>state</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>2405</th>
      <td>2405</td>
      <td>0.067</td>
      <td>45.000000</td>
      <td>Belgorado</td>
      <td>Belgian IPA</td>
      <td>424</td>
      <td>12.0</td>
      <td>Blackrocks Brewery</td>
      <td>Portland</td>
      <td>CO</td>
    </tr>
    <tr>
      <th>2406</th>
      <td>2406</td>
      <td>0.052</td>
      <td>42.713167</td>
      <td>Rail Yard Ale</td>
      <td>American Amber / Red Ale</td>
      <td>424</td>
      <td>12.0</td>
      <td>Blackrocks Brewery</td>
      <td>Portland</td>
      <td>CO</td>
    </tr>
    <tr>
      <th>2407</th>
      <td>2407</td>
      <td>0.055</td>
      <td>42.713167</td>
      <td>B3K Black Lager</td>
      <td>Schwarzbier</td>
      <td>424</td>
      <td>12.0</td>
      <td>Blackrocks Brewery</td>
      <td>Portland</td>
      <td>CO</td>
    </tr>
    <tr>
      <th>2408</th>
      <td>2408</td>
      <td>0.055</td>
      <td>40.000000</td>
      <td>Silverback Pale Ale</td>
      <td>American Pale Ale (APA)</td>
      <td>424</td>
      <td>12.0</td>
      <td>Blackrocks Brewery</td>
      <td>Portland</td>
      <td>CO</td>
    </tr>
    <tr>
      <th>2409</th>
      <td>2409</td>
      <td>0.052</td>
      <td>42.713167</td>
      <td>Rail Yard Ale (2009)</td>
      <td>American Amber / Red Ale</td>
      <td>424</td>
      <td>12.0</td>
      <td>Blackrocks Brewery</td>
      <td>Portland</td>
      <td>CO</td>
    </tr>
  </tbody>
</table>
</div>




```python
## removing brewery_id,id from beer_breweries dataset

beer_breweries.drop(['brewery_id','id'],axis=1,inplace=True)


```


```python
##dummies creation

# beer_breweries_dummy= pd.get_dummies(beer_breweries[['name_of_beer','style','name_of_brewery','city','state']])
# beer_breweries_dummy.shape
```

# EDA

### Pairplot


```python
sns.pairplot(beer_breweries)

```




    <seaborn.axisgrid.PairGrid at 0x2881c91c0c8>




![png](output_36_1.png)


## Correlation Matrix


```python
##correlation matrix

beer_breweries_corr= beer_breweries.corr()
print(beer_breweries_corr)
beer_breweries_features= beer_breweries_corr.index
plt.figure(figsize=(10,10))
beer_breweries_heatmap= sns.heatmap(beer_breweries[beer_breweries_features].corr(),annot=True,cmap='RdYlGn')
```

                 abv       ibu    ounces
    abv     1.000000  0.516560  0.167589
    ibu     0.516560  1.000000  0.039995
    ounces  0.167589  0.039995  1.000000
    


![png](output_38_1.png)


# Scaling the datasets


```python
## normalization of abv column to in scale of 0 and 1

from sklearn.preprocessing import MinMaxScaler
scaler=MinMaxScaler()


beer_breweries['abv_scale']=scaler.fit_transform(beer_breweries['abv'].values.reshape(-1,1))
beer_breweries['ibu_scale']=scaler.fit_transform(beer_breweries['ibu'].values.reshape(-1,1))
beer_breweries.drop(['abv','ibu'],axis=1,inplace=True)

```


```python
## head of dataset

beer_breweries.head()
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>name_of_beer</th>
      <th>style</th>
      <th>ounces</th>
      <th>name_of_brewery</th>
      <th>city</th>
      <th>state</th>
      <th>abv_scale</th>
      <th>ibu_scale</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>Pub Beer</td>
      <td>American Pale Lager</td>
      <td>12.0</td>
      <td>NorthGate Brewing</td>
      <td>Minneapolis</td>
      <td>MN</td>
      <td>0.385827</td>
      <td>0.288904</td>
    </tr>
    <tr>
      <th>1</th>
      <td>Devil's Cup</td>
      <td>American Pale Ale (APA)</td>
      <td>12.0</td>
      <td>Against the Grain Brewery</td>
      <td>Louisville</td>
      <td>KY</td>
      <td>0.511811</td>
      <td>0.288904</td>
    </tr>
    <tr>
      <th>2</th>
      <td>Rise of the Phoenix</td>
      <td>American IPA</td>
      <td>12.0</td>
      <td>Jack's Abby Craft Lagers</td>
      <td>Framingham</td>
      <td>MA</td>
      <td>0.551181</td>
      <td>0.288904</td>
    </tr>
    <tr>
      <th>3</th>
      <td>Sinister</td>
      <td>American Double / Imperial IPA</td>
      <td>12.0</td>
      <td>Mike Hess Brewing Company</td>
      <td>San Diego</td>
      <td>CA</td>
      <td>0.700787</td>
      <td>0.288904</td>
    </tr>
    <tr>
      <th>4</th>
      <td>Sex and Candy</td>
      <td>American IPA</td>
      <td>12.0</td>
      <td>Fort Point Beer Company</td>
      <td>San Francisco</td>
      <td>CA</td>
      <td>0.582677</td>
      <td>0.288904</td>
    </tr>
  </tbody>
</table>
</div>



# Detecting outliers


```python
sns.boxplot(beer_breweries['abv_scale'])


```




    <matplotlib.axes._subplots.AxesSubplot at 0x2881d0e82c8>




![png](output_43_1.png)



```python
sns.boxplot(beer_breweries['ibu_scale'])
```




    <matplotlib.axes._subplots.AxesSubplot at 0x2881d151cc8>




![png](output_44_1.png)



```python
from scipy.stats import zscore

beer_breweries['ibu_scale_zscore'] = zscore(beer_breweries['ibu_scale'])
beer_breweries['abv_scale_zscore']= zscore(beer_breweries['abv_scale'])

```


```python
beer_breweries_zscore= beer_breweries[(beer_breweries['ibu_scale_zscore'].abs()<=3) &(beer_breweries['abv_scale_zscore'].abs()<=3)]

beer_breweries_zscore.head()


```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>name_of_beer</th>
      <th>style</th>
      <th>ounces</th>
      <th>name_of_brewery</th>
      <th>city</th>
      <th>state</th>
      <th>abv_scale</th>
      <th>ibu_scale</th>
      <th>ibu_scale_zscore</th>
      <th>abv_scale_zscore</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>Pub Beer</td>
      <td>American Pale Lager</td>
      <td>12.0</td>
      <td>NorthGate Brewing</td>
      <td>Minneapolis</td>
      <td>MN</td>
      <td>0.385827</td>
      <td>0.288904</td>
      <td>0.0</td>
      <td>-0.707805</td>
    </tr>
    <tr>
      <th>1</th>
      <td>Devil's Cup</td>
      <td>American Pale Ale (APA)</td>
      <td>12.0</td>
      <td>Against the Grain Brewery</td>
      <td>Louisville</td>
      <td>KY</td>
      <td>0.511811</td>
      <td>0.288904</td>
      <td>0.0</td>
      <td>0.481535</td>
    </tr>
    <tr>
      <th>2</th>
      <td>Rise of the Phoenix</td>
      <td>American IPA</td>
      <td>12.0</td>
      <td>Jack's Abby Craft Lagers</td>
      <td>Framingham</td>
      <td>MA</td>
      <td>0.551181</td>
      <td>0.288904</td>
      <td>0.0</td>
      <td>0.853203</td>
    </tr>
    <tr>
      <th>3</th>
      <td>Sinister</td>
      <td>American Double / Imperial IPA</td>
      <td>12.0</td>
      <td>Mike Hess Brewing Company</td>
      <td>San Diego</td>
      <td>CA</td>
      <td>0.700787</td>
      <td>0.288904</td>
      <td>0.0</td>
      <td>2.265544</td>
    </tr>
    <tr>
      <th>4</th>
      <td>Sex and Candy</td>
      <td>American IPA</td>
      <td>12.0</td>
      <td>Fort Point Beer Company</td>
      <td>San Francisco</td>
      <td>CA</td>
      <td>0.582677</td>
      <td>0.288904</td>
      <td>0.0</td>
      <td>1.150538</td>
    </tr>
  </tbody>
</table>
</div>




```python
beer_breweries_zscore.drop(['ibu_scale_zscore','abv_scale_zscore'],axis=1,inplace=True)

```

    C:\Users\MasterDK-Laptop\anaconda3\lib\site-packages\pandas\core\frame.py:3997: SettingWithCopyWarning: 
    A value is trying to be set on a copy of a slice from a DataFrame
    
    See the caveats in the documentation: https://pandas.pydata.org/pandas-docs/stable/user_guide/indexing.html#returning-a-view-versus-a-copy
      errors=errors,
    


```python
beer_breweries_zscore.head()
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>name_of_beer</th>
      <th>style</th>
      <th>ounces</th>
      <th>name_of_brewery</th>
      <th>city</th>
      <th>state</th>
      <th>abv_scale</th>
      <th>ibu_scale</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>Pub Beer</td>
      <td>American Pale Lager</td>
      <td>12.0</td>
      <td>NorthGate Brewing</td>
      <td>Minneapolis</td>
      <td>MN</td>
      <td>0.385827</td>
      <td>0.288904</td>
    </tr>
    <tr>
      <th>1</th>
      <td>Devil's Cup</td>
      <td>American Pale Ale (APA)</td>
      <td>12.0</td>
      <td>Against the Grain Brewery</td>
      <td>Louisville</td>
      <td>KY</td>
      <td>0.511811</td>
      <td>0.288904</td>
    </tr>
    <tr>
      <th>2</th>
      <td>Rise of the Phoenix</td>
      <td>American IPA</td>
      <td>12.0</td>
      <td>Jack's Abby Craft Lagers</td>
      <td>Framingham</td>
      <td>MA</td>
      <td>0.551181</td>
      <td>0.288904</td>
    </tr>
    <tr>
      <th>3</th>
      <td>Sinister</td>
      <td>American Double / Imperial IPA</td>
      <td>12.0</td>
      <td>Mike Hess Brewing Company</td>
      <td>San Diego</td>
      <td>CA</td>
      <td>0.700787</td>
      <td>0.288904</td>
    </tr>
    <tr>
      <th>4</th>
      <td>Sex and Candy</td>
      <td>American IPA</td>
      <td>12.0</td>
      <td>Fort Point Beer Company</td>
      <td>San Francisco</td>
      <td>CA</td>
      <td>0.582677</td>
      <td>0.288904</td>
    </tr>
  </tbody>
</table>
</div>




```python
## correlation after outlier removal and scaling

beer_breweries_zscore.corr()

```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>ounces</th>
      <th>abv_scale</th>
      <th>ibu_scale</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>ounces</th>
      <td>1.000000</td>
      <td>0.166022</td>
      <td>0.035642</td>
    </tr>
    <tr>
      <th>abv_scale</th>
      <td>0.166022</td>
      <td>1.000000</td>
      <td>0.499503</td>
    </tr>
    <tr>
      <th>ibu_scale</th>
      <td>0.035642</td>
      <td>0.499503</td>
      <td>1.000000</td>
    </tr>
  </tbody>
</table>
</div>



## Building machine Learning Models

Inspiration
Can you predict the beer type from the characteristics provided in the dataset?

What is the most popular beer in North Dakota?

Cheers to beer


```python
## select the dependent and response variables
# beer_breweries_zscore.columns

beer_breweries_feature=beer_breweries_zscore.loc[:,['abv_scale','ibu_scale','ounces','style']]
print(beer_breweries_feature.head())
print("shape of dataset is:" ,beer_breweries_feature.shape)
```

       abv_scale  ibu_scale  ounces                           style
    0   0.385827   0.288904    12.0             American Pale Lager
    1   0.511811   0.288904    12.0         American Pale Ale (APA)
    2   0.551181   0.288904    12.0                    American IPA
    3   0.700787   0.288904    12.0  American Double / Imperial IPA
    4   0.582677   0.288904    12.0                    American IPA
    shape of dataset is: (2379, 4)
    

## Choosing a model

In statistics, multinomial logistic regression is a classification method that generalizes **logistic regression to multiclass problems, i.e. with more than two possible discrete outcomes.**[1] 

That is, it is a model that is used to predict the probabilities of the **different possible outcomes of a categorically distributed dependent variable**, given a **set of 
independent variables (which may be real-valued, binary-valued, categorical-valued, etc.).**

Reference: https://en.wikipedia.org/wiki/Multinomial_logistic_regression

# Training and test creation

Stratification is the process of rearranging the data so as to ensure that each fold is a good representative of the whole.

For example, in a binary classification problem where each class comprises of 50% of the data, it is best to 
arrange the data such that in every fold, each class comprises of about half the instances.

It is generally a better approach when dealing with both bias and variance. A randomly selected fold might not adequately represent the minor class, particularly in cases where there is a huge class imbalance.


```python
# input 
x = beer_breweries_feature.iloc[:, 0:3].values 

# # output 
y = beer_breweries_feature.iloc[:, 3].values

from sklearn.model_selection import train_test_split

xtrain, xtest, ytrain, ytest = train_test_split(x, y, test_size = 0.25, random_state = 0) 
```

# Logistic regression with multinomial classification


```python
from sklearn.linear_model import LogisticRegression 
classifier = LogisticRegression(random_state = 0,multi_class='multinomial') 
classifier.fit(xtrain, ytrain) 
y_pred = classifier.predict(xtest) 
```

    C:\Users\MasterDK-Laptop\anaconda3\lib\site-packages\sklearn\linear_model\_logistic.py:764: ConvergenceWarning: lbfgs failed to converge (status=1):
    STOP: TOTAL NO. of ITERATIONS REACHED LIMIT.
    
    Increase the number of iterations (max_iter) or scale the data as shown in:
        https://scikit-learn.org/stable/modules/preprocessing.html
    Please also refer to the documentation for alternative solver options:
        https://scikit-learn.org/stable/modules/linear_model.html#logistic-regression
      extra_warning_msg=_LOGISTIC_SOLVER_CONVERGENCE_MSG)
    

# Confusion matrix


```python
from sklearn.metrics import confusion_matrix 
cm = confusion_matrix(ytest, y_pred) 
  
print ("Confusion Matrix : \n", cm)

```

    Confusion Matrix : 
     [[0 0 0 ... 0 0 0]
     [0 0 0 ... 0 0 0]
     [0 0 0 ... 0 0 0]
     ...
     [0 0 0 ... 0 0 0]
     [0 0 0 ... 0 0 0]
     [0 0 0 ... 0 0 0]]
    

# Accuracy score


```python
from sklearn.metrics import accuracy_score 
print ("Accuracy : ", accuracy_score(ytest, y_pred)) 

```

    Accuracy :  0.26218487394957984
    
