---
layout: single
title: "Experience"
permalink: /experience/
comments: true
author_profile: true
---

### Computer Vision reasearch intern at OriginHealth.ai
{% slider %}
  ![alt text 1](shrikumaran.png)
{% endslider %}

OriginHealth Pte. Ltd. (Singapore) is a startup working to simlify the process of mothers getting their ultrasound scans. Currently we face a critical shortage of radiologists to analyse ultrasound scans , this leads to long waiting times which can lead to delayed interventions in case of any anamolies. To prevent this we worked on automating the task of analysing the scans and giving feedback for the doctor to act upon. I worked on the Computer Vision team which was tasked with finding ways to implement various clinical measurement on the scans. 
### Features implemented
* Developed a kernel based algorithm to remove machine imprints on ultrasound images
  * Most ultrasound images we collected for training our models had various marking from the machine(logos, scales etc.), this greatly hindered our model performace.So, we had to come up with a way to remove this imprints.
  * Did an initial literature study to find exisiting methods used to solve similar problems. Most solutions involved using Discrete Cosine Transforms to remove it, impelemented a DCT based approach but results were'ny good.
  * Implemented my own algorithm by defining my own set of kernels. Passed different combinations of kernels on the image to detect different types of imprints. Replaced imprints with weighted mean of the neighbouring pixels.
* Developed a convex hull based algorithm to detect depressions in the skull
  * A common defect in fetal skulls are presence of deformities in the skull, these may be in the form of depressions or bulges.
  * Developed an algorithm using the concept of convex hull to detect depressions.
* Developed an algorithm to unwrap the skull in fetal scan
  * In a scan image performing operations over the skull region proved to be difficult as we couldn't iterate over the region with ease.
  * To overcome this I implemented a way to unwrap the whole skull region into a rectangular strip over which we can easily iterate and test our measurement algorithms.
* Developed a gradient based algorithm to detect sutures on the skull
  * Sutures are small gaps present between skulls, we had the task to count the number of sutures present in the scan.
  * Used the above unwrapped skull image and calcualted the mean pixel intensity in regular intervals. Intervals which had lesser mean intensity compared to its neighbouring intervals were counted as sutures.

### Summer intern at Alphabt.ai
