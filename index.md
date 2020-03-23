---
layout: default
description: We give scientific answers to social distance strategies for the COVID-19 pandemic.
image: /assets/images/best_strategy.png
---

<br>

# Effectiveness of social distance strategies for protecting a community from a pandemic with a data-driven contact network based on census and real-world mobility data

<br>

Authors: David Martín-Corral (1,4), Alberto Aleta (2,3), Yamir Moreno (2,3), Esteban Moro (1,5).
 
(1) University Carlos III de Madrid, Leganés, Spain.

(2) University of Zaragoza, Zaragoza, Spain.

(3) ISI Foundation, Turin, Italy.

(4) Zensei Technologies S.L., Madrid, Spain.

(5) MIT Media Lab, Cambridge, US.

**Notice:** This results are preliminary and they have not yet been peer-reviewed. We will be updating them with new results and analysis. This work is licensed under a Creative Commons Attribution 4.0 International License. 

A extended version of this report can be downloaded [here](/assets/pdfs/2020-03-22_Preliminary_Report_Effectiveness_of_social_distance_strategies_COVID-19.pdf).

<br>

## Key findings

  1. **School closures do not have a major impact on controlling the epidemic**, despite closing them infections keep occurring within the households and the community layers.

  2. **Passive social distance strategies are not enough to contain the epidemic**, active strategies need to be established. For instance, large scale testing, remote symptoms monitoring, isolation and contact tracing.

  3. **School closures and Self distancing at 90% of adoption is a feasible strategy for minimizing the effects of the epidemic**, but only if they are applied for a large period of time.

  4. If high resolution mobility data is available, **our data-driven approach with real world data can ingest new cities or countries quite easily** to measure the evolution of social distance strategies and the epidemic.

<br>

## Background

Current situation of emergency is global. In less than three months of social distance strategies that they started to be in place, there are more than 23 countries with more than 1.000 infected cases by COVID-19. Each of them with different mitigation and suppression strategies that use social distance tactics. 

The results of this variance in strategies is that the balance of infected cases and deaths by country are different, putting millions of people at risk of death or saving millions of lives. 

Our report has preliminary results that try to respond to the following answers to the COVID-19 epidemic and the mitigation strategies based on social distance:

* What is the impact of current social distance strategies over the epidemic? 

* For how long do they need to be in place? How many people will be infected? Who has been infected? 

* How do R(t) and the epidemic dynamic change based on adding strategies? 

* What is the probability of having a second outbreak? 

* If so, How much time do we have to get ready? How long should we wait to have x% of the population infected? 

* Which is the best strategy to minimize the current epidemic and get ready for a second outbreak?

We test a set of six passive social distance strategies and what if cases to respond previous questions.

## Data

We used detailed mobility data and sociodemographic data from the Boston area, from CubeIQ and US Census, respectively. 

We use it to generate one network describing the contact patterns of about 80.000 agents in the Boston area during a period of four months and three layers (Community, Households and Schools).

The community layer is based on mobility data, the households layer is built from census data for generating children and parents or people living alone come from the individuals present in the community, and finally, the school layer is based on children from households. 

Probabilities of contact are based on the time of two individuals being in the same place.

![Best social distance strategy](/assets/images/boston_population.png)

In the previous chart we can see the distribution of adults and children in the population by US Census block groups in the Boston area. The Adult population comes from real world mobility data and children are synthetically generated with the help of the US Census data about Household type by size and Family type by presence of children under 18 years.


## Data-driven epidemic models

### Calibrating layer weights using historical ILI data and a SIR model

Initially, the weight of each link measures a different quantity. Links in households and schools have a weight equal to 1. 

Conversely, links in the community layer are a measure of time, since it is the product of the fraction of time that individuals i and j have been in the same place

### SEIR model for modelling the COVID-19 epidemic

With the values obtained in the previous model, we can weight each link by their relative importance in the propagation of a disease that is transmitted by droplets, such as influenza or covid-19. The next step is to modify the previous model to include the special characteristics of this new disease.

## Social distance startegies

We explore different social distance strategies:

(i) School closures.

(ii) Self-distancing and remote work.

(iii) Self-distancing and remote work plus School closure.

(iv) Restaurants, nightlife and cultural closures.

(v) Non-essential workplace closures.

(vi) Total confinement.

We test the impact of establishing these strategies at different stages of the epidemic curve and for different periods of time.

## Best strategy for minimizing the impact of COVID-19 epidemic

The best strategy based on our study is to appy a social distance of 90% of adoption within the population and school closures. We think that is a feasible strategy that can buy time to get ready for more active suppression strategies, such as massive testing, remote symptoms monitoring, isolation of new cases and contact tracing.

In the following chart, we can see the dynamic of the epidemic if the propose strategy is established.

![Best social distance strategy](/assets/images/best_strategy.svg)

The best strategy based on our study is to appy a social distance of 90% of adoption within the population and school closures. We think that is a feasible strategy that can buy time to get ready for more active suppression strategies, such as massive testing, remote symptoms monitoring, isolation of new cases and contact tracing.

**1) Epidemic trajectory:** We can see that the epidemic trajectory keeps at minimum while the strategy endures. That give us time for getting ready and control the second wave with a well defined suppression strategy.

**2) Total cases:** We can see that the duration of the social distance measures delay the growth of cumulative cases the time of the measures plus 30 days.

**3) Effective reproduction number:** We see that the strategy can reduce the effective reproduction number below 1 to contain the exponetial growth of the epidemic. However, when social distance measures are withdrawn the reproductive number grows exponentially.

**4) New infections by layer:** We see similar epidemic dynamics between 30 and 90 days, the duration of the measures just keep stable the proportion of new infections by layer while the measures are in place.

**5) Case distribution by layer:** Finally, the main proportion of cases take place in the community and workplaces, nearly a 50% of them. Then households are the second place where people are infected. And finally, schools. We do not see differences in the distribution of cases with duration of the measures.

A extended version of this report can be downloaded [here](/assets/pdfs/2020-03-22_Preliminary_Report_Effectiveness_of_social_distance_strategies_COVID-19.pdf).

## Data Protection

This research was solely based on data from anonymized users who have opted-in to provide access to their location data anonymously, through a GDPR-compliant framework. The analysis never singled out identifiable individuals and no attempts were made to link these data to third party data about an individual. 

In order to preserve privacy, residential areas are inferred at an aggregated US Census block group, thereby allowing for demographic analysis while obfuscating the true home location of anonymous users and prohibiting misuse of data.

## Acknoledgements and Partnerships

This preliminary analysis is a collaboration between the [University Carlos III de Madrid](), [University of Zaragoza](https://www.unizar.es/), [MIT Media Lab](https://www.media.mit.edu/people/emoro/overview/), [ISI Foundation](https://www.isi.it/en/home), [CubeIQ Inc](https://www.cuebiq.com/). and [Zensei Technologies S.L.](https://zenseiapp.com). In response to the COVID-19 crisis, [Cuebiq is providing insights to academic and humanitarian groups through a multi-stakeholder data collaborative](https://www.cuebiq.com/about/data-for-good/) for timely and ethical analysis of aggregate human mobility patterns.

  



