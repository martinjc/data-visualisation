---
layout: page
order: 1
title: Exploratory vs. Explanatory Data Visualisation
parent: Introduction to Data Visualisation
eleventyComputed:
  eleventyNavigation:
    key: "{{ title }}"
    parent: "{{ parent }}"
    order: "{{ order }}"
---

## Why do we visualise data?

We have seen above that data visualisation is the process by which we can both understand and communicate about data. These two tasks are often referred to as separate processes; exploratory data visualisation and explanatory data visualisation


### Exploratory vs. Explanatory

**Exploratory data visualisation** is used when we are analyzing a dataset to discover its underlying patterns, trends, anomalies, or structure. In this phase, we are "finding the story" within the data, and the primary audience is ourselves. The visualisations are often quick, iterative, and interactive, helping us formulate hypotheses. In contrast, **explanatory data visualisation** is employed when we have already discovered an insight and want to communicate it to others. Here, we are "telling the story" of the data, and the audience consists of stakeholders, clients, or the general public. Consequently, explanatory visualisations require careful design, formatting, and curation to highlight the key takeaways clearly and avoid cognitive overload.

### Exploratory Data Visualisation

Anscombe's Quartet and the Datasaurus provide us with very compelling practical examples of the need for exploratory data visualisation, and the many examples of 'poor' graphics that are often used to communicate data will highlight the need for a good understanding of effective explanatory data visualisation. 

**Anscombe's Quartet** is a collection of four synthetic datasets constructed by the English statistician Francis Anscombe in [1973](https://doi.org/10.1080/00031305.1973.10478966). All four datasets consist of eleven $(x, y)$ coordinate pairs. When evaluated using traditional summary statistics, all four sets yield nearly identical numerical results. However, when visualised, we realise that the datasets are in fact very different:

{% image "src/img/introduction-to-data-visualisation/anscombe_quartet.png", "Anscombe's Quartet" %}

The **DataSaurus** is a more recent, similar example to Anscombe's Quartet, where a dataset of 12 points was created by  by Justin Matejka and George Fitzmaurice ([2017](https://doi.org/10.1145/3025453.3025912 "null")), building on Alberto Cairo's "Datasaurus":

{% image "src/img/introduction-to-data-visualisation/datasaurus.gif", "The DataSaurus" %}

Together, these examples clearly demonstrate that statistical analysis of our data is not enough when attempting to identify patterns and draw conclusions, and that visualisation is a must if we are to reveal the real story within our data.



### Explanatory Data Visualisation

Explanatory data visualisation follows exploratory data visualisation; once we have discovered the story within the data **explanatory data visualisation** is about communicating that story to others in an effective and ethical manner. We use a range of tools, techiques and principles to create visualisation that deliver effective messaging to our target audience within the minimum of cognitive effort and within the relevant communicative context and ethical framework.


{% accordion "Learn more: Exploratory vs. Explanatory Data Visualisation" %}
Data visualisation serves two fundamental, yet distinct, roles in the data lifecycle: **discovering insights** (Exploratory) and **communicating conclusions** (Explanatory). Understanding when and how to apply each approach is crucial for analysts, data scientists, and communicators.

Exploratory data visualisation focuses on discovering insights hidden within data, whereas explanatory data 
visualization focuses on communicating a specific narrative or takeaway once those insights are found.

---

## Comparison Table

| Feature / Dimension | Exploratory Data Visualisation | Explanatory Data Visualisation |
| :--- | :--- | :--- |
| **Core Purpose** | Uncover hidden patterns, anomalies, trends, and hypotheses | Deliver a clear, targeted story, recommendation, or takeaway |
| **Primary Audience** | Analysts, data scientists, domain experts, researchers | Decision-makers, executives, clients, general audience |
| **Data State** | Raw, granular, complex, multidimensional, unfiltered | Aggregated, curated, filtered, focused |
| **Visual Design** | Functional, rapid, low-polish, system defaults | Polished, intentional, high signal-to-noise ratio, custom styled |
| **Interactivity Level** | High (slicing, zooming, filtering, drill-downs) | Low to Moderate (guided narrative, static presentation) |
| **Key Question Asked** | *"What story is hidden inside this dataset?"* | *"What conclusion or action should the audience take?"* |
| **Focus on Detail** | High depth; displays variance, outliers, and noise | High focus; highlights specific data points and mutes noise |
| **Primary Workflow** | Fast, flexible, hypothesis-driven iteration | Strategic, audience-centric visual storytelling |
| **Common Tools** | Python (Seaborn/Matplotlib), R (ggplot2), Jupyter, SQL drafts | PowerPoint, Figma, Datawrapper, Tableau Dashboards, D3.js |

---

## 1. Exploratory Data Visualisation

Exploratory Data Analysis (EDA) relies heavily on exploratory visualisation. In this phase, you are looking for the story within the data, without necessarily knowing what that story might be. We focus on quick, iterative chart generation without emphasis on custom palettes, titles, or aesthetic formatting. We use full raw datasets, and start to filter only once we know data is not relevant to the conclusions we are drawing. This process allows us to rapidly test assumptions about the data, the hypothesis, and the potential insights that may be drawn from it.

### Key Objectives
- Identify distributions (normal, skewed, bimodal, long-tailed).
- Detect missing data, anomalies, or collection errors.
- Discover correlation and collinearity between multiple variables.
- Formulate data-driven hypotheses for statistical validation.

---

## 2. Explanatory Data Visualisation

Once our insights are extracted and validated, we move to the explanatory data visualisation phase. The goal here shifts from discovery to persuasion, clarity, and guidance; our focus is on communicating a clear, targeted story or recommendation to a specific audience, using curated, polished visuals that minimise cognitive load and drive action. We are no longer asking "what story is hidden inside this dataset?", but rather "what conclusion or action should the audience take?".

### Key Objectives
- Drive decision-making among business leadership or non-technical stakeholders.
- Minimise cognitive load so the visual message is understood within seconds.
- Provide clear narrative structure with actionable recommendations.

---

## From Exploration to Explanation

A common mistake in communication is presenting _exploratory_ visuals to the audience instead of taking the time to develop _explanatory_ visuals.

```
[ Raw Data ] ---> ( Exploratory Vis ) ---> [ Insight Discovery ] ---> ( Explanatory Vis ) ---> [ Decision / Action ]
```

- **Exploratory Visuals** are designed for *the analyst* 
- **Explanatory Visuals** are designed for *the audience*
{% endaccordion %}