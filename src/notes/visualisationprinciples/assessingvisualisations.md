---
layout: page
order: 2
title: Assessing Visualisations
parent: Visualisation Principles
eleventyComputed:
  eleventyNavigation:
    key: "{{ title }}"
    parent: "{{ parent }}"
    order: "{{ order }}"
---

# Assessing Visualisations

Evaluating the efficacy of a data visualisation can be done in a few ways. We can use structured assessment frameworks to determine its quality, clarity, and utility. We can use empirical methods—such as user studies, measuring a viewer's performance and comprehension—or we can apply a subjective, guideline-based personal reflective analysis, which is a highly practical approach for everyday assessment.

The following frameworks and principles provide a systematic way to simply and effectively evaluate visualisations.

### 1. Guided Questioning
A foundational method for assessment is developing and ranking a core set of analytical questions. This process helps clarify what constitutes an effective graphic. Key questions to consider include:
Does the visualisation reveal more insight than a standard data table?
Are the chosen visual encodings appropriate for the data types?
Are there any misrepresentations or distortions of the data?
Is the final product user-friendly?

{% accordion 'Example: Assessing the Effectiveness of a Bar Chart' %}
Here is an example of how we might approach this for a simple bar chart showing monthly sales figures for a company over a year.
Assessing for Insight

Does it reveal more than a table? Yes. A table of 12 numbers is hard to scan for trends, but the bar chart immediately shows the peak sales month (December) and the lowest (February).
Are visual encodings appropriate? Yes. A bar chart is excellent for comparing magnitudes. The height of the bars directly corresponds to the sales value, which is a standard and effective encoding.
Any misrepresentations? Let's assume the y-axis starts at 0. If it started at 50,000, it would be misleading. Assuming a standard baseline, this is likely accurate.
Is it user-friendly? Yes. The bars are vertical, the text is horizontal, and the message is clear.
This quick check suggests it's a good, standard bar chart.

{% endaccordion %}

### 2. The "Friendliness" Heuristic

A significant component of a graphic's success relies on user experience and viewer comprehension. Graphics can generally be categorized by their accessibility:

- Friendly Graphics: Utilize fully spelled-out words, horizontal text that reads naturally, and clear typography. They incorporate small explanatory annotations or call-outs, maintain simplicity to the point of rendering legends unnecessary, and utilize effective colour palettes.
- Unfriendly Graphics: Rely heavily on obscure abbreviations, rotated or scattered text, and lack necessary explanations. They often suffer from "chart junk" that distracts from the core data, utilize overly complex or poorly chosen colours, require large legends, and feature poor typography.

If a visualisation exhibits predominantly "unfriendly" traits, it is highly likely that its data encodings and overall messaging are also ineffective.

### 3. The [Junk Charts Trifecta](https://www.junkcharts.com/junk-charts-trifecta-checkup-the-definitive-guide/) Checkup
Developed by the Junk Charts blog, this framework evaluates the alignment of three core components:
  - The Question: What is the specific purpose of the visualisation, and is it clearly answerable?
  - The Data: What story or facts do the underlying data reveal?
  - The Visual: What message does the chart actually convey to the viewer?
A successful visualisation aligns all three elements seamlessly; the chart should accurately reflect the data to answer the primary question.

### 4. Prescriptive Checklists
For a more granular evaluation of layout and presentation, tools like the [Data Visualization Checklist](https://stephanieevergreen.com/data-visualization-checklist/) (developed by Stephanie Evergreen and Ann K. Emery) offer a rigid but effective methodology. This checklist provides a fast, standardized way to score the formatting and communicative power of a graphic.

### 5. Usability Heuristics

To perform evaluations without recruiting large user panels, evaluators use specialised heuristic sets. Building upon Jakob Nielsen’s general interface principles, Camilla Forsell and Jimmy Johansson derived a consolidated set of 10 Usability Heuristics specifically validated for Information Visualization systems ([Forsell & Johansson, 2010](https://doi.org/10.1145/1842993.1843029)):

  1. **Information Coding**: Visual marks and spatial channels must accurately and intuitively map to underlying data attributes.
  2. **Minimalist Design**: Non-essential visual elements that do not support data interpretation must be minimized.
  3. **Flexibility and Efficiency**: The interface must support both novice spatial exploration and accelerated expert workflows.
  4. **Consistency and Standards**: Visual idioms, color conventions, and interaction behaviors must remain uniform across all views.
  5. **Spatial Organization**: Visual elements and visual marks must be arranged logically to leverage human spatial reasoning.
  6. **Visibility of System State**: Interactive filtering, semantic zooming, and data queries must offer immediate visual feedback.
  7. **Orientation and Awareness**: Multi-view or zoomed interfaces must preserve contextual awareness to prevent user disorientation.
  8. **Structured Actions**: Complex analytical workflows must be broken into logical, step-by-step interactive stages.
  9. **Remove Redundancy**: Redundant visual encodings should be eliminated unless deliberately used to reinforce critical signals.
  10. **Error Prevention and Recovery**: Interactive controls must prevent invalid data states and allow seamless visual state undoing.
    

However, Sheelagh Carpendale provides critical qualifications regarding heuristic inspections, noting that relying exclusively on pre-defined heuristic rules can stifle creative design innovation and fail to evaluate subjective aesthetic qualities, narrative flow, or deep domain-specific insights ([Carpendale, 2008](https://doi.org/10.1007/978-3-540-70956-5_2)). Heuristic evaluations should therefore be combined with empirical user evaluations rather than used in isolation.


## Further Reading and Sources
Developing a strong subjective eye for data visualisation requires consistent practice and exposure to expert critiques. The following resources regularly deconstruct the successes and failures of real-world graphics:

  - [Financial Times (FT) Chart Doctor](https://www.ft.com/chart-doctor): A dedicated series by the FT data journalism team analyzing both in-house visualisations and those published elsewhere.
  - [Visualising Data](https://visualisingdata.com/the-little-of-visualisation-design/): The Little of Visualisation Design: A recurring series by Andy Kirk that highlights the micro-level design choices—both good and bad—that impact a graphic's effectiveness.

{% panel "prompt" "Assessing Visualisations" %}
Now it's time to think about how you assess visualisations personally. If you come across a visualisation for the first time, how do you approach it? Is there anything you specifically look at/for first? How do you decide whether it's a 'good' visualisation worth looking at further?

{% endpanel %}

