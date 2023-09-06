---
layout: post
title: Country name changes over time
thumbnail: "/assets/images/wiki-nc/wiki-nc-fig1.png"
---

**[code](https://github.com/joledan/wiki-country-names) and tools:** R, rvest, ggplot2

<!--more-->

![fig1]({{site.url}}/assets/images/wiki-nc/wiki-nc-fig1.png)

[This Wikipedia article](https://en.wikipedia.org/wiki/Geographical_renaming) contains a (incomplete) list of significant country name changes from the 1500s to present day. Changing names is not an easy task as there are a lot of factors to consider. Does currency need to be reprinted? What about names of established institutions? Rebranding can be costly, but is often done out of necessity. 

Name changes can occur due to countries splitting, such as the dissolution of the Soviet Union in the 1990s or the break-up of Yugoslavia. Renaming is also an act of decolonization: around 31 ex-European colonies changed their names from 1940 to 1980 upon independence. 

The Republic of Türkiye is the latest country to officially change its name, previously known as The Republic of Turkey. Recently, The Republic of India used "Bharat" to refer to itself in dinner invitations to G20 members. Perhaps there will be a new name to remember. 

-----

## Reflections

There are a lot of packages to facilitate scraping in R. This also gave me a chance to brush up on my HTML/XPath skills that I picked up during my studies. Scraping a simple list from Wikipedia was not too challenging; I think the most difficult part of this task was re-structuring and cleaning the text data into a neat and usable format. 