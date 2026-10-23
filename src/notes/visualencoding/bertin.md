---
layout: page
order: 2
title: Bertin's Visual Variables
parent: Visual Encoding and Perception
eleventyComputed:
  eleventyNavigation:
    key: "{{ title }}"
    parent: "{{ parent }}"
    order: "{{ order }}"
---

## Bertin's Visual Variables

Jacques Bertin's _Sémiologie Graphique_ (or "Semiology of Graphics", [Bertin, 1967](https://books.google.com/books/about/Semiology_of_Graphics.html?id=X5caQwAACAAJ)) is a landmark text for data visualisation in which Bertin classifies the visual variables that can be used to encode data. 

Bertin’s foundational visual variables include 

1. position across the spatial plane - e.g. x/y/z coordinate,
2. size along visual dimensions - e.g. length, area, volume,
3. shape boundaries - e.g. circle, square, triangle,
4. orientation or tilt angle - e.g. alignment,
5. color hue derived from visual wavelength - e.g. red, blue, green,
6. color value or lightness - e.g. light, medium, dark, and 
7. visual texture grain, or pattern - e.g. dashed, dotted, solid. 

{% image "src/img/visual-encoding/bertin.png" "Bertin's Visual Variables" "Bertin's visual variables ordered by their ability to express specific levels of perceptual organisation. Jacques Bertin, Semiology of Graphics (1967)." %}

Bertin evaluated these visual channels through their ability to express specific levels of perceptual organisation, classifying visual properties into associative, selective, ordered, and quantitative visual capabilities.

{% accordion "Bertin's Classificaiton"%}
- Selective variables are those variables that allow us to pick out items from a visual display (e.g. choosing all the items of a particular colour). If the visual representation allows us to group data items together based on a particular visual variable, then that variable is selective.
- Associative variables are those variables that do not impact our ability to group items using selective variables. So, for example, shape is an associative variable, as shape does not impact our ability to pick out variables by colour. Disassociative variables are those that impact our ability to group items using selective variables. Size is a disassociative variable, as size impacts our ability to pick out variables by colour. 
- Ordered variables are those that have a recognisable order. Size is an ordered variable, as we can arrange things from smallest to largest.
- Quantitative variables allow us to estimate the value of a variable by comparing the difference between data points. Position and size are both quantitative.

A nice visual explainer for the differences between these classifications can be found at [Axis Maps](https://www.axismaps.com/guide/visual-variables)

{% endaccordion %}

Since Bertin first proposed this categorisation of variables in 1967, the list has been extended and further refined, most notably by Alan M. MacEachren in his book "How Maps Work: Representation, Visualization and Design". A good summary of an expanded list of visual variables, and their classifications can be found in [Roth (2017), "Visual Variables"](https://www.researchgate.net/publication/317266613_Visual_Variables).

Experimentation, such as that carried out by [Cleveland and McGill (1985)](https://www.jstor.org/stable/1695272) looks at the relative accuracy of different visual variables in order to rank them in terms of their effectiveness for encoding quantitative information.

{% image "src/img/visual-encoding/cleveland-mcgill.png" "Cleveland and McGill's Ranking of Visual Variables" "Cleveland and McGill's ranking of visual variables by their effectiveness for encoding quantitative information. Cleveland, W. S., & McGill, R. (1985). [Graphical Perception and Graphical Methods for Analyzing Scientific Data](https://doi.org/10.1126/science.229.4716.828). Science, 229(4716), 828–833. " %}

This provides a useful guide for us as visualisation designers into which types of visual representation will help us to communicate our data most efficiently and effectively, and which representations of data may cause larger issues and roadblocks to understanding. 

| Rank | Visual Variable | 
| ---- | --------------- |
| 1    | Position along a common scale |
| 2    | Position along non-aligned scales |
| 3    | Length |
| 4    | Angle and slope |
| 5    | Area |
| 6    | Volume, Density, Colour Saturation | 
| 7    | Colour Hue | Choropleth map |


{% panel "info" "Summary and Application"%}
Karl Sluis does a nice job of summarising the work of Bertin and how it relates to both designing and reading data visualisations in his article "[Before Tufte, there was Bertin](https://karlsluis.medium.com/before-tufte-there-was-bertin-63af71ceaa62)".
{% endpanel %}
