---
layout: single
author_profile: false
excerpt: |
  This project analyzes factors that affect the outcomes of peer review, uses these to improve reviewer selection, develops software that optimizes reviewer assignments, and evaluates the resulting models in the real-world context of a scientific journal, major scientific conferences, and massive open, online courses (MOOCs)
header:
  image: https://upload.wikimedia.org/wikipedia/commons/6/68/ScientificReview.jpg
  caption: "By Center for Scientific Review [2] [Public domain], via Wikimedia Commons"
title: |
 NSF: Optimizing scientific peer review
categories: Funding
---


{% include toc %}

[See in NSF](https://www.nsf.gov/awardsearch/showAward?AWD_ID=1800956){: .btn .btn--primary}

### Investigators
- [Daniel E. Acuña](/about/) (PI)
- [James Evans](https://www.knowledgelab.org/people/detail/james_a_evans/) (Co-PI)
- [Konrad Körding](http://kordinglab.com/people/konrad_kording/index.html) (Co-PI)

### Abstract

Scientific peer review is a central process when deciding who gets published, promoted, or awarded a prize or grant. Consequently, it may have tremendous impact on the career of scientists and the direction of science. Several researchers, however, have shown that scientific peer review can be slow and low-quality. Moreover, some studies have quantified peer review biases - e.g., prejudices against certain ideas - and inconsistencies - e.g., the same work receiving widely different opinions from different groups of peers. These problems delay or sometimes truncate the dissemination of important research, affecting technological development and ultimately the economy. This project analyzes factors that affect the outcomes of peer review, uses these to improve reviewer selection, develops software that optimizes reviewer assignments, and evaluates the resulting models in the real-world context of a scientific journal, major scientific conferences, and massive open, online courses (MOOCs). By the end of this project, the scientific community will have a better understanding of the factors that affect peer review and actionable insights to make peer review better.

The first component of this project quantifies problems in bias, variance, timing, and quality of reviews. This includes direct effects (e.g., do they collaborate or cite one another) and indirect effects (e.g., do they contribute to and hopefully self-identify with the same community). The project also identifies bias as a function of personal characteristics of author and reviewer. These aspects include age, gender, and minority status, and their visibility and centrality within the field. The same general approach is used to predict the timing of reviews, including the choice to accept the review task. Lastly, the research uses this feature set to predict the quality of reviews. The result, for a given manuscript, includes prediction for each possible reviewer's biases and decision variance, likelihood and timing to participate in the review process, and ultimate review quality. The second component of this project researches and develops techniques to estimate the characteristics of potential reviewers and uses those inferred characteristics to propose, for any given manuscript, a review panel. The techniques optimize the expected value for a cost function that balances the three objectives of reviewer choice variance (bias and covariance), review timing, and review quality. Presumably, this involves suggesting panels comprised of reviewers with complementary expertise and potentially career stage, who understand the topic and are interested in the manuscripts contents. The project allows the option of making these recommendations conditional on the background, characteristics and position of the editor under consideration. Lastly, the project tests the techniques that automatically assign reviewers and analyzes the output of the process in real world applications. In particular, the project collaborates with a large journal, scientific conferences, and massive open, online course (MOOC) organizations. Through random assignments (current methods versus the project's algorithm), the project evaluates the degree to which the assignment approach produces less reviewer choice variance, faster reviews, and reviews of higher quality. The project creates software and results that can be used by other venues.
