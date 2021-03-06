---
title       : Stopping Distance Prediction
subtitle    : Developing Data Products Course Project Presentation
author      : ccliuc
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets    : [bootstrap, quiz, shiny, interactive] # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
ext_widgets: {rCharts: [libraries/nvd3]}

--- 
## Introduction
The training data set used in this course project is "cars" in R package. 

```r
data(cars)
par(mar=c(15,4,0,2))
plot(cars, xlab = "Speed (mph)", ylab = "Stopping distance (ft)",las = 1, xlim = c(0, 25))       
```

![plot of chunk unnamed-chunk-1](assets/fig/unnamed-chunk-1.png) 

---

## Instructions
This shiny application builds a polynomial regression model to predict the stopping distance of a car given an input speed.To use the shiny app (https://ccliuc.shinyapps.io/CourseProject/), please follow the steps below.

1. Choose a number from the drop down list on the left side as the degree in the polynominal regression model.

2. Input a speed value.

3. Click the submit button.

After clicking the submit button, the app will predict the stopping distance.

Meanwhile, the prediction curve is shown.

---

## Input interface
![width](assets/img/input.png)
<img src="input.png" alt="input" width="42" height="42">

---

## Output interface
![width](assets/img/output.png)
<img src="output.png" alt="output" width="42" height="42">
