### Sam Tybout
I'm a second-year MS student in the Geology department. I am from State College, Pennsylvania and got my Bachelor's degree at the University of Rochester. My skills include:
* _keepin' it real_
* _kickin' it old school_
* _getting totally extreme to the max_

#### My Research
I use the fossil record to study patterns of species diversification and extinction in bivalve mollusks. My data comes from the [paleobiology database](https://paleobiodb.org/#/), and most the analysis is run in R, so I'd like to make everything available from a centralized source like Github. Here's a snippet of code that I wrote:
```R
ml_vol = function(series, processed = TRUE){
  if(!processed){
    series = process_series(series)
  }
  n_events = length(series$t)
  size = series_size(series, processed)
  return(n_events / size)
}
```
