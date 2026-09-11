---
layout: page
order: 4
title: Thinking about visualisation
parent: Introduction to Data Visualisation
eleventyComputed:
  eleventyNavigation:
    key: "{{ title }}"
    parent: "{{ parent }}"
    order: "{{ order }}"
---

# Thinking about visualisation

Look at the visualisation below. You may already have seen it (or a similar visualisation) elsewhere. These are the 'Climate Change Stripes' which visualise the change in gloabl temperatures from 1850 to the present day. Blue represents a year that was cooler than average, red represents a year that was warmer than average.

{% image "src/img/introduction-to-data-visualisation/climate_stripes.png", "Climate Stripes" %}

Now consider the second visualisation below, which shows the same data, in a different way:

{% image "src/img/introduction-to-data-visualisation/climate_stripes_context.png", "Climate Stripes" %}

Both visualisations show exactly the same data, but use different forms and visual encodings to represent that data. The first uses regular bars of equal height, where only the colour represents the magnitude of the data. The second also uses bars, but this time uses both colour and height to represent the data values, and includes a central '0' line from which bars rise of fall to represent whether they are positive (warmer) or negative (cooler). The second visualisation also includes more information, including the start and end year, an explanatory headin, and some scales on the axes.

Considering all this information, and thinking about how you read the visualisations, do you think the visualisations have exactly the same aim? Do you think one visualisation is more effective than the other visualisation? If the data is the same, and the aim of the visualisations are the same, what has led to them using different forms? Why are they different?

{% panel  "info" "A prompt" %}
Have a think about these questions for a moment, then write down your answers.
{% endpanel %}
