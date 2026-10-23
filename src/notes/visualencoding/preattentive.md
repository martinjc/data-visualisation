---
layout: page
order: 4
title: Preattentive Processing
parent: Visual Encoding and Perception
eleventyComputed:
  eleventyNavigation:
    key: "{{ title }}"
    parent: "{{ parent }}"
    order: "{{ order }}"
---

**Preattentive Processing** refers to the automatic way in which our visual system processes information that is not the focus of our attention. This processing happens unconsciously and very quickly (in the order of milliseconds), and it is based on a set of hardwired rules and biases. For example, the human visual system is particularly good at detecting certain visual properties, such as color, shape, and orientation, and it can do so even when there are many other visual elements present. Items selected for pre-attentive processing are then raised higher in consciousness for attentive processing.

Basic features that trigger fast detection include:

- Color / Hue / Intensity: Bright colours, high-contrast items, or unique shades stand out immediately among uniform hues (e.g., a red circle among blue circles).
- Form & Shape: Differences in line length, size, curvature, and spatial closure.
- Orientation & Motion: Lines tilted at a different angle or objects exhibiting flicker/motion.
- Spatial Positioning & Grouping: Proximity, similarity, and spatial arrangement.

{% gallery %}

{% galleryslide "src/img/visual-encoding/preattentive_01_color.gif", "Feature 1: Colour (Hue) - Pre-Attentive Pop-Out" %}

When a single data mark changes in hue against a uniform field of distractors, detection occurs almost instantaneously (<200 ms) in early visual cortex processing.

- **Visual Channel:** Hue / Chromatic Contrast
- **Perceptual Effect:** Pre-attentive pop-out occurs prior to conscious eye movement. Search time remains flat regardless of set size.
- **Visualisation Takeaway:** Use selective colour highlighting sparingly to direct viewer focus immediately to the core narrative or key metric.
{% endgalleryslide %}

{% galleryslide "src/img/visual-encoding/preattentive_02_orientation.gif", "Feature 2: Orientation (Angle) - Pre-Attentive Pop-Out" %}

All needles initially share an identical vertical posture ($0^\circ$). When a solitary mark tilts to $45^\circ$, the orientation disparity triggers instant pop-out across the visual field.

- **Visual Channel:** Orientation / Angle / Tilt
- **Perceptual Effect:** A small angular difference breaks visual uniformity instantly.
- **Visualisation Takeaway:** Effective for flow fields, directional indicators, vector plots, and scatterplot trend markers.
{% endgalleryslide %}

{% galleryslide "src/img/visual-encoding/preattentive_03_size.gif", "Feature 3: Size (Scale / Area) - Pre-Attentive Pop-Out" %}

All circles begin with uniform radius ($10\,\text{px}$). When one mark expands to $22\,\text{px}$, the scale discrepancy creates an unmissable focal point.

- **Visual Channel:** Size / Diameter / Area
- **Perceptual Effect:** A small difference in size breaks visual uniformity instantly.
- **Visualisation Takeaway:** Naturally suited for quantitative magnitude encoding (e.g., bubble charts, proportional symbol maps, graduated scatter points).
{% endgalleryslide %}

{% galleryslide "src/img/visual-encoding/preattentive_04_shape.gif", "Feature 4: Shape (Form / Curvature) - Pre-Attentive Pop-Out" %}

All marks begin as smooth circles. When one mark transitions into a sharp angular diamond, the boundary curvature and vertex discontinuity produce immediate pop-out.

- **Visual Channel:** Shape / Form / Boundary Curvature
- **Perceptual Effect:** Curvature disparity and sharp vertex presence are extracted across the entire field in parallel.
- **Visualisation Takeaway:** Ideal for categorical differentiation on scatterplots where colour is already committed to another data dimension.
{% endgalleryslide %}

{% galleryslide "src/img/visual-encoding/preattentive_05_motion.gif", "Feature 5: Motion (Temporal Modulation) - Pre-Attentive Pop-Out" %}

Against a static array of marks, a single mark begins oscillating horizontally. Motion is the most potent and involuntary pre-attentive trigger in human perception.

- **Visual Channel:** Motion / Oscillation / Flicker
- **Perceptual Effect:** Motion commands immediate, reflexive attentional capture, overriding surrounding static features.
- **Visualisation Takeaway:** Use only for alerts or interactive state changes - when many items are moving, the effect is lost.
{% endgalleryslide %}

{% galleryslide "src/img/visual-encoding/preattentive_06_conjunction_color_shape.gif", "Feature Conjunction: Colour + Shape - Serial Search Breakdown" %}

Demonstrating Anne Treisman's Feature Integration Theory: the target (Red Circle) is placed among distractors consisting of Blue Circles and Red Squares. Pop-out completely breaks down.

- **Target Mark:** Red Circle
- **Why Pop-Out Fails:** "Redness" is shared with the squares, and "circularity" is shared with the blue dots. Neither channel alone isolates the target.
- **Visualisation Takeaway:** Avoid encoding multiple overlapping categorical dimensions with shared visual features; readers are forced into slow, item-by-item scanning.

{% endgalleryslide %}

{% galleryslide "src/img/visual-encoding/preattentive_07_conjunction_color_orientation.gif", "Feature Conjunction: Colour + Orientation - Serial Search Breakdown" %}

The target (Vertical Red line) is surrounded by Vertical Blue lines and Horizontal Red lines. Because orientation and hue are distributed across both distractor groups, pre-attentive detection fails.

- **Target Mark:** Vertical Red line ($0^\circ$)
- **Why Pop-Out Fails:** Confirms that conjunction search failure is universal across feature modalities.
- **Visualisation Takeaway:** Multi-attribute visual encodings require careful spatial grouping or direct labelling to prevent cognitive search fatigue.
{% endgalleryslide %}

{% endgallery %}

This concept of preattentive processing clearly ties back in to our earlier consideration of Gestalt psychology and our ability to automatically group items or build up a big picture from smaller parts, often before we consciously focus on individual elements. 

These tricks are also very useful for guiding the reader's attention to particular parts of a visualisation. It is not just data visualisation that takes advantage of these features - they are also used in graphic design, marketing and so on. 

A more in-depth look at preattentive processing is given in [Perception in Visualization](https://www.csc2.ncsu.edu/faculty/healey/PP/) by Christopher G Healey, which also includes a nice practical experiment allowing you to test how well colour and shape affect preattentive processing, along with examples evidencing preattentive processing at work.



