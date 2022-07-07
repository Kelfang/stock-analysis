# Stock Analysis


## Overview

The purpose of this project is to optimize the VBA code used to analyze stock market data so that it can easily evaluate thousands of stocks over the span of several years.


### Background

In this analysis we collected specific stock information on 12 “green stock” companies during 2017 and 2018. The purpose of this initial analysis was to evaluate whether they were worthwhile investments. The original code was well suited to the small dataset that we were working with but the desire to expand beyond these companies warranted another look at the code to increase efficiency.


## Results

#### Original Code

In the images below, you'll see the original code used two loops in its execution. In addition, the original data outputs performed in just over 0.5 seconds for both 2017 and 2018.

![Original VBA Code](https://github.com/Kelfang/stock-analysis/blob/main/Resources/Original_Code.png)

![Original Code RunTime 2017](https://github.com/Kelfang/stock-analysis/blob/main/Resources/Original_Code_runtime_2017.png)

![Original Code RunTime 2018](https://github.com/Kelfang/stock-analysis/blob/main/Resources/Original_Code_runtime_2018.png)


#### Refactored Code

In the images below, the refactored code allowed me to assign the values of the tickerVolume, tickerStartingPrices and tickerEndingPrices at once rather than looping through the data multiple times. Due to this rewrite, the refactored code performed about 80% faster, clocking in around 0.11 seconds.

![Refactored VBA Code](https://github.com/Kelfang/stock-analysis/blob/main/Resources/Refactored_Code.png)

![Refactored Code RunTime 2017](https://github.com/Kelfang/stock-analysis/blob/main/Resources/Refactored_Code_runtime_2017.png)

![Refactored Code RunTime 2018](https://github.com/Kelfang/stock-analysis/blob/main/Resources/Refactored_Code_runtime_2018.png)


## Summary

### Advantages and Disadvantages of Refactoring Code

  #### Advantages
  
  As showcased in this analysis, speed of data output is often a top advantage. It also allows for other optimizations, such as reducing redundancies (for example, duplicated subroutines), debugging for possible errors, and it can produce cleaner code that is easier to understand.

  #### Disadvantages
  
  Some of the advantages can also be disadvantages. If multiple people are touching the code, it can be difficult to understand what it’s doing to improve upon it. Assuming that the original code isn’t broke, refactoring could introduce bugs or cause breaks elsewhere that aren’t fully contemplated. It can cost time and money, often refactoring can be more time consuming than starting from scratch. 
  
### Advantages and Disadvantages of the original and refactored VBA script

  #### Advantages
  
  As illustrated in the images above, speed was a notable advantage with this data. This refactor will have even more impact as it’s used with larger datasets in the future. 
  
  #### Disadvantages
  
  The initial code has more steps outlined and, therefore, it may be easier to follow for someone who did not write it. Since the original code was performing as expected the ROI of time and money may not be worth the rewrite.


  

  
