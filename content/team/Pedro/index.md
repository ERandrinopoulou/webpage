---
all_day: true
#authors: []
date: "2019-07-16"
#date_end: "2018-06-12T15:00:00Z"
#event: International Society for Clinical Biostatistics
#event_url: https://example.org
featured: false
# links:
# - icon: twitter
#   icon_pack: fab
#   name: Follow
#   url: https://twitter.com/georgecushen
#location: Leuven, Belgium
# math: true
# projects:
# - internal-project
# publishDate: "2017-01-01T00:00:00Z"
slides: 
summary: "Joint models for recurrent events, terminal event, and longitudinal outcome using the CFF data" 
#tags: []
title: Pedro Afonso
#url_code: ""
#url_pdf: ""
#url_slides: "ISCB_ARAT.pdf"
#url_video: ""
---

Pedro Afonso is a PhD student working on the following projects:

## Efficiently analyzing big data with Bayesian joint models for longitudinal and time-to-event data

Background: Cystic Fibrosis (CF) is a lethal genetic lung disease that requires frequent monitoring. A commonly measured marker of lung function in CF is forced expiratory volume in 1 s of % predicted (FEV1). This sub-study stems from an international workgroup project to establish guidelines for longitudinal analysis of CF FEV1 using the U.S. CF Foundation Patient Registry, which contains health-related information for approximately 30,800 CF patients who collectively contributed 1,215,171 observations and 255,804 years of follow-up. It has been of clinical interest to model the association between FEV1 and time-to-death, but previous work neglected recurrent acute pulmonary exacerbation (PE) events and time-to-lung-transplantation, and mainly made use of smaller subsets of the registry data. Analyzing the entire dataset is expensive in terms of computation times. There is a need for algorithms that perform distributed analyses that simultaneously and unbiasedly investigate multiple correlated outcomes.


Objectives: Our primary goal was to investigate the association between FEV1 and the risk of PE, lung- transplant/death using all available registry data (2003-2016) for patients aged >= 6 years. 


Methods: We relied on the joint modelling framework, under the Bayesian paradigm, to simultaneously fit a joint model for a longitudinal marker, a recurrent event, and a terminal event. Due to the high computational time required to evaluate the entire dataset, we split the dataset into smaller non-overlapping subsets, parallelized their analyses, and then averaged individual posterior samples together. We explored different data splitting and combining strategies to get a consensus posterior. 


Results: Preliminary results suggest that FEV1 is negatively associated with the risk of experiencing death or transplantation. The model obtained from the split data estimates an association of -0.11 (95%CI -0.13,-0.10), while the model leveraging the entire dataset shows an estimates of -0.11 (-0.12,-0.10). The 10-fold reduction in sample size produced a 90% decrease in computing time. The results were also investigated through simulation studies.


Conclusions: The idea of distributing the Bayesian calculation is likely to be a useful solution to handle very big datasets without compromising the amount of information taken into account or sacrificing model adequacy, thereby, enhancing our understanding of CF FEV1 decline.
 