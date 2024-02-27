---
id: 3400
title: 'The most and least punctual bus routes in Melbourne'
date: '2021-07-19T09:00:00+11:00'
author: Philip
layout: post
guid: 'https://philipmallis.com/?p=3400'
header_position:
    - inherit
header_fullwidth:
    - inherit
page_header_styling:
    - inherit
heading_title:
    - '0'
custom_logo:
    - ''
custom_logo_width:
    - ''
custom_menu_skin:
    - default
sticky_menu_on_page:
    - default
custom_sticky_logo:
    - ''
sticky_menu_skin:
    - default
section_logo_switch:
    - '0'
footer_visibility:
    - inherit
fixed_footer:
    - inherit
footer_fullwidth:
    - inherit
custom_grid_container_width:
    - '0'
breadcrumb:
    - inherit
featured_image_placing:
    - hide
post_image_size:
    - inherit
page_custom_css:
    - ''
auto_update_uri:
    - '1'
image: /wp-content/uploads/2021/07/50284007992_e0c8320790_c.jpg
categories:
    - Transport
tags:
    - 'Bus data'
    - Data
---

*See the data [here](https://app.powerbi.com/view?r=eyJrIjoiMzE2ZDIyN2YtODY1Yy00ZGY0LWE4YTktNDcxOTcwYWQyMjM5IiwidCI6IjcyMmVhMGJlLTNlMWMtNGIxMS1hZDZmLTk0MDFkNjg1NmUyNCJ9).*

On [Friday last week](https://www.premier.vic.gov.au/new-public-data-reveals-high-performing-bus-network), the Department of Transport added metropolitan bus performance data to its monthly public transport reporting. This is exciting news as it was not previously publicly available.

<figure class="wp-block-image size-full is-resized">![](https://philipmallis.com/wp-content/uploads/2021/07/50284007992_e0c8320790_c.jpg)</figure>The data is not very easy to find.

To get there, you have to visit ptv.vic.gov.au, scroll to the bottom of the page, click on ‘Data and Reporting’, click on ‘[Monthly performance](https://www.ptv.vic.gov.au/footer/data-and-reporting/network-performance/monthly-performance/)‘ and then scroll to nearly the bottom of the page to find a link buried in some text: “For detailed punctuality, reliability, and services monitored[<sup>*(1)*</sup>](https://www.ptv.vic.gov.au/footer/data-and-reporting/network-performance/monthly-performance/#ServicesMonitored) information, [see our Power BI App](https://app.powerbi.com/view?r=eyJrIjoiMzE2ZDIyN2YtODY1Yy00ZGY0LWE4YTktNDcxOTcwYWQyMjM5IiwidCI6IjcyMmVhMGJlLTNlMWMtNGIxMS1hZDZmLTk0MDFkNjg1NmUyNCJ9)“

There is a lot of information to digest in this Power BI table. Unfortunately, it’s not available to download, so the general public are quite limited in the type and scope of analysis that is practically possible. It is also only available back to July 2017.

Despite these constraints, we can still pull out some interesting findings.

#### COVID-19 has significantly improved average (mean) bus punctuality

In 2019, mean bus punctuality across the network was 86.8%. In 2020, this shot up by more than eight per cent to 92.9%.

<figure class="wp-block-image size-large">![](https://philipmallis.com/wp-content/uploads/2021/07/buspatronage.png)</figure>- - - - - -

This was likely due to the [significant decrease](https://chartingtransport.com/2020/05/03/what-impact-has-the-2020-covid-19-pandemic-had-on-road-traffic-volumes-in-victoria/ "https://chartingtransport.com/2020/05/03/what-impact-has-the-2020-covid-19-pandemic-had-on-road-traffic-volumes-in-victoria/") in motor vehicle traffic across Melbourne and Victoria throughout most of 2020 due to lockdown restrictions on movement. Less road traffic means fewer delays to buses caused by motor vehicles (crashes, congestion, etc.)

Lower passenger numbers may have also played a part. This may have been by reducing the number of stops that buses needed to make and speeding up journey times.

#### Buses are most punctual in January and least punctual in March

Under non-COVID conditions (looking at 2018-2019 data), mean bus punctuality across the network varied quite considerably between months.

Moreover, if you look at it month-by-month, January had the highest percentage of on-time services. March had the lowest percentage of on-time services, closely followed by February.

This is probably the impact of school holidays and the resulting decrease in motor vehicle traffic that usually causes delays to bus services.

#### The best-performing bus routes tend to be very short and / or infrequent

Unfortunately I can’t link route length data to punctuality information as the Power BI tables cannot be downloaded. So this is more off my general observations rather than many hard stats.

You can sort routes by punctuality, and it seems that those that perform the best are those with short routes or infrequent service patterns.

<figure class="wp-block-table is-style-stripes">| Route | % On Time (July 2017 – June 2021) | 2018-19 Patronage |
|---|---|---|
| 444 | 99.8% | N/A |
| 786 | 98.8% | 2,630 |
| 489 | 98.5% | 85,348 |
| 550 | 98.5% | 58,054 |
| 486 | 98.4% | 137,572 |
| 673 | 98.3% | 3,768 |
| 487 | 97.8% | 67,063 |
| 570 | 97.8% | 202,371 |
| 696 | 97.8% | 2,231 |
| 454 | 97.7% | N/A |

</figure>- - - - - -

The most punctual bus route, the 444, [is a new one](https://web.archive.org/web/20200320084725/https://www.premier.vic.gov.au/bus-boost-for-melton-rockbank-and-the-growing-west/), having only commenced services in November 2019. It also travels only a short distance from Rockbank Station into the Aintree Estate with only eight stops.

Most of the rest have been around for quite a while longer but they all fall into one of the two categories mentioned earlier. The [786](https://www.ptv.vic.gov.au/route/timetable/4663/786-rye-to-st-andrews-beach/#RoutePage:::datetime=2021-07-18T23%3A20%3A00.000Z&direction_id=251&stop_id=-1&_auth=80619c3452fbe9ea11c487e2602aa8fef1a115ef6cd6c591dcc887fd57eaee1c), for example, only operates six services on weekdays plus three on Saturdays and carries a [tiny number of passengers](https://philipmallis.com/blog/2020/02/28/melbourne-bus-route-patronage-data-for-2008-2019/) (2,630 in 2018-19), while the 696 (running from Olinda to Monbulk) only carried 2,231 passengers in 2018-19 along its nine stops.

Three of the top ten (489, 486 and 487) operate in Sunbury and are presumably less likely to be affected by motor vehicle delays due to the lower levels of traffic.

The [570](https://www.ptv.vic.gov.au/route/11118/570-thomastown-rmit-bundoora/) is an interesting one. My two thoughts on this are that it is a relatively short route and also passes directly past the Dyson’s bus depot in Bundoora, making it very quick and easy for buses to start or end their trips. If you have any other theories or ideas as to why this comes up as the eighth most-punctual bus route in Melbourne, please let me know in the comments below.

<figure class="wp-block-table is-style-stripes">| Route | % On Time (July 2017 – June 2021) | 2018-19 Patronage |
|---|---|---|
| 606 | 69.1% | 128,113 |
| 182 | 70.9% | N/A |
| 417 | 72.4% | 34,567 |
| 219 | 73.8% | 335,909 |
| 538 | 74.8% | 38,533 |
| 546 | 75.4% | 206,071 |
| 693 | 76.8% | 438,186 |
| 795 | 77.2% | 13,673 |
| 350 | 77.7% | 199,586 |
| 232 | 79.2% | 180,196 |
| 303 | 79.2% | 68,530 |

</figure>- - - - - -

The top 10 least punctual routes are a bit more of a mixed bag. It includes a new route (182, which hasn’t been operating for even six months yet) and some old, well-established routes like the 219.

It’s less clear to me why these particular routes are in the top 10, other than they all have significant lengths of their route on roads that get quite congested. Again if you have any ideas, please let me know in the comments.

- - - - - -

It’s important to remember how this data is compiled and presented. There are a lot of qualifications. For example, ‘on time’ is defined by DoT for buses as: *“Number of services arriving no more than 4 minutes and 59 seconds late and departing no more than 59 seconds early at timing points.”*

There is more information on this in the first three tabs of the Power BI dashboard if you are interested.

I’ve barely scratched the surface for the potential of this great dataset. For example, I would love to link this data to others that include bus patronage, route length and number of stops to cross-tabulate and analyse this information. But as I mentioned above, this is impossible unless the data is able to be downloaded in a machine-readable format (at least as far as I’m aware).

I may come back to this topic soon after I’ve had some more time to dig around and cross-reference to related datasets. I’m sure others will also be doing the same.