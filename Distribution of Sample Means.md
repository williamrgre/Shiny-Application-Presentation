Distribution of Sample Means
========================================================
author: WIlliam Green
date: December 6, 2016
autosize: true

INTRODUCTION
========================================================

  This shiny pitch is intended to illustrate the Central Limit Thoerem (CLT) in Coursera's Developing Data Products module.
  
  My approach to App creation:
  
The central limit theorem states that the distribution of the sum (or average) of a large number of independent, identically distributed variables will be approximately normal, regardless of the underlying distribution.


DISTRIBUTION OF RANDOM VARIABLES
========================================================

- Building on this idea I have considered many different types 
   - Normal
   - Uniform
   - Log-normal
   - Espontential
   
SHINY APP
========================================================

My Shiny app can be found here:

https://dskswu.shinyapps.io/Distribution/

My GitHub reprository can be found here: 

https://github.com/williamrgre/Shiny-Application-Presentation



EXAMPLE DISTRIBUTION 1 
========================================================


```r
library(ggplot2)
set.seed(1234)
dat <- data.frame(cond = factor(rep(c("A","B"), each=200)), 
                   rating = c(rnorm(200),rnorm(200, mean=.8)))
# View first few rows
head(dat)
```

```
  cond     rating
1    A -1.2070657
2    A  0.2774292
3    A  1.0844412
4    A -2.3456977
5    A  0.4291247
6    A  0.5060559
```

SLIDE EXAMPLE DISTROBUTION GGPLOT
========================================================

![plot of chunk unnamed-chunk-2](Distribution of Sample Means-figure/unnamed-chunk-2-1.png)
