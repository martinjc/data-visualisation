---
layout: page
order: 1
title: Data and Measurement
parent: Data Bias and Descriptives
eleventyComputed:
  eleventyNavigation:
    key: "{{ title }}"
    parent: "{{ parent }}"
    order: "{{ order }}"
---

## Data as Quantitative Observations

Data often consists of collections of empirical observations or numerical measurements (e.g., household demographics, civic metrics, voter turnout, local business employee ages). However, the process of collecting and recording that data is always subject to some degree of measurement error. These errors can range from the negligible, through acceptable levels of noise, up to severe systematic distortion.

{% panel "info" "The Principle of Error Awareness" %}
Visualisation does not eliminate measurement error. Analysts must assess the relative magnitude of potential error and determine whether it fundamentally alters the message, visual encoding, or decision-making context. It is important to remember that any errors present in the data will be carried through to the visual representation.
{% endpanel %}

Measurement error can be thought of as the difference between the true underlying value of a phenomenon (the conceptual 'truth') and the recorded observation (the empirical data). Understanding the sources and types of measurement error is essential for assessing data quality and the reliability of visual representations.

### Types of Measurement Error

Measurement error can be broadly classified into random error and systematic error, each originating from different sources and possessing distinct statistical properties.

#### Random Error
Random error refers to unpredictable fluctuations or variations in measurement that do not follow a systematic pattern. These errors typically arise from chance factors during the measurement process and tend to cancel each other out over multiple observations.

* **Sources:** Random variations in measurement instruments (e.g., fluctuations in power supply, sensor noise), inconsistent recording procedures, or unpredictable environmental factors (e.g., temperature variations, air currents).
* **Characteristics:** Random errors follow a random probability distribution (often assumed to be normal) around the true value. They do not bias the measurement in a consistent direction but rather introduce noise, which can be reduced by increasing sample size or using averaging techniques.
* **Impact on Visualisation:** Random error affects the precision of visual encodings. In a scatterplot, for instance, random measurement error causes points to deviate from their true positions, creating "scatter" around the underlying trend. While it does not systematically distort the overall pattern, it can obscure subtle effects and reduce the clarity of relationships, particularly in datasets with large measurement variability relative to the effect size.

#### Systematic Error
Systematic error (also known as bias) refers to consistent, repeatable deviations from the true value that occur in the same direction across all measurements. Unlike random error, systematic error shifts the measurements in a predictable manner, leading to biased estimates and potentially misleading interpretations.

* **Sources:** Systematic errors can arise from various sources, including instrument calibration issues (e.g., an uncalibrated scale consistently reading high), methodological flaws (e.g., a survey question phrased in a leading manner), or consistent environmental conditions that affect all measurements uniformly.
* **Characteristics:** Systematic errors introduce a bias that consistently shifts measurements in a particular direction (either higher or lower than the true value). This bias can be constant (absolute error) or proportional to the true value (relative error). Unlike random error, increasing the number of measurements does not reduce systematic error; in fact, it can compound the bias if the error source persists.
* **Impact on Visualisation:** Systematic error fundamentally distorts visual representations by shifting the perceived relationships between variables. In a bar chart, for example, a systematic error that inflates all values will exaggerate the magnitude of differences between categories. In a line chart, a bias that increases over time will create a misleading impression of accelerating growth or decline. Detecting and correcting systematic error is crucial for maintaining the integrity of visualisations, as bias can lead to incorrect conclusions and flawed decision-making.

### Examples of Measurement Error

Understanding these error types is critical in practical data analysis, as real-world datasets are often subject to one or both forms of measurement error. Below are examples of how measurement error can manifest in different data collection scenarios.

**Example 1: Household Energy Consumption Survey**
Consider a survey collecting data on household energy consumption in a metropolitan area. Residents are asked to report their monthly electricity usage based on utility bills.
* **Random Error:** A household might misread their bill, reporting 450 kWh instead of the actual 425 kWh. This type of error is random and may occur due to fatigue or momentary distraction. While such misreporting can vary between households and from one month to the next, these random fluctuations are unlikely to significantly alter the overall distribution of energy consumption across the entire sample, particularly if the sample size is large.
* **Systematic Error:** However, if the survey is administered during a particularly hot summer month, many households may report higher energy consumption than usual due to increased air conditioning usage. This systematic effect, driven by an external environmental factor, would cause all reported values to be elevated relative to their typical levels. If not accounted for, this bias would lead to an overestimation of typical energy consumption, potentially skewing promotional materials or policy recommendations based on the survey data.

**Example 2: Voter Turnout in Municipal Elections**
A municipal government wants to understand voter turnout patterns to improve engagement strategies. They collect data on voter turnout from polling stations across different wards.
* **Random Error:** Some polling stations might experience minor technical glitches with electronic poll books, leading to slight delays in recording voter entries. These delays, which can vary unpredictably depending on the severity of the issue and the time it takes to resolve, represent random errors in the timing of turnout counts. While they might slightly inflate or deflate turnout in specific polling stations, the overall pattern of turnout across wards is less likely to be systematically affected.
* **Systematic Error:** In contrast, suppose that the polling stations in wards with lower socioeconomic status experience more frequent power outages. Each outage requires manual backup procedures, which can lead to undercounting or delayed reporting of voters. This systematic issue would cause turnout figures in these wards to be consistently lower than in wards with reliable power infrastructure, even if the actual voter interest is similar. A data visualisation that fails to account for this systematic bias would incorrectly suggest that residents in these wards are less engaged in the electoral process, leading to inappropriate policy responses.

**Example 3: Age Distribution of Employees in Local Businesses**
A business development agency surveys local businesses to understand the age demographics of their workforce. They collect data on the ages of employees from participating businesses.
* **Random Error:** Some employees might provide rounded ages (e.g., reporting 40 instead of 38 or 42). This type of random rounding is likely to be distributed somewhat evenly around the true ages, with no systematic upward or downward bias across the entire dataset.
* **Systematic Error:** However, if the survey is primarily distributed through channels that are more accessible to older business owners or if the data collection methods favour certain types of businesses, the sample may be systematically biased. For instance, small family-owned businesses with long-established workforces might be overrepresented, leading to an inflated perception of the average employee age. Without awareness of this potential bias, an analyst might incorrectly conclude that the local workforce is aging more rapidly than it is, potentially misinforming workforce development strategies.

