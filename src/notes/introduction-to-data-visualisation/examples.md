---
layout: page
order: 5
title: Looking at Visualisations
parent: Introduction to Data Visualisation
eleventyComputed:
  eleventyNavigation:
    key: "{{ title }}"
    parent: "{{ parent }}"
    order: "{{ order }}"
---

# Activity: Assessing Visualisations

We've started to think about the whys and hows of data visualisation, and in the last section we started to think about a specific visualisation in terms of what it means to us, how we can read it, how we might think about the purpose of a visualisation, and how that relates to it's success as a graphic. 

We're going to expand on that now by looking at a few more visualisations, and asking ourselves to examine the issues present within those visualisations and attempting to decide whether they are what could be considered 'good' or 'bad'. Later on we'll consider more formal methods and frameworks for evaluating visualisations, but for now we'll be asking you to use whatever knowledge you already have, along with your own thoughts and experiences.

{% panel "prompt" "Starting to assess Visualisations"%}
For each of these visualisations below, take a moment to look at the visualisation and decide whether you consider it a 'good' visualisation or a 'bad' visualisation. Then, take a moment to think about why you've made that decision. Don't worry if you're not sure, as we'll be spending a lot of time doing this sort of activity as we go through the module, and the more we look at visualisation theory and principles, the easier this sort of task will become. Try to assess based only on the visualisation itself, without looking at other context or information. Below each visualisation you'll find some further information to consider. Look at this once you've formed your own thoughts and ideas, and then you can see how well your thoughts match the evaluation provided. Again, don't worry if you disagree or have not spotted all the things mentioned in the evaluation.
{% endpanel %}


{% gallery "Visualisation Examples" %}

{% galleryslide "src/img/introduction-to-data-visualisation/examples/vis1.png", "Sleep Cycles" "A visualisation of sleep cycles by [Andrew Elliott](https://www.reddit.com/r/dataisbeautiful/comments/5l39mu/my_daughters_sleeping_patterns_for_the_first_4/)" %}

{% accordion "Evaluation"%}
This is a fun one to start with, because it is very nice to look at, or aesthetically pleasing, but is actually relatively difficult to understand as the amount of information presented alongside the visualisation is minimal. In fact, we can really only discover what it is about by reading the original Reddit thread it comes from, which, as we will see later, is something that a 'good' visualisation should not require. In this instance, the visualisation presents sleep data from the author's child, with awake phases represented in one colour, and sleep phases in another. Each ring on the circle represents a single day, so each ring represents 24 hours. With this knowledge we can start to pick out patterns in the child's sleep, and observe how it changes over time, so the visualisation starts to become more usable - however presented as it is with no legend and context it's merit is purely aesthetic, rather than informational. 

There is also a problem with this visualisation, in that the data representation is not consistent. Each ring on the circle represents a single day, or 24 hours. However, the circumference of each ring is not the same, so an hour on the outer ring is represented by far more pixels than an hour on the inner ring. This means that time is not represented consistently across the visualisation, and so the work required to interpret the visualisation is increased as we can not easily compare days with one another. We also experience this distortion as it gives increased prominence to the phases towards the outer edge of the circle, a phase that might only be an hour long on the outer edge is given a similar visual prominence to a phase that is three hours long further in, which can lead to a misleading interpretation of the data.
{% endaccordion %}
{% endgalleryslide %}

{% galleryslide "src/img/introduction-to-data-visualisation/examples/vis2.png", "Gun Deaths in Florida" "Gun Deaths in Florida - C Chan - Reuters - 2014" %}

{% accordion "Evaluation"%}

On the face of it, compared to the previous graphic, this looks like a good visualisation. The context is presented alongside the data, we have information on what the data is showing in both the title and subtitle, the axes are labelled and an annotation draws our attention to a key point. 

However, there is a problem here in that a quick surface reading of the visualisation leads us to the conclusion that gun deaths in Florida decreased after the enactment of the 'Stand your Ground' law. This is because our general understanding is that if a line goes down on a graph, the value of the data must be decreasing. In this graphic however, we note that the y-axis is inverted, and as such the visualisation is actually showing the opposite. So, the data is actually showing us the opposite - gun deaths in Florida increased after the law was enacted. However we have to pay attention to the graphic to spot this. 

The use of the 'blood red' colour is a strong statement for a visualisation, and we'll look at colour associations and some of the benefits and disadvantages of these later in the module.

So, is this an intentionally misleading graphic, or just a misguided attempt to present data in a particular way  that has been let down by some of the details?  There's a really nice [deep dive on this visualisation](https://medium.com/@nigelmills2000/the-truth-and-lies-behind-the-infamous-blood-graph-f6d6691c3626) that discusses this, and brings in the original graphic that this is potentially attempting to replicate.
{% endaccordion %}
{% endgalleryslide %}


{% galleryslide "src/img/introduction-to-data-visualisation/examples/vis3.png", "Bute Park Visitors" "Cardiff Council report on Bute Park visitors ~2014" %}

{% accordion "Evaluation"%}
This one I love because it's a really good example of how hard data visualisation is to get right, because there is *nothing* right in this visualisation. 3D exploded Pie Chart? Terrible. Misleading or hard to understand legend? Awful. Wrong choice of chart entirely? Absolutely wrong. 

Look, I'm not going to tell you that Pie Charts are always bad. We'll look at an argument in the next section that discusses the rights and wrongs of Pie Charts, and lays out some scenarios where Pie Charts are the right choice. But this is not one of those scenarios. Pie Charts are for "part of whole" comparisons, where we have 100% of something and we're looking to compare the relative size of the different parts, and where we have appropriate numbers of parts of appropriate sizes to compare. I'm not convinced, given the labelling, that we have 100% of the people interviewed here and we're showing how that 100% is made up, because that would indicate that we have people on their own who are neither adults or children, and it worries me as to who they are in that case. 

On top of that, the three dimensional effect and the 'explosion' of the pie chart further distort the data by giving prominence to the slices at the front of the diagram, and reducing the visual salience of the other slices. So, having picked the wrong type of visualisation in the first place, the errors are compounded by then picking the worst implementation of the wrong type of visualisation.

I don't blame whoever at the council made this. I blame Microsoft Excel. But seriously, this is why the most important skill you can develop as a data visualisation practitioner is the self-reflective critical eye that allows you to look at your own work and ask 'is this right, and is it good?'. Because then when you make stuff like this you can very quickly realise the answers are 'no' and 'no', and pivot to making two separate bar charts instead.
{% endaccordion %}
{% endgalleryslide %}


{% galleryslide "src/img/introduction-to-data-visualisation/examples/vis4.png", "Age of Death and Musical Genre" "[Age of Death and Musical Genre](https://theconversation.com/music-to-die-for-how-genre-affects-popular-musicians-life-expectancy-36660)" %}

{% accordion "Evaluation"%}
Oh my. This one is another fun one. Again, as with 2nd example, on the face of it all seems okay. We have a title, a subtitle, clear axes labelling. The data is readable, and unlike the 2nd example we've not inverted any axes or used any other tricks to present the data in a misleading way.

However, go a little deeper, and we start to notice some issues.

Firstly, lets take the lighter lines represeting US Male and Female life expectancy. These lines slowly increase across the graphic, which matches with our understanding that in general, barring some occasional dips, life expectancy has increased over the past century or so. However, what period does this actually cover? There is no axis representing time. As such we are left guessing that this is indeed presenting life expectancy for the US over a period of time, but we can't be sure - and any time we are unsure when we're reading a graphic we have a problem, and it indicates that the graphic needs further work.

However, there's a couple of bigger issues here. We have average age of death of male and female musicians from different genres plotted as another line graph. Line graphs are absolutely the right choice for presenting the life expectancy over time, but absolutely the wrong choice for representing the average age of death of musicians from different genres, as that data is discrete, not continuous. Bars or another type of data representation would be more appropriate here, as we're almost suggesting that music genres lie on a linear spectrum, and the line we draw between them has some meaning, which it doesn't. (I'm completely with you - music genres definitely are a spectrum, and they overlap and intertwine and could almost certainly be represented as a four dimensional hypercube if we can calculate where folk-punk begins and alt-country ends.... but that's another module entirely.)

Then we have a potentially even larger problem, and it's not necessarily with the visualisation alone, but with the data itself. This graphic tells us the story that the average age of death for artists in Rap and Hip-Hop is much lower than the average age of death in Blues and Jazz. Okay. Except ... Rap and Hip-Hop have only existed as genres for around 50 years (40 years at the time the graphic was made), while Jazz and Blues have existed for over 100 years. Any Rap/Hip-Hop artists who have died already have likely died un-naturally young, as the genre has not existed long enough for the artists in the genre to live full lives and die of natural causes at an old age. The data suffers from survivorship bias, or right censoring, in that the data for the later genres is not as complete as the data for the genres that have been around longer, and therefore comparison is much more difficult to do.

This examples teaches us a few things then. As with the earlier examples, the choice of visualisation type must match the type of data you're presenting, and the message you are trying to get across. It's not enough to say 'if something has a title and axes that are correct, it must be good'. And finally, we must be able to trust our data, and be sure that our data is saying what we think it is.

Again, there's another [good look at this visualisation that is worth reading](https://callingbullshit.org/case_studies/case_study_musician_mortality.html), and this one includes a rebuttal to the criticisms from the original author.

{% endaccordion %}
{% endgalleryslide %}

{% galleryslide "src/img/introduction-to-data-visualisation/examples/vis5.png", "Global Carbon Emissions from Fossil Fuels" "Global Carbon Emissions from Fossil Fuels from the [Gates Newsletter](https://www.gatesnotes.com/2016-Annual-Letter?WT.mc_id=02_22_2016_00_AL2016_GL-GN_&WT.tsrc=GLGN)." %}

{% accordion "Evaluation"%}
A line chart to show continuous change over time. Title present, axes labelling. Source of data noted. Simple colour choices. Annotation on the line giving some key information. On the face of it, this is a good chart.

Except ... what's going on there with the horizontal axis? We're looking at changes over time, and we start going in 20 year increments up until 1990, then jump 21 years, then start going in yearly increments! So what looks like a steep increase followed by a levelling off is anything but... it's just that the the final third of the graph shows as long a time period as a quarter of one of the previous 8 time periods. 

Again, this points to consistency of data representation and the distortion and misleading that occurs when we ignore consistency.

Interestingly, humans aren't the only ones that can be misled by this, as we'll see in the next session. 

{% endaccordion %}
{% endgalleryslide %}


{% galleryslide "src/img/introduction-to-data-visualisation/examples/vis8.png", "Google Trends - Solar Eclipse" "Solar Eclipse - [Oh my Eyes Hurt](https://www.reddit.com/r/dataisbeautiful/comments/6v8a9m/oc_my_eyes_hurt/)" %}

{% accordion "Evaluation"%}
Again, on the face of it, all the elements are present and correct here, and we're given a line chart that gives us a funny representation of data - look at the silly people staring at the sun and googling 'my eyes hurt'.

Except that's not how google trends works - these two lines are actually on completely different scales - Google trends just shows you '100' as the max level for that search in that time period, and scaled everything else appropriately. So this chart could be showing us all 8.6 million people in New York City googling for 'solar eclipse' between 11 and 3, with the peak at 2:30, and just 10 people in googling for 'my eyes hurt' a little later at 3pm - but the presentation makes it look like they both had the same level of interest.

Again, not necessarily Google's fault - but perhaps not the best way to represent the relative interest in these two search terms. 

{% endaccordion %}
{% endgalleryslide %}


{% galleryslide "src/img/introduction-to-data-visualisation/examples/vis9.png", "Average Male Height" "[Looking Down on the Rest of the World](https://stuffdutchpeoplelike.com/2011/10/30/tall-dutch-people/)" %}

{% accordion "Evaluation"%}
Where to start with this one? Let's start with the racism. There's no way to spin it - using simplified cultural stereotypes to represent different nationalities is racist and unacceptable. It might look like 'fun charicatures' but it's offensive and there's no place for it in a professional data visualisation. You can use fun characters by all means, data visualisation does not have to always be a serious place (and I'm happier when it's not) but this is just plain wrong.

Then we get into the technical error with the axis scaling. As with 'pie charts are bad' there are plenty of people who'll tell you that one of the clearest and hardest rules in data visualisation is that 'the y-axis must always start at 0'. However, as with pie charts, this is not always true, and there are plenty of scenarios where a y-axis starting at something other than 0 is entirely appropriate. We saw two in the earlier example about life expectancy and age of death - that visualisation had 99 problems, but an axis that didn't start at zero wasn't one (did you see what I did there?). However, in this case (and in all cases where we're using the height of a bar or anything that is acting like a bar to represent our data) it absolutely **needs** to start at 0. As it is, this chart is suggesting that dutch men are **three** times as tall as men from the Phillipines, and that just. isn't. true. The actual difference in height is a little more than 20cm, so both figures should be approximately the same size on the scale, but by not extending our y-axis down to 0 we are drastically distorting the difference.

So, let's not do that?
{% endaccordion %}
{% endgalleryslide %}


{% galleryslide "src/img/introduction-to-data-visualisation/examples/vis10.png", "Amazon's Growth" "In charts: how US retailers fared as Amazon powered ahead – Financial Times ([November 2017](https://www.ft.com/content/d17a1da8-cf08-11e7-b781-794ce08b24dc?syn-25a6b1a6=1))" %}

{% accordion "Evaluation"%}
You know who makes good charts? The Financial Times makes good charts. Often they're quite complex, but that's fine because their audience can read them. They know what they're doing and who they're making visualisations for, and that means they can make things like this, where they want to get a message across and the do it with a minimum of fuss, presenting all the context and information we need to read and  understand the visualisation. 

Good work FT.
{% endaccordion %}
{% endgalleryslide %}


{% galleryslide "src/img/introduction-to-data-visualisation/examples/vis12.png", "Federica Fragapane for La Lettura" "[Federica Fragapane for La Lettura](https://www.domestika.org/en/projects/1232340-data-visualizations-for-la-lettura-corriere-della-sera)" %}

{% accordion "Evaluation"%}
This is an interesting example, because it starts to bring in some more of the tradeoff that we've already thought about briefly between aesthetics and simplicity.
{% endaccordion %}
{% endgalleryslide %}



{% galleryslide "src/img/introduction-to-data-visualisation/examples/vis15.png", "OpenSignal Android Fragmentation Report" "OpenSignal Android Fragmentation Report" %}

{% accordion "Evaluation"%}

{% endaccordion %}
{% endgalleryslide %}


{% galleryslide "src/img/introduction-to-data-visualisation/examples/vis17.png", "US Immigration - National Geographic" "US Immigration - [National Geographic](https://www.nationalgeographic.com/culture/graphics/graphic-united-states-immigration-origins-rings-tree-culture)" %}

{% accordion "Evaluation"%}

{% endaccordion %}
{% endgalleryslide %}


{% galleryslide "src/img/introduction-to-data-visualisation/examples/vis18.png", "Literacy Rates" "Female and Male Literacy Rates - [Information is Beautiful](https://informationisbeautiful.net/beautifulnews/86-literacy-rates-equal/)" %}

{% accordion "Evaluation"%}

{% endaccordion %}
{% endgalleryslide %}


{% galleryslide "src/img/introduction-to-data-visualisation/examples/vis19.png", "Military Expenditure" "Top Six Countries by Military Expenditure - [St Louis Fed](https://www.stlouisfed.org/on-the-economy/2023/jan/military-expenditures-how-top-spending-nations-compare)" %}

{% accordion "Evaluation"%}

{% endaccordion %}
{% endgalleryslide %}


{% endgallery %}



