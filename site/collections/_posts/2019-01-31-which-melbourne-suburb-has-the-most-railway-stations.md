---
id: 1946
title: 'Which Melbourne suburb has the most railway stations?'
date: '2019-01-31T07:00:00+11:00'
author: Philip
layout: post
guid: 'https://philipmallis.com/?p=1946'
categories:
    - Transport
tags:
    - Data
    - Melbourne
    - Trains
---

Melbourne’s 218 railway stations are not always where you expect them to be: Huntingdale Station is in Oakleigh, North Melbourne Station is in West Melbourne and Burwood Station is in Glen Iris.

This then begs the question: which suburb in Melbourne has the most?

[![Westgarth Station at night](https://farm5.staticflickr.com/4801/38907580440_f72a8ab286_z.jpg)](https://www.flickr.com/photos/philipmallis/38907580440/ "Westgarth Station at night")<script async="" charset="utf-8" src="//embedr.flickr.com/assets/client-code.js"></script>

### Method

To answer this question, I extracted data from OpenStreetMap using [Overpass](https://overpass-turbo.eu/). I then loaded this into QGIS to exclude some of the extrated data to remove tourist railways, miniature railways and similar points. I then loaded the [suburb and locality boundaries](https://www.data.vic.gov.au/data/dataset/locality-boundaries-property-polygon-vicmap-admin) from data.vic.gov.au to run a spatial analysis and come up with the results.

### Results

The results of this analysis were quite surprising.

There are only four suburbs in Melbourne that have four or more train stations located within their boundaries. There are two joint winners with a total of five stations each – Northcote and Camberwell.

| Suburb | Number of stations | Stations |
|---|---|---|
| Camberwell | 5 | Camberwell   East Camberwell   Hartwell   Riversdale   Willison |
| Northcote | 5 | Croxton   Dennis   Northcote   Merri   Westgarth |
| Brighton | 4 | Brighton Beach   Gardenvale   Middle Brighton   North Brighton |
| Melbourne (CBD) | 4 | Flagstaff   Flinders Street   Melbourne Central   Parliament |

When Melbourne Metro 1 opens, Melbourne CBD will shoot up to the top of the list. Three of the five new stations (State Library, Town Hall and Anzac) will be located within its boundaries, bringing the total number up to seven.

It could also be argued that Parliament Station is technically located partially in [East Melbourne](https://www.openstreetmap.org/way/458461654) and that Richmond Station is located partially in the [Melbourne CBD](https://www.openstreetmap.org/node/4681252024). This doesn’t change the total number, but if you are pedantic then this could be something to think about.

So if you live in Northcote or Camberwell, consider yourself lucky to have more railway stations than any other suburb!