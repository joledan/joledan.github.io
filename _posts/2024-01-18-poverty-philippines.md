---
layout: post
title: >- 
    In due time: the Philippines' journey towards eliminating poverty
thumbnail: "/assets/images/ph-pov/ph-pov-fig2.png"
---

**[code](https://github.com/joledan/ph-poverty) and tools:** R, Python, sf, ggplot2  

The Philippines, an island nation of 113.9 million in Southeast Asia, has laid out a plan to accelerate poverty reduction. By 2028 President Ferdinand Marcos Jr aims to [decrease](https://asia.nikkei.com/Economy/Philippine-poverty-rate-drops-to-22.4-still-far-from-Marcos-target) the national poverty rate to 9% as his presidential term ends. 

<!--more-->
<!--Philippine poverty rates are stubborn, but ambitious plans are on the way-->
In line with the first UN Sustainable Development Goal, the country aims to eradicate extreme poverty, defined as the share of population living below $2.15 a day, by 2030. Compared to China's swift progress or Indonesia and Vietnam's consistent decline, the Philippines is stuck at 3% from 2018 to 2021 (see next chart). A susceptibility to [natural disasters](https://climateknowledgeportal.worldbank.org/country/philippines/vulnerability) and global shocks, coupled with [high inflation](neda.gov.ph/ph-records-lowest-inflation-rate-in-2023-govt-to-continue-measures-to-protect-filipino-purchasing-power-neda/), and a history of conflict has stalled progress in the Philippines. 

<img width="50%" src="{{site.url}}/assets/images/ph-pov/ph-pov-fig1.png"  style="display:block;float:none;margin-left:auto;margin-right:auto;width:60%">

<!-- poverty rate by major island group -->
The Philippines is split into three major island groups from north to south: Luzon, Visayas, and Mindanao. The National Capital Region (NCR) contains the capital Manila and 16 other cities and municipalities. The national poverty rate is [defined](https://psa.gov.ph/statistics/poverty/node/162559) as the share of poor Filipinos whose income per person is insufficient to meet their basic needs. From 2021, the most recent year of data, the [threshold](https://psa.gov.ph/statistics/poverty/node/167972) was set at PhP 12,030 per person ($215 USD) per month. Since 2006, the Philippines' national poverty rate dropped from 26.5% to 18.1% equivalent to around 20 million Filipinos (see next chart). This value exceeds the country's current [target](https://psa.gov.ph/statistics/statdev/press-release) between 15.5 to 17.5%. This was accomplished through various social welfare policies in the form of [cash transfer programs](https://www.officialgazette.gov.ph/programs/conditional-cash-transfer/), community driven development, and improvements to livelihood and [employment opportunities](https://www.lumina.com.ph/news-and-blogs/blogs/social-welfare-programs-in-the-philippines/) for the most vulnerable populations.  

![fig2]({{site.url}}/assets/images/ph-pov/ph-pov-fig2.png)

Poverty rate by major island group follows the reverse pattern from top to bottom: Mindanao records the largest values, followed by Visayas, Luzon, and the NCR. The national poverty rate cuts through the middle leaving the order unchanged over time. 

In the past two decades all three major island groups decreased poverty rates. From 2006 to 2012 progress appeared flat then decreased steadily in the latter half of the 2010s going into 2018. The [impact of the 2020 COVID-19 pandemic](https://www.reuters.com/world/asia-pacific/pandemic-pushed-millions-more-into-poverty-philippines-govt-2022-08-15/) reverted some progress, though importantly not all, resulting in increased rates nationally and in Luzon, Visayas, and the NCR, from 2018 to 2021. Mindanao is the only island group that saw a constant decrease in poverty over the three years of data. However, it still records the highest poverty rate among the major island groups in the country.

<!-- urban/rural poverty -->
The Philippine case suggests poverty is split along geographic and economic lines. Visayas and Mindanao, with predominantly agriculture and fishing-based economies, record higher rates compared to Luzon and the NCR, the economic centre of the country. 

![fig3]({{site.url}}/assets/images/ph-pov/ph-pov-fig3.png)

Three patterns reveal the stark nature of the urban-rural poverty divide across regions in the Philippines (see previous chart). First, rural poverty is higher than urban poverty in 15 out of 16 regions. Regions in Mindanao record some of the largest rural poverty rates in the country which exceed the national value. Second, the majority of urban poverty rates are higher than the national value, including all regions in Visayas and Mindanao. The Bangsamoro Autonomous Region in Muslim Mindanao (BARMM) records the highest urban poverty rate in the country at 37.9%. Finally, the differences in urban and rural poverty in regions of Visayas and Mindanao are relatively large compared to those in Luzon. The difference in rates in 7 out of 9 regions in Visayas and Mindanao are all higher than the largest difference in Luzon (Region V has a 10 percentage point difference). Region IX in Mindanao has the largest difference in urban and rural poverty rates in the country (27 percentage points). 

<!-- conclusion on future plans -->
Disparities in urban and rural poverty suggest a potential starting point for policy makers. The [Philippine Development Plan 2023-2028](https://pdp.neda.gov.ph) outlines the Marcos administration's goals to reduce poverty through economic growth. Importantly it recognizes the multidimensional nature of poverty and the need to approach it from all angles. Better health outcomes for all could lead to more productive workers regardless of geography. Modernizing agriculture and land use practices could decrease rural poverty. Improving road and transport links between urban and rural areas allows for better market access and economic opportunities. Addressing environmental concerns, from improving pollution and air quality in urban areas to building resilient infrastructure in more disaster-prone areas, provides some relief to the most vulnerable. The administration's poverty alleviation agenda is rigorous and ambitious. Better to cover all bases rather than too little.

-----

## Reflections

### Learning when to stop

I went through several iterations of plots showing different poverty rates at different geographic levels, but eventually I had to re-focus and make sure not to get too lost in the data. From this project I learned that changing plans can and should happen but there needs to be a clear stopping point. This reflects my academic background, where I think I need to cover all feasible ideas and sanity checks. 

### You can use Python in R with relative ease

For one part of the data cleaning, I had to match province names across different data sets, that could then be used to create the plots by major island group or region. As part of my regular, every-day work I faced a similar dilemma matching strings from different data sets and decided to use string matching algorithms that were easily accesible in Python. Rather than processing that data in a separate Python script, I used reticulate, a R package which allowed me to call Python from R. I then used Polyfuzz to give me the matched strings. In future projects, I hope to code more in Python (rather than calling from R) so watch this space. 

### Drawing from my background

I studied economics, with a focus on development and poverty, so this topic was a nice re-visit to what I had  learned all those years ago. I don't get to work on development/poverty anymore in my day-to-day life so this was a good exercise to both jog my memory and to learn recent progress in the development/poverty space. I also learned the international poverty line was adjusted from $1.90 a day to $2.15 a day in 2022. 