---
id: 3624
title: 'How to export Flickr photos with metadata attached'
date: '2023-09-11T16:02:21+11:00'
author: Philip
guid: 'https://philipmallis.com/?p=3624'
image: https://upload.wikimedia.org/wikipedia/commons/f/f4/Flickr_logo_-_SuperTinyIcons.svg
categories:
    - Photography
tags:
    - Flickr
---

I have been a user of Flickr for about eight years. While I have no plans to move away, there are many reasons why someone would want to export their photos and videos.

Having spent many hours reading through forum posts, documentation and Github repositories, I want to share my method of how I achieved this. It wasn’t easy.

If you want to skip the backstory and go straight to the method, click [here](#method-that-works "here").

## Parameters

What I needed was a download of all of my Flickr content with the metadata attached.

The issue is that Flickr only allows you to export photos with the data attached from **before** it was uploaded. So if you were like me, and did at least some editing within Flickr itself, none of this would be attached to the files.

The only thing to do is to either request a data export of all Flickr content, where all of this would be contained in separate .json files, or use a third-party provider.

This also assumes that you are only downloading your own Flickr content and not someone else’s.

## What I tried

Eventually I finally figured out that since 2020, Flickr have added additional numbers to file names. As a result, the \[8\] in the command that captures the image ID number in Step 6 below should now be an \[11\]. And that’s what finally made it work!

## Method that works

This works on Linux but should also work on Windows with the necessary tweaks.

Before you start, install:

- [Downthemall](http://downthemall.org/)
- [Exiftool](http://exiftool.org/ "Exiftool")

Then follow these steps:

1. Navigate to Flickr account settings page to download your entire Flickr archive
2. Use Downthemall (right-click) and filter by .zip files to download all of the files into the folder of your choice
3. Extract all of the archives into a single folder (right-click and go ‘extract’ in 7Zip or whatever)
4. Run this command in your command prompt/console: `exiftool -s file.json` (change \[file.json\] to the path to any photo file in that folder)
5. Read the output and select which tags you want to extract. Then match these tags to whichever items you want to attach the image to on this list of supported EXIF metadata: <https://exiv2.org/tags.html>
6. Run this command in your command prompt/console: `exiftool -AddTagsFromFile %dphoto_%-11.2f.json "-keywords<AlbumsTitle" "-ImageDescription<Title" "-gpslatitude<GeoLatitude" "-gpslongitude<GeoLongitude" "-name<Name" "-keywords<TagsTag" "-ProfileCopyright<License" <fullfilepath> `(note that all of the items in double quotation marks are examples only, you should change these to the tags that you want as outlined in Step 5 – the first name being what is listed in the exiv2.org link earlier, the second being what the output shows in Step 4. Also change &lt;fullfilepath&gt; to the path shown when you drag and drop a file into the terminal, for some reason relative paths weren’t working for me.)
7. Execute the command.
8. Once this is completed, check one of the new image files by running `exiftool -s` again on one of them to see that it has everything you need.
9. If you are like me, you ended up with a second copy of these files. To get rid of these, run &lt;COMMAND&gt;
10. Open your photos in the photo editor/organiser of your choice (I use and recommend [Digikam](https://www.digikam.org/)).

Congratulations, that should be all!

Once that’s done, you may want to sort them. Exiftool has a lot of different ways to do this. One of the most common is organising by date and time. If you are interested in doing this, I found this page to be the most helpful: https://exiftool.org/filename.html

Many thanks to the many people who created resources previously to explain this. For further reading and information, please go to these places:

- <https://exiftool.org/forum/index.php?topic=11072.0>
- [https://exiftool.org/exiftool\_pod.html](https://exiftool.org/exiftool_pod.html)
