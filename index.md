CO2Hawaii dataset from Stat2Data R package
========================================================
author: María Cristina Sánchez Iglesias
date: March, 2021
autosize: true
font-import: "https://fonts.googleapis.com/css2?family=Raleway:wght@300&display=swap"
font-family: 'Raleway'
css: custom.css



Master in Statistics for Data Science - UC3M

Course: Data Tidying and Reporting

About CO2Hawaii dataset
========================================================
incremental:true

CO2Hawaii dataset contains information about monthly carbon dioxide readings at Mauna Loa, Hawaii from January, 1988 to December, 2017

The variables that compound "CO2Hawaii" dataset are:

- Year
- Month
- CO2: Atmospheric carbon dioxide level in ppm
- t: Time interval, with values from 1 to 360 (the number of available values)

It has been collected from the ESRL/GMD data page at <span style="font-weight: bold; text-decoration-line: underline"> <https://www.esrl.noaa.gov/gmd/ccgg/trends/data.html></span>

Data structure
========================================================


```r
library(Stat2Data)
data(CO2Hawaii)
data=CO2Hawaii
head(data)
```

```
  Year Month    CO2 t
1 1988     1 350.39 1
2 1988     2 351.64 2
3 1988     3 352.41 3
4 1988     4 353.69 4
5 1988     5 354.21 5
6 1988     6 353.72 6
```


Concentration over time
========================================================
type: exclaim

![plot of chunk unnamed-chunk-2](index-figure/unnamed-chunk-2-1.png)

<div class="p_iframe">
<iframe frameborder="0" seamless='seamless' scrolling=no src="time_serie.html"></iframe>
</div>



Average concentration per year
========================================================


<style>
  .p_iframe iframe {
    width:75%;
    height:576px;
}
</style>

<div class="p_iframe">
<iframe frameborder="0" seamless='seamless' scrolling=no src="plotly.html"></iframe>
</div>


Average concentration per month
========================================================



<div class="p_iframe">
<iframe frameborder="0" seamless='seamless' scrolling=no src="plotly_mean.html"></iframe>
</div>



