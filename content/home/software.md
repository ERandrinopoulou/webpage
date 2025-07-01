+++
# Custom widget.
# An example of using the custom widget to create your own homepage section.
# To create more sections, duplicate this file and edit the values below as desired.
widget = "custom"
active = true
date = 2016-04-20T00:00:00

# Note: a full width section format can be enabled by commenting out the `title` and `subtitle` with a `#`.
title = "Software"
subtitle = ""

# Order that this section will appear in.
weight = 7

+++

`multiLME`

This **R** package fits multivariate mixed effects models with association parameters. Furthermore, individual dynamic predictions can be obtained.

*Useful functions*:

- `mv_lme`: multivariate mixed effects models with association parameters
- `DynPred_mv_lme`: dynamic individual predictions
Install the package using the following code:

`devtools::install_github("ERandrinopoulou/multiLME", dependencies = TRUE)`

The vignette can be found [here](https://erandrinopoulou.github.io/multiLME/multiLME-vignette.html)