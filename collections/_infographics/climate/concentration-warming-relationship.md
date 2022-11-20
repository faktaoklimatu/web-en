---
layout:        infographic
title:         "How are CO₂ concentrations related to warming?"
slug:          "concentration-warming-relationship"
redirect_from: "/concentration-warming-relationship"
published:     2022-11-20
weight:        90
tags-scopes:   [ world ]
tags-topics:   [ climate ]
caption:       "Historical data as well as future climate models show that global warming is (approximately) directly proportional to the increase of CO<sub>2</sub> concentrations in the atmosphere. More specifically: every time the CO<sub>2</sub> concentrations rise by 10 ppm (parts per million), the mean global temperature increases by 0.1 °C."
data-our:      "https://docs.google.com/spreadsheets/d/1aVn3Uz1wLUtmATagtZHEpeayiee6uy_BRAivZPwfb2s/edit?usp=sharing"
data-orig:
  - [ "NASA", "https://data.giss.nasa.gov/gistemp/" ]
  - [ "Keeling curve", "https://scripps.ucsd.edu/programs/keelingcurve/" ]
---
{% comment %}
{% include preview-box.html
    title="A more detailed description of the context"
    text="The direct correlation between warming and increased CO<sub>2</sub> concentrations, as well as the effect of other greenhouse gases and aerosols or the effect of climate inertia, is explained in more detail in the explainer text."
    slug="otepleni-zvysenim-koncentrace-co2"
%}
{% endcomment %}

## What the graph shows

The points on the left side of the graph show the individual years from 1884-2020. The location of the point corresponds to the CO<sub>2</sub> concentration values (on the horizontal axis) and the temperature anomaly values for that year (on the vertical axis). The graph shows that the relationship is approximately proportional, with **each 10 ppm increase in CO<sub>2</sub> concentration leading to a temperature increase of about 0.1 °C**. The text below describes this relationship in more detail. <!-- and also in the related explainer [How much warmer will it get if CO₂ concentrations increase?](/explainery/otepleni-zvysenim-koncentrace-co2).-->

The dots in the graph are color-coded per individual year (grouped by 20 years each). The points show that the increase in CO<sub>2</sub> concentrations has been accelerating in recent years, corresponding to increasing annual CO<sub>2</sub> emissions.

On the right-hand side of the graph, we show the expected global warming for higher CO<sub>2</sub> concentrations if emissions continue at the current rate.

## How is the relationship between CO<sub>2</sub> concentration and global warming inaccurate?

The dominant effect of carbon dioxide on global warming is well established, so the **graph** shows **causation**, not just random correlation.
On the other hand, many other factors also influence global warming: other greenhouse gases, currents in the atmosphere and ocean that distribute heat around the planet, as well as aerosols and cloud formation (the shading effect). 
Is it correct to state that every time the CO<sub>2</sub> concentration rises by 10 ppm also leads to a rise in temperature of about 0.1 °C? The following paragraphs show how this relationship is only an approximation.

* The theoretically derived relationship for the dependence of global warming on greenhouse gas concentration is logarithmic. [^1] [^11] However, a small range of concentrations can be well approximated by a linear relationship, as shown by the measured data.

    $$
    \Delta T(c) = S \cdot \log_2 \left(\frac{c_0 + \Delta c}{c_0}\right) \approx \frac{S}{c_0 \ln 2} \cdot \Delta c
    $$

    In this relationship, $$c_0$$ denotes the initial concentration, $$\Delta c$$ is the increase in concentration, and $$S$$ is a parameter called *climate sensitivity* - it expresses how much the temperature of the planet increases when the concentration of greenhouse gas in the atmosphere doubles. **The direct proportionality between concentrations and global warming ceases to be a good approximation if the increase in concentrations is too large**.

* The climate system has inertia - some processes reach equilibrium in units of years, others in tens or hundreds of years. Therefore, it is necessary to distinguish between **short-term climate sensitivity** (*TCR, Transient Climate Response*), which takes into account processes on the order of units of years, **balanced climate sensitivity** (*ECS, Equilibrium Climate Sensitivity*), which takes into account processes on the order of tens of years, and **long-term climate response** (*ESS, Earth System Sensitivity*), which takes into account processes on the order of hundreds and thousands of years.[^8] [^9] [^2] Current climate system models suggest short-term climate sensitivity values *TCR* of around 1.7 °C (range 1.3-3.0°C)[^3] and balanced climate sensitivity values *ECS* of around 3 °C (range 2.3-4.7 °C).[^10] [^4] The data we show in the graph are continuous and correspond to the short-term climate response. If concentrations were to stabilise, temperatures would continue to rise for several decades before global warming stopped at values corresponding to the balanced climate sensitivity. In other words, **the direct proportionality between concentrations and global warming would cease to hold if CO<sub>2</sub> emissions were radically reduced to near zero.** In that case, concentrations would stabilise or begin to fall, but the planet's temperature would continue to rise for some time.

* Carbon dioxide is responsible for about 70% of global warming.[^6] The remaining 30% is due to other greenhouse gases, mainly methane and nitrous oxide, which are also increasing in the atmosphere. Along with greenhouse gases, however, mankind also emits aerosols, which have a cooling effect on the planet by reflecting solar radiation and contributing to the formation of clouds.[^7] Global warming shown includes all these phenomena, but only CO<sub>2</sub> concentrations are plotted on the horizontal axis. **Thus, the claim of direct proportionality between concentration increases and warming is misleading in that it only shows a dependence on the dominant factor.** However, because the cooling effect of aerosols and the warming effect of other greenhouse gases partially cancel each other out, it can be argued that CO<sub>2</sub> is the driving factor behind well over 70% of global warming.

## Where the data in this infographic comes from?

* Temperature anomaly values for each year are from the *NASA Goddard Institute for Space Studies* dataset.<!-- For more on the concept of temperature anomaly, see the accompanying text to the infographic [Evolution of the global temperature anomaly](/infografiky/vyvoj-teplotni-anomalie).-->

* CO<sub>2</sub> concentration values for each year are based on measurements from the *Scripps Institution of Oceanography*, which is part of <glossary id="noaa">NOAA</glossary>.<!-- Separately, the evolution of atmospheric CO<sub>2</sub> concentration is shown in the graphic [Evolution of atmospheric CO₂ concentration](/infografiky/koncentrace-co2).-->

* The trend curve corresponds to the equation $$\Delta T(c) = S \cdot \log_2 (\frac{c}{c_0})$$, where $$c$$ is the concentration, $$c_0$$ is the initial concentration, and $$S$$ is the continuous climate sensitivity parameter. This theoretical relationship is used in idealized conditions of simulations – either as a relation for warming after equilibrium, where S corresponds to ECS (*Equilibrium Climate Sensitivity*), or for the transient warming when the CO<sub>2</sub> concentration increases by 1% each year, where S corresponds to TCR (*Transient Climate Response*). However, in the data shown, global warming is not only due to an increase in CO<sub>2</sub> concentrations but also due to increasing concentrations of other greenhouse gases. Therefore, we take the TCR and ECS values obtained from the simulations as indicative only and fit the value of S to show the dependence (S = 2.37 °C). The uncertainty band is shown between S = 2.0 °C and S = 3.1 °C, which corresponds to the uncertainty profile in both TCR and ECS and partially accounts for the effect of climate inertia in stabilizing CO<sub>2</sub> concentrations.

## Historical note

The link between global warming and atmospheric carbon dioxide concentration is one of the keys and longest-studied links in the study of climate change. The first calculations were published by Svante Arrhenius in 1886, and his estimates of climate sensitivity have been confirmed and refined by subsequent studies.<!-- More in graphics and text [History of greenhouse effect research](/infografiky/historie-sklenikoveho-efektu).-->

## Sources and notes

[^1]: More precisely: radiative forcing is directly proportional to the logarithm of concentration - and warming is directly proportional to radiative forcing; for more see [wikipedia: Radiative Forcing](https://en.wikipedia.org/wiki/Radiative_forcing)
[^2]: A more detailed discussion of the concept of climate sensitivity, including different time scales [wikipedia: Measures of Climate Sensitivity](https://en.wikipedia.org/wiki/Climate_sensitivity#Measures_of_climate_sensitivity)
[^3]: G. A. Meehl et. al. ["Context for interpreting equilibrium climate sensitivity and transient climate response from the CMIP6 Earth system models."](https://advances.sciencemag.org/content/6/26/eaba1981), Science Advances 6.26 (2020).
[^4]: S. C. Sherwood, Webb, et. al. ["An Assessment of Earth's Climate Sensitivity Using Multiple Lines of Evidence."](https://agupubs.onlinelibrary.wiley.com/doi/10.1029/2019RG000678), Reviews of Geophysics 58.4 (2020).
[^5]: Matthews, H. D., Tokarska, K. B., Nicholls, Z. R. J. et al. ["Opportunities and challenges in using remaining carbon budgets to guide climate policy."](https://doi.org/10.1038/s41561-020-00663-3), Nature Geoscience 13.12, str. 769–779 (2020).
[^6]: [Annual Greenhouse Gas Index](https://www.globalchange.gov/browse/indicators/annual-greenhouse-gas-index)
[^7]: Myhre, G., Myhre, C. E. L., Samset, B. H. & Storelvmo, T. (2013) ["Aerosols and Their Relation to Global Climate and Climate Sensitivity."](https://www.nature.com/scitable/knowledge/library/aerosols-and-their-relation-to-global-climate-102215345/), Nature Education Knowledge 4.5, str. 7 (2013).
[^8]: Knutti R. Hegerl. ["Beyond Equilibrium Climate Sensitivity."](https://www.nature.com/articles/ngeo3017), Nature Geoscience 10.10, str. 727–736 (2017).
[^9]: Carbon Brief explainer: [How scientists estimate climate sensitivity](https://www.carbonbrief.org/explainer-how-scientists-estimate-climate-sensitivity)
[^10]: Carbon Brief guest post: [Why low-end climate sensitivity can now be ruled out](https://www.carbonbrief.org/guest-post-why-low-end-climate-sensitivity-can-now-be-ruled-out)
[^11]: Skeptical Science: [How could global warming accelerate if CO₂ is 'logarithmic'?](https://skepticalscience.com/why-global-warming-can-accelerate.html)