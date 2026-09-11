---
layout: page
order: 3
title: Tradeoffs and debates in Data Visualisation
parent: Introduction to Data Visualisation
eleventyComputed:
  eleventyNavigation:
    key: "{{ title }}"
    parent: "{{ parent }}"
    order: "{{ order }}"
---

## Tradeoffs and debates in Data Visualisation

As we will see, the field of Data Visualisation is one of considerable debate and disagreement. The nature of data visualisation is such that there are few hard and fast rules, and many guidelines and best practices are based on an accumulation of experience and evidence, rather than on rigorous scientific experimentation and proof. This is a field where there are few universal truths, and where the best approach is often context- and audience-dependent. Not only that, but there remains a distinct subjective element around individual aesthetic preferences, making consideration of what makes a 'good' or 'effective' visualisation often a case of balancing conflicting principles and preferences, rather than a case of finding the single 'right' answer.

For example, a key tradeoff or discussion within the field is that of minimalism vs graphical embellishment. Practitioners such as Edward Tufte propose minimalist approaches, arguing that the best data visualisations are those that present data in a clear, concise, and uncluttered manner, without any unnecessary adornment. In contrast, other practitioners argue that some level of graphical embellishment can be beneficial, as it can help to make the data more engaging and easier to understand, as well as increasing long term memorability. Indeed, empirical research by [Bateman et al. (2010)](https://doi.org/10.1145/1753326.1753716 "null") found that more embellished graphics led to both better long term memorability and engagement.  As we look at more examples we will see more of these sorts of tradeoffs and debates in practice.


## Ethics of Data Visualisation

Some may hold that a visual representation of data is an objective and accurate portrayal of that data, a neutral medium for transmitting information from one person to another, in the form of a visual 'truth'. However, the reality is somewhat more complex. The process of data visualisation is necessarily one of making decisions, and as such, it is inherently subjective. Furthermore, the choices we make can have a significant impact on how our data is perceived and interpreted, and as such, it is important to consider the ethical implications of our work and the decisions that are made as part of that work. The choices we make in the analysis of data, the presentation of data, and the communication of data can all have profound implications for our audiences, and as such, we must be careful to consider these implications as we work. 

{% accordion "Learn more: Visualisation Rhetoric" %}

Jessica Hullman and Nicholas Diakopoulos ([2011](https://ieeexplore.ieee.org/document/6064988)) formalised this idea by analysing the rhetoric of data visualisation, how data graphics function as persuasive, editorialised and culturally situation communications, rather than objective depictions of an underlying reality. They highlight the impact design decisions at all stages of the visualisation pipeline have on the message that is communicated to the audience, particularly as different decisions on the additions or omissions of information at various levels impact how the audience perceives and interprets the data.

```
+-----------------------------------------------------------------+
| 1. Data Layer           (Omission, Aggregation, Binning)        |
+-----------------------------------------------------------------+
                                |
                                v
+-----------------------------------------------------------------+
| 2. Visual Encoding Layer (Mapping, Scale Selection, Color Hue)  |
+-----------------------------------------------------------------+
                                |
                                v
+-----------------------------------------------------------------+
| 3. Text & Annotation Layer (Titles, Labels, Annotations)  |
+-----------------------------------------------------------------+
                                |
                                v
+-----------------------------------------------------------------+
| 4. Interaction Layer     (Tooltips, Filtering, Default Views)   |
+-----------------------------------------------------------------+
```

### 1. The Data Layer (Editorial Selection)

The choices made prior to visual mapping determine what information is made accessible:

- **Omission & Filtering:** Excluding extreme values, specific demographic subsets, or temporal segments to align data trends with a preferred narrative.
    
- **Dynamic Binning & Aggregation:** Grouping continuous data into custom bins (e.g., age groups or income brackets) to exaggerate or minimize variance across categories.
    
- **Baseline Selection:** Choosing arbitrary starting points or temporal ranges (e.g., picking local peaks vs. long-term trend baselines) to alter perceived growth rates.
    

### 2. The Visual Encoding Layer (Mapping Mechanics)

How structured data parameters are bound to graphical channels introduces rhetorical emphasis:

- **Axis Truncation & Non-Zero Baselines:** Truncating the quantitative axis in bar charts exaggerates relative proportional differences.

- **Non-Linear Scaling:** Applying logarithmic or square-root scales without clear perceptual cues can compress exponential growth, making rapid escalation appear linear or stabilized.
    
- **Color Semantics & Saliency:** Using culturally loaded color palettes (e.g., aggressive red shades vs. neutral grays) primes emotional reactions, while non-monotonic color ramps obscure subtle numerical gradients.
    

### 3. The Textual & Annotation Layer (Linguistic Framing)

Textual elements guide how perceptual inferences are translated into cognitive conclusions:

- **Slant & Loaded Titles:** An imperative title (e.g., _"Unemployment Spikes Sharply"_) pre-interprets a chart for the user compared to a neutral descriptor (e.g., _"Quarterly Unemployment Rates: 2020–2024"_).
    
- **Visual Callouts:** Using arrows, shaded trendlines, or highlighted callout boxes forces immediate visual focus onto specific regions while drawing attention away from contextual baselines.
    
- **Statistical Context:** Omitting confidence intervals, error bars, or sample sizes presents uncertain or noisy estimates as deterministic facts.
    

### 4. The Interaction Layer (Procedural Rhetoric)

In interactive dashboards, the software interface regulates exploration:

- **Default Presets:** The initial state of an interactive graphic serves as an anchor bias. Most users do not modify dynamic filter options or adjust default zoom levels.
    
- **Constrained Filtering:** Limiting slider ranges, dynamic axes, or drill-down features prevents users from testing alternative hypotheses.

This introduces the suggestion that we have both white-hat and black-hat capabilities as data visualisation practitioners, and that the power to alter the interpretation of a visualisation lies with us as designers, not with our audience, who may not be equipped to critically evaluate the visualisation. 

{% endaccordion %}
