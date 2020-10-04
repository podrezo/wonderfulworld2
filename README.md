# Wonderful World

Wonderful World is a curated list of awesome sight-seeing places to visit around the world. You can view the live site at https://wonderfulworld.podrezo.com/

## Running the project locally

This project uses the static website generated called Hugo. [Install Hugo](https://gohugo.io/getting-started/quick-start/) and then clone the project. Simply run `hugo server` from the root directory of the project and then browse over to the URL it outputs to see the website.

## Contributing: Adding a new location

Create a new directory under `content` and give it a descriptive name, following the same convention as the other directories in there. In this directory, create a new markdown file called `_index.md` and follow this recipe for the file content:

```
---
title: NAME_OF_THE_PLACE
country: TWO_LETTER_ISO_3166_COUNTRY_CODE
details_link: SOME_LINK_FOR_MORE_INFO
author: AUTHOR_NAME
longitude: FLOATING_POINT_LONGITUDE
latitude: FLOATING_POINT_LATITUDE
layout: location
tags:
  - Tag 1
  - Tag 2
  - ...
---
Description here. *Markdown is allowed.*

```

Optional fields: `author`, `details_link`. The details link is ideally something useful to travellers like an article about the place from [WikiVoyage](https://www.wikivoyage.org/). For an example of a filled-out file, check the files already inside the `content` directory. It is critical that the country code is present in the `data/countries.yaml` file in order to properly render country name and flag. To find the Alpha-2 code you can consult [this table from Wikipedia](https://en.wikipedia.org/wiki/ISO_3166-1#Officially_assigned_code_elements) or simply check that same `data/countries.yaml` file to search the code by name.

Add images, simply put the files in the same directory as the `_index.md` file you created. Images **must be under 1MB** in file size. The thumbnail image will be the alphabetically first image file in the directory.


## TODO

* Clickable world map of all places
* Meta tags for sharing and social networking
* Make the theme more fun
