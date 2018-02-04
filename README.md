# PatternRecognitionForFX
TLDR; Don't use this and ignore the project.

Side-project that I was playing around on my free time. The end product was below expectations and I would not recommend using/investing. Code is too slow to find a pattern with 60% (or above) similarity, and the model is too simplistic to invest more time in speeding it up with Cython/MutliProcessing. 

Core idea was to use tick-by-tick data and treat them as seperate time series (rolling window), 
find the %change between each tick and 
compare the similarity of the %change between the two time series. 
The assumption being, if the two time series have the same %change per tick, we can assume the next tick will be (CurrentPrice*%ChangeOfSimilarTimeSeries). 
