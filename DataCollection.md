Data sets
================
05 Juli, 2016

-   [ggplot2movies](#ggplot2movies)
-   [ggplot2::mpg](#ggplot2mpg)
-   [ggplot2::txhousing](#ggplot2txhousing)
-   [nycflights13](#nycflights13)
-   [University of Texas: Inequality
    Project](#university-of-texas-inequality-project)

This is a collection of both "real" and example data useful for the
illustration of different aspects related to data science (e.g.
visualization, modeling or statistical thinking in general).

------------------------------------------------------------------------

ggplot2movies
-------------

**Description**: Information and user ratings on 58'788 movies from
<http://.IMDB.com>. The data set contains all movies until 2005 that had
at least one vote. There are 24 variables:

1.  `title`: Title of the movie
2.  `year`: Year the movie was released
3.  `length`: Length in minutes
4.  `budget`: Total movie budget in US dollars
5.  `rating`: Average IMDB user rating
6.  `votes`: Number of IMDB users who rated the movie
7.  `r1-r10`: If multiplied by 10 the variables `r1` to `r10` give the
    percentiles of users who rated the movie with 1 star (worst
    possible rating)
8.  `mpaa`: Movie rating by the Motion Picture Association of America
    (MPAA), an association representing the six biggest Hollywood
    studios
9.  `Action-Short`: Seven dummies indicating the movie genre. Variable
    names are: Action, Animation, Comedy, Drama, Documentary,
    Romance, Short.

**Most useful for**: Cross-sectional analysis, visualization, modeling  
**Version info**: Version `0.0.1` of the `ggplot2movies` package as of
December 2015.  
**How to get it**:  
+ In R:

``` r
install.packages("ggplot2movies")
library(ggplot2movies)
data("movies")
```

------------------------------------------------------------------------

ggplot2::mpg
------------

**Description**: The dataset contains a subset of the fuel economy data
that the Environmental Protection Agency (EPA) makes available on
<http://fueleconomy.gov>. It contains only models which had a new
release every year between 1999 and 2008, resulting in 234 observation
on 38 unique models of car. There are 11 variables:

1.  `manufacturer`: Name of the company that produced the car
2.  `model`: Name of the model
3.  `displ`: Engine displacement in liters
4.  `year`: Year the car was released
5.  `cyl`: Number of cylinders
6.  `trans`: Type of transmission.
7.  `drv`: Drivetrain. Possible values: f=front wheel, r=rear wheel,
    4=four wheel
8.  `cty`: Miles per gallon (mpg) for city driving
9.  `hwy`: Miles per gallon (mpg) for highway driving
10. `fl`: Fuel type: Possible values: c=CNG, d=diesel, e=ethanol E85,
    p=premium, r=regular
11. `class`: Class or type of car. Possible values: compact, subcompact,
    midsize, minivan, pickup, suv, 2seater

**Most useful for**: Visualization, simple modeling.  
**Version info**: dataset as contained in ggplot2 version `2.0.0`
(December 2015).  
**How to get it**:  
+ In R:

``` r
install.packages("ggplot2")
library(ggplot2)
data("mpg")
```

------------------------------------------------------------------------

ggplot2::txhousing
------------------

**Description**: Information about the housing market in Texas provided
by the [real estate center of the Texas A&M University
(TAMU)](http://recenter.tamu.edu/). Data on all variables was collected
on a monthly basis from January 2000 to July 2015 with 187 observations
for each of the 46 Texan cities within the dataset, totaling the number
of observations to 8602. There are 9 variables:

1.  `city`: Name of the city/ares according to the multiple listing
    service (MLS) classification
2.  `year`: Year observation was made
3.  `month`: Month observation was made
4.  `sales`: Total number of housing sales
5.  `volume`: Total volume of the sales
6.  `median`: Median sales price
7.  `listings`: Total active listings
8.  `inventory`: Number of month it would take to sell the current
    listings at the current pace of sales.
9.  `date`: Date observation was made as a combination of `year` and
    `month` where each month is a twelfth.

**Most useful for**: Time-series analysis, seasonal trends,
visualization, modeling.  
**Version info**: dataset as contained in ggplot2 version `2.0.0`
(December 2015).  
**How to get it**:  
+ In R:

``` r
install.packages("ggplot2")
library(ggplot2)
data("txhousing")
```

------------------------------------------------------------------------

nycflights13
------------

**Description**: The main data set `flights` contains Information about
all flights that departed from NYC (e.g. EWR, JFK and LGA) in 2013. This
amounts to a total of 336,776 flights. To help understand what causes
delays, it also includes a number of other useful datasets such as

-   `weather` : hourly meterological data for LGA, JFK and EWR.
-   `airlines`: airline names and carrier codes
-   `airports`: airport metadata such location and timezone
-   `planes` : plane metadata such as speed, model etc.

**Most useful for**: Visualization, modeling, seasonal trends,
time-series and cross-sectional regression.  
**Version info**: version `0.0.1`  
**How to get it**:  
+ In R:

``` r
install.packages("nycflights13")
library(nycflights13)
data("flights"); data("planes"); data("airlines"); data("airports"); data("weather")
```

------------------------------------------------------------------------

University of Texas: Inequality Project
---------------------------------------

**Description**: The University of Texas Inequality Project (UTIP)
produces data sets on pay inequality at the global level, at the
national level including for Argentina, Brazil, Cuba, China, India, and
Russia, and at the regional level for Europe. They have also used pay
inequality as an instrument to estimate measures of household income
inequality, for a large panel of countries from 1963 through 1999. As
the ISO3 country codes are given, The data sets can easily be joined
with other country data. A detailed description can be found on [UTIP's
website](http://utip.lbj.utexas.edu/default.html). For a peak at what
can be done with one of their data sets see for example:
<http://ellisp.github.io/blog/2016/06/30/ehii>

**Most useful for**: Visualization, modeling, time-series and
cross-sectional regression.  
**Version info**: last accessed: 05.07.2016  
**How to get it**: Go to: <http://utip.lbj.utexas.edu/data.html>
