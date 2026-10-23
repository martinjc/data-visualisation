---
layout: page
order: 3
title: Minimalism, Embellishment and Humanism
parent: Visualisation Principles
eleventyComputed:
  eleventyNavigation:
    key: "{{ title }}"
    parent: "{{ parent }}"
    order: "{{ order }}"
---


## Minimalism, Embellishment and Humanism

As we are considering assessing visualisations, we can start to consider one of the key tradeoffs within data visualisation, around the level of visual embellishment that is 'correct' for a data visualisation. 

Edward Tufte's classical visual doctrine centers on maximizing the **Data-Ink Ratio** — the proportion of ink devoted to the non-redundant display of data information - while ruthlessly eliminating non-essential visual elements, termed **Chartjunk** ([Tufte, 1983](https://www.edwardtufte.com/book/the-visual-display-of-quantitative-information/)). Tuftean minimalism assumes that visual clarity is strictly synonymous with sparse visual ink, and that this aids rapid understanding of data.

The process of moving from excess 'Early 90's Excel' style graphic to a more minimalist approach is shown in the gallery below.

{% gallery %}

{% galleryslide "src/img/visualisation-principles/step_00.png", "Step 0 - Initial version with chartjunk" %}

Heavy textured linen background, bevelled & embossed 3D bars, random rainbow coloring, redundant legends, thick borders, and clumsy database column labels overwhelm the chart. Over 85% of ink conveys zero data.

- **Data-to-Ink Ratio:** 14%
- **Chartjunk Erased:** 0%
- **Key Issues:** Heavy linen texture, 3D bevels, bar drop shadows, thick black borders, 10-player redundant legend, database field titles (`batsman_unique_id_name`, `total_career_runs_ipl`).
{% endgalleryslide %}

{% galleryslide "src/img/visualisation-principles/step_01.png", "Step 1 - Remove Outer Background & Frame" %}


We strip away the texture and heavy outer drop-shadow box. The chart starts to feel lighter.

- **Data-to-Ink Ratio:** 21%
- **Chartjunk Erased:** 15%
- **Changes:** Erased heavy linen texture background from canvas; removed outer container bevel and deep drop shadow.

{% endgalleryslide %}

{% galleryslide "src/img/visualisation-principles/step_02.png", "Step 2 - Remove Inner Plot Background" %}


We remove the secondary gradient background directly behind the bars. The plot area becomes clean, improving contrast with the data marks.

- **Data-to-Ink Ratio:** 28%
- **Chartjunk Erased:** 27%
- **Changes:** Erased dark gradient fill inside the chart area; eliminated inner bevel emboss around the plot boundary.

{% endgalleryslide %}

{% galleryslide "src/img/visualisation-principles/step_03.png", "Step 3 - Remove Chart Border & Perimeter Box" %}


The chart perimeter was boxed in a heavy dark rectangle. Caging data marks in boxes does nothing to aid comprehension so we can remove it.

- **Data-to-Ink Ratio:** 36%
- **Chartjunk Erased:** 38%
- **Changes:** Removed thick outer rectangular boundary line and plot container box shadow.

{% endgalleryslide %}

{% galleryslide "src/img/visualisation-principles/step_04.png", "Step 4 - Flatten 3D Bevels & Drop Shadows" %}


3D extrusion and specular shiny lighting on flat 2D bars is chartjunk. It distorts the perception of data.

- **Data-to-Ink Ratio:** 46%
- **Chartjunk Erased:** 49%
- **Changes:** Stripped 3D bevel and lighting filters; erased drop shadows beneath each bar. Bars flattened to accurate rectangles.

{% endgalleryslide %}

{% galleryslide "src/img/visualisation-principles/step_05.png", "Step 5 - Remove Heavy Bar Outlines" %}


With thick borders around each bar, an ambiguous question arises: Does David Warner's run total include the 3px stroke or not? Removing outlines clarifies endpoints.

- **Data-to-Ink Ratio:** 55%
- **Chartjunk Erased:** 58%
- **Changes:** Removed 3px black stroke around each bar; bar length now corresponds cleanly to numeric runs without optical edge ambiguity.

{% endgalleryslide %}

{% galleryslide "src/img/visualisation-principles/step_06.png", "Step 6 - Remove Redundant Color Legend" %}


The legend on the right repeats the exact player names already displayed on the category axis. It wastes valuable horizontal space and forces fans to bounce back and forth.

- **Data-to-Ink Ratio:** 64%
- **Chartjunk Erased:** 68%
- **Changes:** Eliminated redundant 10-player color legend box; expanded horizontal chart space for better run resolution.

{% endgalleryslide %}

{% galleryslide "src/img/visualisation-principles/step_07.png", "Step 7 - Clean Verbose Axis Titles & Units" %}


Raw database column names like `batsman_unique_id_name` and `total_career_runs_ipl` are stripped. The measurement unit (Runs) is cleanly stated once in the header context.

- **Data-to-Ink Ratio:** 73%
- **Chartjunk Erased:** 77%
- **Changes:** Erased database field names; simplified tick marks from '2,000 runs' to clean '2,000'; placed measurement context cleanly in the subtitle.

{% endgalleryslide %}

{% galleryslide "src/img/visualisation-principles/step_08.png", "Step 8 - Focus Colors (Semantic Highlighting)" %}


Random rainbow colors act as distraction and do not add to understanding. We shift overseas players (David Warner, AB de Villiers, Chris Gayle) to calm neutral slate and use intentional blue to highlight domestic players who dominate 7 of the top 10.

- **Data-to-Ink Ratio:** 82%
- **Chartjunk Erased:** 85%
- **Changes:** Replaced 10 conflicting rainbow hues with cohesive palette; overseas players set to muted neutral slate; Indian domestic players highlighted with deliberate pre-attentive blue.

{% endgalleryslide %}

{% galleryslide "src/img/visualisation-principles/step_09.png", "Step 9 - Lighten Non-Data Ink & Soft Hairlines" %}


We un-bold the aggressive 90s typography, remove text drop shadows, and soften heavy gridlines into ultra-faint hairline guides. Non-data elements retreat to the background.

- **Data-to-Ink Ratio:** 89%
- **Chartjunk Erased:** 92%
- **Changes:** Reduced font weights from heavy bold to readable regular weight; erased text drop shadows; heavy dark gridlines converted to ultra-faint hairline guides.

{% endgalleryslide %}

{% galleryslide "src/img/visualisation-principles/step_10.png", "Step 10 - Direct Labeling & The Tufte Minimalist Chart" %}


Direct labels are placed at the end of every bar (8,004 runs, 6,769 runs...), eliminating eye scanning guesswork. With direct labels in place, the X-axis line and tick marks become redundant and are completely removed.

- **Data-to-Ink Ratio:** 95%
- **Chartjunk Erased:** 100%
- **Changes:** Direct values labeled right beside each bar for instant reading; eliminated entire X-axis line and tick numbers; gridlines removed as bar lengths are their own measurement. Peak Data-to-Ink ratio achieved!

{% endgalleryslide %}

{% endgallery %}

However, as we have already mentioned, empirical research exists that challenges the validity of this minimalist viewpoint. Comparative studies by [Bateman et al. (2010)](https://doi.org/10.1145/1753326.1753716) revealed that **visual embellishments** ("useful junk") do not impair task interpretation speed or visual accuracy when compared to plain minimalist charts. Crucially, the presence of visual embellishments enhanced long-term chart memorability and message recall among viewers when re-tested after multi-week delays. This work looked at examples of embellished charts like the one below, created by Nigel Holmes, who [talks more here](https://www.johngrimwade.com/blog/2016/10/03/nigel-holmes-on-humor/) about his approach to adding visual interest within visualisations.

{%image  "src/img/visualisation-principles/holmes.jpg", "a chart by Nigel Holmes" "An embellished chart example by Nigel Holmes, originally published in Time magazine" %}

Work by [Borkin et al. (2013)](https://doi.org/10.1109/TVCG.2013.234) further refines our understanding of **chart m    emorability** through large-scale eye-tracking studies and memory recognition tasks, concluding that visual features traditionally condemned by minimalist purists—such as pictorial icons, custom visual palettes, high visual density, and non-standard chart layouts—are precisely the components that trigger human **visual salience** and consolidate memory structures. This leads to an understanding that actually different levels of visual embellishment may have benefits and disadvantages for different audiences; minimalist designs minimise initial processing friction for expert analysts conducting rapid data lookup, whereas visual diversity and embellishment foster engagement and long-term recall in public communication contexts.

### Data Humanism

Giorgia Lupi's **Data Humanism Manifesto** ([Lupi, 2017](https://giorgialupi.com/data-humanism-my-manifesto-for-a-new-data-wold)) introduces a philosophical shift away from traditional engineering-centric visualization guidelines such as the minimalist approach. Data Humanism directly critiques the assumption that data is an objective, emotionless mirror of reality. Instead, Lupi posits that data is inherently intertwined with human experience and context, emphasizing that behind every dataset lies a human story. Lupi's approach advocates for visualizations that celebrate the complexity and richness of data, often incorporating artistic, unconventional, and narrative-driven elements to foster a deeper, more intuitive connection between people and information. This perspective underscores the importance of ethical storytelling, where designers use data not just to inform, but to inspire curiosity, empathy, and meaningful engagement with the world around us - this approach clearly invites further embellsishment of graphics and perhaps a softer, more aesthetic and human approach to visualisation design.

{% image "src/img/visualisation-principles/giorgia_lupi.webp", "a visualisation" "[Humanistic data visualisation](https://giorgialupi.com/data-humanism-my-manifesto-for-a-new-data-wold) - Giorgia Lupi and Stefanie Posavec, [Dear Data](https://www.dear-data.com/) " %}

Linking in with some of the thoughts around Visualisation Rhetoric, Data Humanism promotes treating datasets as contextual, qualitative, and human-collected artifacts rather than absolute objective truths, understanding the subjective human element within data and the choices and decisions that have been made in the collection, preparation, and presentation of the data.    
It suggest we **Embrace Nuanced Complexity**, rejecting oversimplified visual summaries in favor of rich, multi-layered visual narratives that honor complex human experiences, and quite often utilise elements such as **hand-drawn elements**, **customised visual metaphors**, and **personal data tracking** to bridge the emotional distance between the viewer and the underlying subjects.

{% panel "info", "Summary" %}

Ultimately, each of these visualisation approaches has its use, and understanding where and when each approach might be most appropriate is an important skill for the data visualisation practitioner to develop. More and more we'll see as we go through this module that ultimately the approach depends on the context of the visualisation - what are we trying to show, and who are we trying to show it to? Given the wide range of possible contexts and audiences for data visualisation, it makes sense that there is no single 'best' approach - rather, the 'best' approach will depend on the answers to those questions.

{% endpanel %}