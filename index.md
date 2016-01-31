---
title       : Understanding the cost of ownership
subtitle    : New or used car 
author      : Vincent Phan
job         : Data Scientist
framework   : io2012       # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides

---

## Are you a trust fund baby? Chances are, you're probably not...

- We all dream of financial stabilities but are we making the right choice when we decide to pull up to an BMW dealer and buy that M3 that have been long sought after?
- Here's a web based application that can probably make you think again.

---
## How much are you actually spending on a new or used car?

1. If you're financing your car, what is your APR?
2. How long do you planned to own your car?
3. What is the out-the-door cost of your car?
4. Is your car a gas gustler? What is the MPG? 
5. What is the current gas prices?
6. How much will your car depreciate?

All of these variables will play an important role in determining your true cost of ownership on your next car.

--- .class #id 

## What's going on behind the application? 
#### User input:
1. Owned or financed? If Financed, APR input will be prompt. There's a function within the application that creates an amortization table. It will then sum up the total interests paid based on total principal, APR and length of loan. 
2. Depreciation is calculated based on 19%, 31%, 42%, 51%, and 60% depreciation over 1, 2, 3, 4, and 5 years, respectively. 
3. Fuel cost is calculated using gas prices per gallon and average of 13,476 miles per year.
 
References:
- Depreciation  
http://www.edmunds.com/car-buying/how-fast-does-my-new-car-lose-value-infographic.html  
- Amortization function by Thomas Girke  
http://faculty.ucr.edu/~tgirke/Documents/R_BioCond/My_R_Scripts/mortgage.R  
- Average miles  
https://www.fhwa.dot.gov/ohim/onh00/bar8.htm  

---

## Give the app a try

#### $33,744.04!

- This is the dollar amount that will come out of your pocket if you finance a $39,800 car at 3.25 APR for 5 years!

#### $36,216.64
- We're lucky that gas prices are record low right now...
- If gas prices goes up to $3.99/gallon, you spend $2472.60 more!

#### What's my point? Buying a car is NOT an investment....

---


```r
publish(user = "Zupervinn", repo="DataProduct_shiny_presentation")
```

```
## Please set mode to selfcontained and run Slidify
```

```
## This would place library files in the slide folder
```

```
## making it self-contained
```

```
## [1] FALSE
```
