---
layout:        infographic
title:         "Energy production: transition pathways (Czechia)"
slug:          "transition-scenarios-comparison-czechia"
redirect_from: "/transition-scenarios-comparison-czechia"
published:     2022-07-26
weight:        73
tags-scopes:   [ cz ]
tags-topics:   [ energy, policies ]
caption:       "This infographic provides a comparison of four recent transition scenarios for electricity production in Czechia by 2030. Each of these pathways has a strikingly different impact on reducing greenhouse gas emissions that are related to electricity generation. The scenarios also focus on different things and use different methodologies."
data-our:      "https://docs.google.com/spreadsheets/d/14CB428mF-_iHTgrLb2Dd0zJZ4xHUMdGhbr_FZ2fZy6k/edit"
data-orig:
  - [ "Ember", "https://ember-climate.org/project/coal-free-czechia-2030/" ]
  - [ "Energynautics", "https://en.frankbold.org/sites/default/files/publikace/czech_grid_without_coal_by_2030_fin_0.pdf" ]
  - [ "Energynautics (follow-up study)", "https://frankbold.org/sites/default/files/publikace/sensitivity_analysis_czech_grid_without_coal_by_2030.pdf" ]
  - [ "BloombergNEF", "https://data.bloomberglp.com/professional/sites/24/BNEF-white-paper-EU-coal-transition-Final-6-July.pdf" ]
  - [ "NECP", "https://www.mpo.cz/cz/energetika/strategicke-a-koncepcni-dokumenty/vnitrostatni-plan-ceske-republiky-v-oblasti-energetiky-a-klimatu--252016/" ]
---

In this infographic, we compare several scenarios for the development of [electricity](/topics/energy) in Czechia.

## How to read the infographic

**Top of the graphic** compares the situation in 2019 and the situation in 2030 according to **power generation**: This parameter shows how much electricity will be delivered to the transmission system by which sources. Formally, this is the so-called _net generation_, which does not count the electricity that the power plants themselves consume. A reduction in total generation means that (due to savings) consumption will decrease, that _net exports_ will decrease, or even that we will import more electricity than we export.

{% include preview-box.html
    title="Individual scenarios"
    class="double-preview-box"
    card_class="col-6 p-1"
    text="We have prepared a detailed infographic for each scenario."
    slug="2020-scenario-bloombergnef,2020-scenario-ember,2018-scenario-energynautics,2019-scenario-necp"
%}

A gradual move away from fossil fuels, and most of all from coal, means a reduction in **greenhouse gas emissions**. Each study calculates such reductions using its own methodology (or not at all). Therefore, for all studies we **present our calculation of emission reductions** based on the difference in generation mix between 2019 and 2030 and on emission factors from the IPCC. See below for more on our calculation methodology.

**The bottom of the graphic** compares selected aspects of each scenario. In this table, we show the difference in the focus of each scenario and the methodology used to create them.

Of course, more scenarios for the transformation of the Czech energy sector have been developed over the years than we are able to compare in a single graphic.<!--; more can be found in our [research](/2020-research-transformation-of-energy).-->

### How the scenarios differ

The most significant difference is in the **energy mix** itself and thus in the impact of the scenarios on reducing <glossary id="anthropogenicgreenhousegases">greenhouse gas emissions</glossary>. This metric is most closely related to the share of coal and natural gas in electricity generation. However, the scenarios also differ substantially in the proportion of generation from solar, wind, and biomass and biogas. The only BloombergNEF and McKinsey scenarios have biomass and biogas as part of the market optimization and experience surprising reductions in generation. The BloombergNEF scenario also has a significant disparity between solar and wind -- in favor of wind, which has more balanced production during the day and year compared to solar panels. As a result, this mix can make do with less installed capacity from gas-fired power plants.

The scenarios differ in **the extent of the predicted [coal phase-out](/infographics/coal-phase-out-eu)**. The NECP and McKinsey scenarios project the shutdown of only some coal plants. The Energynautics scenario contemplates shutting down all coal _power plants_, yet there remains a significant amount of electricity generation from coal-fired thermal plants (combined heat and power). The Ember and BloombergNEF scenarios go the furthest and assume the shutdown of all coal _electric and thermal plants_.

The latter scenarios differ in their **focus and methodology**. For example, the Energynautics scenario focuses on the stability of the transmission system and therefore determines the installed capacity of each resource based on expert estimates. In contrast, the Ember, BloombergNEF and McKinsey scenarios look for changes in installed capacity through market optimization. In doing so, the Ember scenario looks at what a full coal phase-out option would look like as part of the assignment, while the BloombergNEF and McKinsey scenarios consider the lowest overall cost option.

{% include includes-local/energy-scenarios/where-the-scenarios-coincide.md %}

## Methodological comments on graphics

### Categorisation of resources: 2019

For 2019 generation, we use data from the [Energy Regulatory Office](https://www.eru.cz/en) (ERO) and consider the amount of electricity generated from a given feedstock regardless of the type of power plant in which it was produced.

In addition, there remains a small category of other generation, which we do not show for clarity (because energy scenarios typically do not show it). This consists of municipal and industrial waste, waste heat, fuel oils and other liquid fuels and amounts to 0.27 TWh, only about 0.3% of total generation.

### Categorisation of resources: 2030

**[BloombergNEF](/studies/2020-scenario-bloombergnef):** Compared to the numbers in the study, we adjust hydropower generation to be comparable to other electricity studies, i.e. we omit pumped storage. For the hydropower plants themselves, we therefore derive the planned generation from the current utilisation factor and the planned installed capacity.

**[Ember](/studies/2020-scenario-ember):** Compared to the numbers in the study, we are slightly adjusting the categorization to be more consistent with our 2019 distribution as well as other studies.

* **Gas:** The Ember study refers to only CCGTs and new gas CHP units as gas, as existing CHP units are not subject to optimization in their model. We add them to this category, specifically the _Other thermal_ category from their underlying data. In addition to existing CHP units, other facilities such as waste incinerators are in the _Other thermal_ category. However, these are insignificant in terms of installed capacity and generation, and so their inclusion in the gas category does not have a noticeable effect on the graphic or the emissions estimate.
* **Biomass and biogas:** The study does not include this category (as it is not subject to optimization in the model), we include the _Other renewable_ category from the underlying data, which is overwhelmingly biomass and biogas (in addition to biodegradable municipal waste).

<!--

**[McKinsey](/studies/2020-scenario-mckinsey):** As with the BloombergNEF study, we adjust hydroelectric generation to be comparable to other electricity studies, i.e., we omit pumped storage plants, compared to the numbers in the study. Thus, for hydropower plants alone, we again derive the planned generation from the current utilisation factor and the planned installed capacity.

The study also differs in the categorisation of biogas, which it categorises as a gas. The exact amount of biogas in the scenario is not known and according to the authors this amount is very small, so we have not adjusted the values in the scenario. Thus, the gas category here includes a small amount of biogas and the biomass and biogas category actually includes only biomass.

-->

**[Energynautics](/studies/2018-scenario-energynautics):** The numbers given directly in the study correspond well to our categorization, so we take them directly.

**[NECP](/studies/2019-scenario-necp):** The generation figures are taken directly from the study (in fact they are a combination of two tables, one showing generation from renewable sources in TJ, the other showing generation from conventional sources in TWh).

{% include includes-local/energy-scenarios/emissions.md %}
