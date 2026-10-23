---
layout: page
order: 3
title: Exploratory Data Analysis
parent: Data Bias and Descriptives
eleventyComputed:
  eleventyNavigation:
    key: "{{ title }}"
    parent: "{{ parent }}"
    order: "{{ order }}"
---

EDA operates across univariate, bivariate, and multivariate domains:

- **Univariate Analysis:** Focuses on the descriptive statistics and visualisations of single variables. Tools and charts include kernel density estimates, histograms, boxplots, and empirical cumulative distribution functions.
    
- **Bivariate Analysis:** Examines relationships between two variables. This includes exploring various types of correlations, conditional distributions, and cross-tabulations to surface non-linear associations, multicollinearity, and variance shifts across subgroups. 
    
- **Multivariate Analysis:** Employs various dimension reduction techniques, canonical correlation, and high-dimensional scatterplot matrices to expose complex structures in high-dimensional feature spaces. This is less commonly done through data visualisation, but rather through various statistical methods and models.
    

EDA is not a preliminary cleaning step in the analysis pipeline, but a continuous iterative process between the researcher and the data.