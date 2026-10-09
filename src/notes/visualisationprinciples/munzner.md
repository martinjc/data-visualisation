---
layout: page
order: 1
title: Munzner's Four Level Model
parent: Assessing Visualisations
eleventyComputed:
  eleventyNavigation:
    key: "{{ title }}"
    parent: "{{ parent }}"
    order: "{{ order }}"
---

Tamara Munzner's "[Nested Model for Visualization Design and Validation](https://ieeexplore.ieee.org/document/5290695)" is a useful tool when considering the design of visualisations, that also allows us to evaluate the visualisation's effectiveness. The model proposes a four-level framework for thinking about and evaluating data visualisations, moving from the more abstract, high level goals of data visualisation, down to the more concrete, detailed implementation details. It relates to the three questions posed as part of the [Junk Charts Trifecta](https://www.junkcharts.com/junk-charts-trifecta-checkup-the-definitive-guide/), but more formally structures them and relates in a deeper fashion to the technical implementation of the visualisation.

The model can be used as an evaluative tool when considering visualisations, or as a guide to the design of visualisations. It presents the four-levels of consideration as:

1. **Problem** - is the right problem being addressed?
2. **Abstraction** - is the right thing being shown?
3. **Encoding** - Is the way the thing is being shown correct?
4. **Algorithm** - Is the thing working well enough?

These four layers are presented as nested within one another, as below:

{% image "src/img/visualisation-principles/munzner.png" "Munzner's Nested Model" "Reproduced from Munzner, T. [A Nested Model for Visualization Design and Validation](http://ieeexplore.ieee.org/document/5290695) in IEEE Transactions on Visualization and Computer Graphics, vol. 15, no. 6, pp. 921-928, Nov.-Dec. 2009, doi: 10.1109/TVCG.2009.111." %}

## Domain Problem Characterisation

This covers the tasks of data visualisation connected to understanding the context of the visualisation. What are the needs of the intended end users? What vocabulary do they use? What domain knowledge do they have? What are their workflows? These factors will all influence the design of the visualisation, and will help to ensure that the visualisation is fit for purpose. If this stage is wrong, or the output of this is wrong, we run the risk of building a visualisation that solves the wrong problem, and is therefore not useful. 

## Data Abstraction

This is about translating the domain problem characterisation into a more abstract representation of the data, considering the structure and semantics of the data that we will be working with. Here we are turning domain specific questions into data types and operations that can be understood. Here we are functionally choosing the operations that allow the questions of the end users to be answered, such as facilitating comparisons, summarising distributions, identifying trends, across the data we have selected

## Visual Encoding

Here we select the mappings of data attributes to visual variables, in order to encode the data and answer the questions we've formulated. This level moves from abstract considerations of operations and data types, to more concrete mappings of data to visual variables. Our key problem here is choosing the correct visual variables to represent the data, such as position, size, colour, shape, etc. We also need to consider the ordering of the data, and the arrangement of the data in the visual space to maximise accuracy, interpretability and cognition, without confusing or overwhelming.

## Algorithm

The final layer brings in the technical implementation of the visualisation, moving from abstract considerations of encodings and mappings to an actual implementation, in a manner that is efficient and that facilitates real-time user interaction and exploration.


{% panel "warning" "Downstream Cascade" %}
The real insight of this model is the notion that because the layers are nested within one another, an error at any one level will cascade down to the subsequent layers. So, if we get the domain problem characterisation wrong, even if we get the data abstraction and visual encoding correct, our visualisation is already compromised. A perfectly executed algorithm at Level 4 cannot redeem a flawed data abstraction at Level 2 or an incorrect domain problem characterisation at Level 1.  
{% endpanel %}

