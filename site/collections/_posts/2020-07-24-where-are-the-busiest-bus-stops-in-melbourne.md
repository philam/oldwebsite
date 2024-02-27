---
id: 2770
title: 'Where are the busiest bus stops in Melbourne?'
date: '2020-07-24T12:36:09+11:00'
author: Philip
layout: post
guid: 'https://philipmallis.com/?p=2770'
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
featured_image_placing:
    - default
post_image_size:
    - inherit
page_custom_css:
    - ''
slide_template:
    - default
rs_page_bg_color:
    - '#ffffff'
categories:
    - Transport
tags:
    - 'Bus data'
---

***Update 3:25pm 24/07/2020:** It’s been brought to my attention that some of the figures below are incorrect due to an error with amalgamating patronage data from multiple stops. I’m working to fix it ASAP and will update here again once it’s complete.*

***Update 7:45pm 24/07/2020:** I’ve tried several programs and techniques but nothing seems to work adequately. If anyone has any ideas, please let me know in the comments below or [contact me directly](https://philipmallis.com/about/ "About"). The basic problem is that if I cast the geofence wider, it catches stops that aren’t related to each other. If I use stop names to join stops instead, it also catches stops that shouldn’t be grouped. For now, **please assume that the numbers below are rough guides only and almost certainly exclude some nearby stops**.*

Last year I obtained bus stop patronage data for 2018-19 from the Department of Transport and displayed it on [this interactive map](https://maps.philipmallis.com/victorian-bus-stop-patronage/).

We’ve [already briefly looked](https://twitter.com/philipmallis/status/1240157985931808768 "https://twitter.com/philipmallis/status/1240157985931808768") at the least used bus stops in this dataset, with 2,044 recording one or fewer average daily boardings.

But where are the busiest?

[![Bus running 782 to Balnarring at Frankston Station bus interchange](https://live.staticflickr.com/65535/50094964438_9e5233ce81_z.jpg)](https://www.flickr.com/photos/philipmallis/50094964438/ "Bus running 782 to Balnarring at Frankston Station bus interchange")<script async="" charset="utf-8" src="//embedr.flickr.com/assets/client-code.js"></script>- - - - - -

Before we can answer that, a quick word about the data.

DoT record each bus stop as a separate point on a map rather than grouping them by location or name.

For example, each bay at Chadstone Shopping Centre is mapped as a separate point even though they are all within the same interchange and have the same destination. You can see the result of this on Google Maps which uses a feed from the same GTFS dataset.

<iframe allowfullscreen="" aria-hidden="false" frameborder="0" height="450" loading="lazy" src="https://www.google.com/maps/embed?pb=!1m14!1m12!1m3!1d468.0747797427934!2d145.08356315815843!3d-37.8879098900762!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!5e0!3m2!1sen!2sau!4v1595548954305!5m2!1sen!2sau" style="border:0;" tabindex="0" width="600"></iframe>- - - - - -

So to get a decent answer to this question we have to group like stops together.

For the purposes of the map above, I did this based on name and a geofence around the central point of the interchange. It’s probably not perfect but I think good enough for this project. **As noted in the update above, after I wrote this post it’s been pointed out to me that the numbers below are quite a bit off. So please take these results with a grain of salt until a solution can be found.**

To start with, let’s see which stops have 1,000 or more average boardings per day.

<div class="tableauPlaceholder" id="viz1595554486655" style="position: relative"><noscript>[![ ](https://public.tableau.com/static/images/JQ/JQF9G5FX2/1_rss.png)](https://maps.philipmallis.com/victorian-bus-stop-patronage/)</noscript><object class="tableauViz" style="display:none;"><param name="host_url" value="https%3A%2F%2Fpublic.tableau.com%2F"></param> <param name="embed_code_version" value="3"></param> <param name="path" value="shared/JQF9G5FX2"></param> <param name="toolbar" value="yes"></param><param name="static_image" value="https://public.tableau.com/static/images/JQ/JQF9G5FX2/1.png"></param> <param name="animate_transition" value="yes"></param><param name="display_static_image" value="yes"></param><param name="display_spinner" value="yes"></param><param name="display_overlay" value="yes"></param><param name="display_count" value="yes"></param><param name="language" value="en"></param></object></div> <script type="text/javascript">                    var divElement = document.getElementById('viz1595554486655');                    var vizElement = divElement.getElementsByTagName('object')[0];                    vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';                    var scriptElement = document.createElement('script');                    scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    vizElement.parentNode.insertBefore(scriptElement, vizElement);                </script>- - - - - -

I think that this map by itself is fascinating. There are clear patterns for where boardings are high. The Werribee and Dandenong Lines have high boardings in the middle and outer suburbs, showing the high demand for interchanging between rail and bus services.

Although I’m not 100% sure what’s going on with the ‘Hume Anglican Grammar School’ stop in Craigieburn. I suspect that this may be a data error given that one of the default myki touch on locations (for when myki is running in ‘headless mode’ and doesn’t know where it is) is around there. So unless someone familiar with the area can explain this, I’m ignoring it for now.

I won’t go into detailed analysis about the spatial distribution of these stops as I think that deserves a separate post and others would probably do it better. For now, we’re just concerned with finding the busiest ones.

<div class="tableauPlaceholder" id="viz1595552684680" style="position: relative"><noscript>[![ ](https://public.tableau.com/static/images/20/2018-19BusStopPatronageMelbourne/Stopswith1000ormoreavgdailyboardings2/1_rss.png)](https://maps.philipmallis.com/victorian-bus-stop-patronage/)</noscript><object class="tableauViz" style="display:none;"><param name="host_url" value="https%3A%2F%2Fpublic.tableau.com%2F"></param> <param name="embed_code_version" value="3"></param> <param name="site_root" value=""></param><param name="name" value="2018-19BusStopPatronageMelbourne/Stopswith1000ormoreavgdailyboardings2"></param><param name="tabs" value="no"></param><param name="toolbar" value="yes"></param><param name="static_image" value="https://public.tableau.com/static/images/20/2018-19BusStopPatronageMelbourne/Stopswith1000ormoreavgdailyboardings2/1.png"></param> <param name="animate_transition" value="yes"></param><param name="display_static_image" value="yes"></param><param name="display_spinner" value="yes"></param><param name="display_overlay" value="yes"></param><param name="display_count" value="yes"></param><param name="language" value="en"></param><param name="filter" value="publish=yes"></param></object></div> <script type="text/javascript">                    var divElement = document.getElementById('viz1595552684680');                    var vizElement = divElement.getElementsByTagName('object')[0];                    vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';                    var scriptElement = document.createElement('script');                    scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    vizElement.parentNode.insertBefore(scriptElement, vizElement);                </script>- - - - - -

Probably as expected, Monash University takes first place with 5,912 average daily boardings.

Box Hill Station, North Melbourne Station, Chadstone Shopping Centre and Footscray Station take out the remaining top four spots.

Four out of these top five are significant destinations in their own right. North Melbourne Station is the anomaly here. Almost all of those boardings would be passengers changing from trains to buses, almost certainly to the University of Melbourne in Parkville.

[![Crowd of people boarding route 733 bus at Monash University, Clayton](https://live.staticflickr.com/65535/49849355461_7439628ce4_z.jpg)](https://www.flickr.com/photos/philipmallis/49849355461/in/photolist-2iX1YDT-2iX3yKY-2iWYfZm "Crowd of people boarding route 733 bus at Monash University, Clayton")<script async="" charset="utf-8" src="//embedr.flickr.com/assets/client-code.js"></script>- - - - - -

Most of the other 90 stops are associated with railway stations, reinforcing the important role that buses play in the rail network. Given that the latest data that we have on mode access at stations is from 2013-14, bus stop data like this is the next best thing that we have.

Some of the stops in the top 95 serve destinations that do not have heavy rail. Daniel Bowen has [noted this before](https://www.danielbowen.com/2020/07/03/sydney-vs-melb-rail-patronage/ "https://www.danielbowen.com/2020/07/03/sydney-vs-melb-rail-patronage/") as one of the key differences between Melbourne and Sydney and helps explain why the latter has train patronage around 50% higher than the former. Chadstone, Northland and Doncaster Shopping Centres are a few examples here.

A final note to make is that the numbers at these stops are definitely higher than recorded in this data. As mentioned previously, I have excluded numbers from default ‘headless mode’ stops. In this data, these numbers comprised 6.5% of the total patronage figure. It’s rather strange because in the notes from DoT, they said that headless mode data is excluded and estimate it at around 10%, and yet it does seem to be in the spreadsheet that they sent.

Regardless, these numbers are not just raw myki touch ons and offs. They’re part of a changing formula used by DoT to estimate patronage (detailed notes included in the data on [this page](https://public.tableau.com/profile/philipmallis#!/vizhome/2018-19BusStopPatronageMelbourne/Map)).

As always, if you have any thoughts or questions, please feel free to comment below.