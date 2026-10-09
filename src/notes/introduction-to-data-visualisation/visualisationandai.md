---
layout: page
order: 6
title: Data Visualisation and AI
parent: Introduction to Data Visualisation
eleventyComputed:
  eleventyNavigation:
    key: "{{ title }}"
    parent: "{{ parent }}"
    order: "{{ order }}"
---

# Data Visualisation and AI

With the increasing use of AI within tools such as Tableau and PowerBI, and the increased capability of Large Language Models (LLM) to write code that can both perform data analysis and create visualisations, it is important to consider the role of AI in the data visualisation toolkit. 

Within data science, machine learning is already an integral part of the workflow, but we will not be considering that wider application of AI in this module. Instead, we are focused more on the use of AI as an assistant to creating visualisations of data.

There are many ways that AI can fit into your workflow as a data visualisation practitioner, from using a conversation with an LLM as part of your initial ideation through to having the AI generate code for analysis or even create the visualisation itself. 

However, the really important thing to remember is that while our AI may generate 'correct' code that will successfully run, or a chart that is technically correct, it does not mean that it has produced a good data visualisation. LLMs frequently suffer from visual hallucinations, improper logic, create charts with the wrong visual encoding, and lack the contextual awareness needed to create a truly successful graphic. Thus, while AI can be a useful assistant in the creation of visualisations, it should be seen as just that, an assistant. The real power still lies in the hands of us as data visualisation practitioners, as we are the ones who can perform the critical analysis and reflection needed to successfully create a successful data visualisation.

In addition, AI can suffer from the lack of critical reflection that humans can bring to evaluating data visualisations, so relying on an LLM to review a visualisation and ensure that it is telling the right story in the right way is not reliable. See for instance one of the examples we looked at in the last [analysis activity](examples): 

{% image "src/img/introduction-to-data-visualisation/examples/vis5.png" "Misleading Vis Example" %}
{% image "src/img/introduction-to-data-visualisation/ai-error.png" "AI being wrong" %}

You can see that the AI has not spotted that the change in time scale that we discussed in the last section distorts the reading of the chart and gives a false sense of plateauing, which is not really there, claiming this plateau to be a fact, rather than a visual error. 

So, AI can be a useful tool, but as always it needs the human in the loop to make it really successful.

{% panel "aside" "CMT218 & CMT231" %}
Within these modules, you are free to use AI tools as part of your workflow, because the important part of the module is not that you have the technical skills to build a data visualisation in JavaScript, or R, or PowerBI, or whatever tool you choose to use. Instead, the important part is that (however you create it), the data visualisation is successful in its aim. Thus, it is important to understand the principles that make a data visualisation successful, rather than just how to build one - and it is that task that the AI will struggle with.
{% endpanel %}
