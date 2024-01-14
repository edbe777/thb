# Hugo Split Gallery

Split Gallery is a theme for [Hugo](http://gohugo.io/) focused on photos and maps.  
This Hugo theme features a photo gallery, a map and custom content per page, and supports custom sections and taxonomies.

This project is licensed under the [GPLv3 license](/LICENSE). Due to 3rd-party included in this project, you are *not* free to use it for commercial applications. See the license section below for more info.

It is inspired by [Hugo Split Theme](https://github.com/christianmendoza/hugo-split-theme), itself ported from [Split](https://onepagelove.com/split) by [One Page Love](https://onepagelove.com).

### Structure of Posts

This theme requires each post to follow this structure:

```text
content/
├── posts
│   ├── First_post
│   │   ├── index.md
│   │   ├── track0.gpx
│   │   └── images
│   │       ├── IMG0.jpg
│   │       └── ..
│   ├── Second_post
│   │   ├── index.md
│   │   ├── track1.gpx
│   │   ├── track2.gpx
│   │   └── images
│   │       ├── IMG1.jpg
│   │       ├── IMG2.jpg
│   │       └── ..
```

Photos displayed in the gallery **must** be in a `images` subfolder, and track(s) -if any- must be at the same level as the content.
Supported formats for tracks are GPX (`.gpx` files), KML (`.kml` files) and GeoJSON (`.geojson` files).

Additionnally, the content of the post:
* **requires** an `images` parameter, refering to at least one picture from this post, which will be used as thumbnail in the home gallery,
* can have a `seealso` parameter, refering to one or multiple other posts.

Example:

```text
---
title: "Test1"
date: 2024-01-40T00:00:00+00:00
images: ["images/IMG19.jpg"]
seealso: ["posts/test-a", "posts/test-b"]
---

```


## License

This theme is licensed under the [GPLv3 license](/LICENSE), except for the photos distributed with the example site which are not free to use.

This theme includes [fancybox](https://fancyapps.com/fancybox/3/), which is not free to use for commercial applications. If you wish to use this theme in commercial applications, you will need to get a [commercial license from fancybox](https://fancyapps.com/fancybox/3/#license).

All other third-parties included are free to use (under MIT License, SIL OFL 1.1, BSD-2-Clause).
