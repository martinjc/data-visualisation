---
layout: page
order: 2
title: Visualisation Principles
parent: Data Visualisation
eleventyComputed:
  eleventyNavigation:
    key: "{{ title }}"
    parent: "{{ parent }}"
    order: "{{ order }}"
---

## Visualisation Principles

When we start to think about how to create a "successful" data visualisation we often start by thinking about what principles and guidelines we should follow.

{% panel "prompt" "Visualisation Principles" %}
Before we go on and read what others think about visualisation principles, lets stop and consider the role of 'rules' in data visualisation.

What does the word 'rule' mean to you personally? Reflect on your current understanding of visualisation principles. What guidelines do you believe are crucial for creating effective data visualisations? Consider instances where you felt a certain rule was essential, or perhaps an occasion when breaking a 'rule' led to a better understanding of the data.

Write down the list of your 'Top 10' most important visualisation rules.

{% endpanel %}

There are a lot of ways to think about such principles. Some might view them as concrete rules that must always be followed, and which can never be broken. Others see these rules as more flexible, as guidelines that we can follow, but that can be broken when appropriate. 

How many "firm" rules there are is a matter for debate, as is what guidelines are appropriate and how we should apply them.

[Chad Skelton](https://www.chadskelton.com/?m=1) gives an introduction to some of these debates in his article "[In defence of data visualization rules](https://www.chadskelton.com/2015/12/in-defence-of-data-visualization-rules.html?m=1)". He introduces some of these debates, and pushes back to argue that rules are very important, particularly for those who are new to data visualisation, essentially suggesting that they can help newcomers to avoid crucial mistakes.

Many in the data visualisation field push for a set of clear principles that focus on clear presentation of data in a minimalist or more scientific manner, favouring clarity and avoiding unnecessary additions to the data. This perspective is often associated with figures such as [Edward Tufte](https://www.edwardtufte.com/), who argues for a reduction of "chart junk" to allow the data to speak for itself. The idea here is that the data has an inherent structure and meaning, and that the role of the data visualisation practitioner is to reveal that structure and meaning as clearly and directly as possible. However, many others would argue favourably for a more aesthetic approach, seeing that there is a useful role for more artistic interpretation of data to reveal meaning, and to create more engaging and impactful visuals. 

[Giorgia Lupi](https://medium.com/@giorgialupi) makes this point in their article "[Beautiful Reasons](https://medium.com/@giorgialupi/beautiful-reasons-why-data-visualization-is-so-much-more-than-numbers-e31c8b30094e)", presenting a number of visualisations that clearly go against the minimalist principles of Tufte et al., yet are still effective at communicating data and engaging to their audience. The argument is made that aesthetic elements are not just "chart junk" but can actually be a useful part of the communication of data. 

[Lisa Charlotte Muth]() draws a lot of this together in her talk "[What to consider when considering data vis rules](https://lisacharlottemuth.com/datavisrules)". As well as bringing together some of the good reasons *for* data visualisation rules, she gives a good breakdown of what makes a good visualisation rule, and addresses the fact that often our data visualisation rules are contradictory - because they depend very much on the purpose of the visualisation. She goes on to link classical art theories to the aims of data visualisation, which can help us to understand where and when guidelines or rules might be most useful.


{% accordion "Artistic Theory" %}

Many rules within data visualisation directly contradict each other because they are rooted in fundamentally different **theories of data visualisation**. By applying traditional Western art theories to information graphics, Muth categorizes these conflicting priorities into five distinct lenses:

```
                       ┌────────────────────────┐
                       │ Theories of Visual Art │
                       └───────────┬────────────┘
        ┌──────────────┬───────────┼──────────────┬──────────────┐
        ▼              ▼           ▼              ▼              ▼
  ┌───────────┐  ┌───────────┐┌───────────┐  ┌───────────┐  ┌───────────┐
  │ Formalism │  │Instrumen- ││Expression-│  │Imitational│  │Institu-   │
  │           │  │talism     ││ism        │  │ism        │  │tionalism  │
  └───────────┘  └───────────┘└───────────┘  └───────────┘  └───────────┘
```

| Visual Theory | Primary Focus & Judgment Criteria | Key Visual Examples |
| :--- | :--- | :--- |
| **Formalism** | Judged by composition, visual beauty, symmetry, innovative use of shapes, and colour palettes. | Nadieh Bremer's *Royal Constellations*; creative, non-traditional shapes. |
| **Instrumentalism** | Judged by purpose, utility, speed of informing, social impact, and driving change. | Interactive COVID-19 dashboards (e.g., ZEIT Online); financial dashboards. |
| **Expressionism** | Judged by how successfully the graphic expresses or evokes human emotion and feelings. | Giorgia Lupi's *Bruises* (Data Humanism); NYT list of COVID-19 victims. |
| **Imitationalism** | Judged by how realistically and objectively the chart portrays the complete, raw complexity of the data. | Detailed "Maps of the Web"; Reddit comment network maps; detailed Raincloud distribution plots. |
| **Institutionalism** | Judged by the consensus of authority, award bodies, expert curators, and established organizational guidelines. | Kantar *Information is Beautiful* Awards; Tableau *Iron Viz* winners; corporate style guides. |

{% endaccordion %}

Ultimately then, when you are thinking about creating a data visualisation, the first thing you should be thinking about is **what are you trying to achieve with this visualisation?** It is this key question that will help you to decide which of these visual principles are most important for your particular visualisation, and to make good decisions about how to create an effective data visualisation for your particular purpose.

