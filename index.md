---
layout: home
title: Beer Reviews
subtitle: Location of Brewery
cover-img: "/assets/img/beer.jpg"
---

## Motivation

&nbsp;&nbsp;&nbsp;&nbsp; Breweries are becoming more and more popular nowadays, each of them proposing beers with unique flavors. Appreciated by casual beer drinkers and craft beer enthusiasts, beers happen to be a thriving market. A rising amount of new breweries have emerged in the last decades. When starting a new brewery, the choice of location of the brewery is a significant step to guarantee its success.  

&nbsp;&nbsp;&nbsp;&nbsp; There are several factors to consider when choosing a location for a brewery such as the access to raw materials (water, hops, barley, and yeast), the proximity to customers, zoning laws and regulations, costs of renting or buying property, and competition with other breweries.  

## Goal

&nbsp;&nbsp;&nbsp;&nbsp; Throughout this project, we will try to give some tools for brewers to help them to choose the location of their future brewery by answering some research questions.

## Research questions

&nbsp;&nbsp;&nbsp;&nbsp; Is a brewery inside a city more inclined to be successful?

&nbsp;&nbsp;&nbsp;&nbsp; Which regions are more conducive to which style of beer?

## Methodology

&nbsp;&nbsp;&nbsp;&nbsp; We used a dataset on beer reviews provided by RateBeer website which collected over 7 millions reviews for a period of 17 years (2001-2017). It includes :
- metadata about 442k beers, 24k breweries, and 70k users
- ratings across different aspects: appearance, aroma, palate, taste
- textual review

&nbsp;&nbsp;&nbsp;&nbsp; Heatmap of reviews

<div class="flourish-embed flourish-heatmap" data-src="visualisation/12245524"><script src="https://public.flourish.studio/resources/embed.js"></script></div>

&nbsp;&nbsp;&nbsp;&nbsp; Basic analysis on those datas shows the different appreciations on beer styles. The most prefered one is imperial stout with a mean rating of 3,85. The less prefered one is malt liquor with a mean rating of 1,92.

<div class="flourish-embed flourish-chart" data-src="visualisation/12232997"><script src="https://public.flourish.studio/resources/embed.js"></script></div>

&nbsp;&nbsp;&nbsp;&nbsp; For further analysis, we needed to obtain precise location of breweries with API queries. 

## Expliquer combien ont été discard car mal placés montrer clusters par ville, combien de brasseries classifiées en ville et hors de villes? etc… 
&nbsp;&nbsp;&nbsp;&nbsp; Using the google API queries, not all breweries locations could be found. In a first step, all breweries where no location where found have been discarded, i.e., (2555 breweries). After that step, the breweries that were classified in the wrong country where also removed (XXX breweries) and we considered that the rest of the breweries where correctly classified. Then, using a shapefile that had the major cities in the world (i.e XXX cities), it was possible to extract which breweries where inside of a city and which breweries where outside of a city. Thiss resulted in XXX breweries in the city and XXX breweries outside of the city.



### Boxplot rating comparison ville/campagne



### carte de densité brasseries

### Linear-regression rating ville/campagne en fonction de la distance
![ Image description ](./images/Correlation_city_center_rating.png){:style="display: block; margin-left: auto; margin-right: auto;" width="200"}
<center><i>Figure: example</i></center>

The correlation is clearly low, as moving one kilometer away from the city center changes the rating of the brewery of 0.001, which is equal to a change of 0.1 per 100km of distance from the closest city center. The city considered are often pretty big, which can results in a large distance from the city center even for breweries located inside the cities. The average distance from the nearest city center for rural and urban breweries is **45.27km** and **10.13km** respectively, which is not that a big difference. 


### Barplot nombre de reviews par location user pour montrer confounder

### carte de munich avec cercles d'éloignements
### linear regression sur Munich

