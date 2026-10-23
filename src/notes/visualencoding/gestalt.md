---
layout: page
order: 3
title: Gestalt Principles
parent: Visual Encoding and Perception
eleventyComputed:
  eleventyNavigation:
    key: "{{ title }}"
    parent: "{{ parent }}"
    order: "{{ order }}"
---


## Gestalt Psychology

_Gestalt Psychology_ is a perceptual theory that considers how the human visual system organises separate pieces of visual information into meaningful wholes. The term _Gestalt_ translates from German to something like "form", "shape", or "unified whole", and the central idea in this theory is that the whole is greater than the sum of its parts. In the context of data visualisation, this means that the way we arrange and combine visual elements can influence how people perceive and understand the data we present. 

This area of psychology is important as our cognitive systems use visual shortcuts and pattern completion heuristics (e.g. preattentive processing, which we'll discuss later), which means that unconsidered visual layouts can inadvertently trick the brain into perceiving non-existent relationships, while well-considered layouts can significantly improve our ability to understand and interpret data. 

### Core Gestalt Principles

* **Emergence:** Simple shapes aggregate visually to reveal macro-patterns, allowing viewers to grasp global structures prior to individual elements.
* **Constructive Perception (Reification):** The visual system completes missing geometric information, causing viewers to perceive objects or boundaries that do not physically exist in the data.
* **Multistable Perception:** The cognitive capacity to perceive a visual artifact in multiple distinct structural or functional states simultaneously.
* **Invariance:** The ability to recognize visual objects as identical across changes in scale, orientation, rotation, or surface texture.
* **Grouping:** Automatically categorizing individual elements into sets or unified clusters based on spatial layout, proximity, similarity, or enclosure.

You can see that some of these link in to Jacques Bertin's ideas of classification of visual variables, particularly the ideas of selective and associative/disassociative variables. 

{% panel "warning" "Warning!"%}
If Gestalt principles are not applied intentionally, layout choices can trigger accidental grouping or visual illusions, leading users to infer erroneous trends not supported by the data. Being aware of the principles and the effects they can cause is important in avoiding unintentional misinterpretations.
{% endpanel %}

Elijah Meeks has a series of articles with some interesting visualisations exploring Gestalt principles. In [Part 1 he looks at similarity, proximity and enclosure](https://emeeks.github.io/gestaltdataviz/section1.html) - all related to the grouping principle in the list above. In [Part 4 he considers figure, ground and metastablity](https://emeeks.github.io/gestaltdataviz/section4.html), picking up on the ideast of Emergence, Constructive Perception and Multistable Perception. These are worth looking at to get a sense of *how* these Gestalt principles might align with and impact the creation and reading of data visualisations. 