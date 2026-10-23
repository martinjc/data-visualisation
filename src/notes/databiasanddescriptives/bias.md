---
layout: page
order: 2
title: Bias
parent: Data Bias and Descriptives
eleventyComputed:
  eleventyNavigation:
    key: "{{ title }}"
    parent: "{{ parent }}"
    order: "{{ order }}"
---

In the last section we talked about random sources of error and systemic errors. Such systematic errors are often caused by **Bias**. There are many different types of Bias.

 | Bias Type                    | Definition / Mechanism                                                                                  | Impact on Visual Analytics                                                 |
| :--------------------------- | :------------------------------------------------------------------------------------------------------ | :------------------------------------------------------------------------- |
| **Selection Bias**           | Systematic differences in the likelihood of individuals or instances being included in a sample.        | Produces unrepresentative distributions; distorts baseline metrics.        |
| **Volunteer Bias**           | Occurs when individuals who self-select into a study differ systematically from the general population. | Over-represents highly motivated or extreme viewpoints.                    |
| **Non-Response Bias**        | Arises when non-respondents differ significantly in key attributes from those who participate.          | Creates blind spots in categorical or demographic data.                    |
| **Informative Censoring**    | Loss of participants or subjects over time in longitudinal studies where dropouts are non-random.       | Skews trend lines and time-series visualisations.                          |
| **Interviewer Bias**         | Unconscious or deliberate influence by the researcher via questioning tone, framing, or probing.        | Introduces systematic measurement shifts in survey responses.              |
| **Recall Bias**              | Errors stemming from the inherent fallibility and inaccuracies of human memory.                         | Leads to distorted historical or retrospective datasets.                   |
| **Detection Bias**           | Differences in the likelihood of detecting or reporting specific events or phenomena across groups.     | Spurious inflations in occurrence rates among heavily monitored subgroups. |
| **Social Desirability Bias** | Tendency for respondents to adjust answers to conform to societal expectations or interviewer cues.     | Deflates sensitive metrics; inflates socially approved behaviors.          |

{% panel "warning" "Bias' impact" %}
Unaddressed bias leads to fundamentally misleading graphics. When visualising biased data, we must either apply statistical adjustments or explicitly annotate limitations.
{% endpanel %}


To maintain analytical integrity when visualising data:

1. **Evaluate Provenance:** Investigate how measurements were collected, noting sampling methods and potential dropout rates.
2. **Determine Error Significance:** Quantify error margins where possible (e.g., displaying confidence intervals or error bars).
3. **Contextualize Limitations:** Use captions, notes, or inline annotations to disclose known biases, preventing misinterpretation by target audiences. 