---
title: "Coding"
pre: "<b>4. </b>"
date: 2022-04-11T18:23:56+01:00
draft: false
---

The sportclimbs.uk site uses the [Hugo static site generator](https://gohugo.io/) to build the content files and templates into a web site.

The site has various custom functions described here.

## Maps

The maps used are by [Leaflet JS](https://leafletjs.com/), a javascript library.

To add a map to a page add the two variables to the frontmatter: `map` and `markers`.

The `map` variable sets 2 things: 

1. the centre of the map and also 
2. the zoom level

The `markers` variable sets the position of a marker and text to appear when the marker is clicked.

```yaml
map: [52.993516, -4.392794, 15]
markers:
- [52.98158, -4.39739, Parking]
- [52.993516, -4.392794, Trefor]
```

With a list of markers only the last one will display it's name. In the above example the marker will display *Trefor*. The other markers need to be clicked on first.