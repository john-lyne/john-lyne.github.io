---
title: "Unsupervised learning for turbulent structure identification"
excerpt: "Clustering dynamically salient regions of channel flow turbulence <br/><img src='/images/vortex.PNG'>"
collection: portfolio
---

Research pertaining to the study of coherent structures in turbulent flows has long involved using arbitrary thresholds to elucidate regions of interest. This normally involves modifying the threshold value of a specific flow quantity until the structures relevant to that flow quantity fit perceptual expectations. The process can be thought of as twisting a knob until things look right, which inherently involves some level of subjective decision making.

While this approach is suitable for gaining general insights on the flow (i.e visualize vortex clusters to see where the flow is most energetic), to further analyze these regions you would have to rationalize as to how a specific threshold value was chosen. In the literature, I've commonly seen arbitrary values to highlight high/low speed regions via a 10%/-10% velocity threshold. Thresholds for vorticity metrics (such as Q-criterion) normally vary from study to study. This makes detailed analyses of the visualized structures challenging, as one would have to rationalize why the selected threshold value was chosen.

This study addresses the aforementioned issues by using a machine learning framework that automatically organizes flow into clusters in an unsupervised fashion. The boundaries of the identified structures are not bound to a subjective value, instead these boundaries are automatically learned based on computational pattern recognition.

