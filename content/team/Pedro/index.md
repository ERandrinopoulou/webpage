---
all_day: true
#authors: []
date: "2025-05-01"
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
summary: "Joint models for multiple longitudinal and survival outcomes using the Cystic Fibrosis data" 
#tags: []
title: Pedro Afonso
#url_code: ""
#url_pdf: ""
#url_slides: "ISCB_ARAT.pdf"
#url_video: ""
---

Pedro Afonso is a PhD student working on the following projects:

## Efficiently analyzing big data with Bayesian joint models for longitudinal and time-to-event data

The joint modeling of longitudinal and time-to-event outcomes has become a popular tool in follow-up stud-
ies. However, fitting Bayesian joint models to large datasets, such as patient registries, can require extended
computing times. To speed up sampling, we divided a patient registry dataset into subsamples, analyzed
them in parallel, and combined the resulting Markov chain Monte Carlo draws into a consensus distribu-
tion. We used a simulation study to investigate how different consensus strategies perform with joint models.
In particular, we compared grouping all draws together with using equal- and precision-weighted averages.
We considered scenarios reflecting different sample sizes, numbers of data splits, and processor characteris-
tics. Parallelization of the sampling process substantially decreased the time required to run the model. We
found that the weighted-average consensus distributions for large sample sizes were nearly identical to the
target posterior distribution. The proposed algorithm has been made available in an R package for joint mod-
els, JMbayes2. This work was motivated by the clinical interest in investigating the association between
ppFEV1, a commonly measured marker of lung function, and the risk of lung transplant or death, using data
from the US Cystic Fibrosis Foundation Patient Registry (35,153 individuals with 372,366 years of cumu-
lative follow-up). Splitting the registry into five subsamples resulted in an 85% decrease in computing time,
from 9.22 to 1.39 hours. Splitting the data and finding a consensus distribution by precision-weighted aver-
aging proved to be a computationally efficient and robust approach to handling large datasets under the joint
modeling framework.
 
## Between- and Within-Group Comparisons of FEV1 Rate of Decline in Cystic Fibrosis 

Difference in rate of change for before and after Ivacaftor treatment in subjects with a G551D mutation. Different modelling approaches (linear mixed-effects models, generalized estimating equations and joint models of longitudinal and survival data) and data scenarios are investigated.

## A joint model for (un)bounded longitudinal markers, competing risks, and recurrent events]{A joint model for (un)bounded longitudinal markers, competing risks, and recurrent events

Joint models for longitudinal and survival data have become a popular framework for studying the
association between repeatedly measured biomarkers and clinical events. Nevertheless, addressing complex survival
data structures, especially handling both recurrent and competing event times within a single model, remains a
challenge. This causes important information to be disregarded. Moreover, existing frameworks rely on a Gaussian
distribution for continuous markers, which may be unsuitable for bounded biomarkers, resulting in biased estimates of
associations. To address these limitations, we propose a Bayesian shared-parameter joint model that simultaneously
accommodates multiple (possibly bounded) longitudinal markers, a recurrent event process, and competing risks. We
use the beta distribution to model responses bounded within any interval (a, b) without sacrificing the interpretability
of the association. The model offers various forms of association, discontinuous risk intervals, and both gap and
calendar timescales. A simulation study shows that it outperforms simpler joint models. We analyze the US Cystic
Fibrosis Foundation Patient Registry to study the associations between lung function decline, cumulative changes
in body mass index, and the risk of recurrent pulmonary exacerbations, while accounting for the competing risks of
death and lung transplantation. Our efficient implementation allows fast fitting of the model despite its complexity
and the large sample size. Our comprehensive approach provides new insights into cystic fibrosis progression. The
model is available in the R package JMbayes2.