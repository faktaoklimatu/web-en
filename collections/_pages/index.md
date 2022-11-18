---
layout: empty
title: Fakta o klimatu
slug: index
sitemap: true
---
<div class="section intro pb-4">
    <div class="container">
        <h1 class="display-1" id="home">Facts on Climate<br>Change</h1>
        <span class="tagline">Publicly available <span class='nobr'>infographics and explainers</span></span>
        <p>We are a team of independent analysts and experts, committed to cultivating the debate on climate change to be factual, constructive and based on science and verified data.</p>
        <p class="intro-buttons">
            <a href="#about" class="btn btn-secondary"><i class="fas fa-fw fa-info"></i> More about project</a>
            <a href="https://twitter.com/{{ site.twitter }}" class="btn btn-secondary"><i class="fab fa-fw fa-twitter"></i> Twitter (CZ)</a>
        </p>
    </div>
</div>

<div class="section pt-4 bg-extralight-blue"><div class="container" markdown="1">
{: .display-2}
## Featured

<p class="lead mb-0">New to the topic? Want to learn about climate change, its relationship to the level of emissions, temperature change and future predictions? Start with the infographics below.</p>
{% assign featured_slugs = "climate-change-scheme, concentration-warming-relationship, map-temperature-change, emission-pathways-paris, fossil-fuels-emissions, tipping-points-1" | split: ", " %}
{%- include preview-blocks-expandable.html slugs=featured_slugs rows=2 %}
<div class="alert alert-info data-staleness" role="alert">
    <h5 class="alert-heading"><i class="fas fa-lightbulb"></i> Work in progress </h5>
    <p>This website is the initial English version of a successful Czech project <a href="https://faktaoklimatu.cz">Fakta o klimatu</a>. At the moment, only a fraction of the content is available in English. If you like what you see, you can support further work via the <a href="{{ site.benevity }}">Benevity Cause</a> via your employer CSR program or directly using the <a href="{{ site.fundraising }}">Czech donation page</a>.</p>
</div>
</div></div>

{% assign sorted_index_tags = site.data.tags | where_exp: "item", "item.index-weight > 0" | sort: "index-weight" %}
<div class="section"><div class="container" markdown="1">
{: .display-2}
## Key project areas

{:.lead}
Climate change is a complex of interrelated phenomena. That is why the data that we collect, process and present is related to a number of areas of human activity – from economy to politics and power industry. Our materials are grouped in the following categories:

<div class="accordion" id="accordionExample">
{% for index_tag in sorted_index_tags %}
<div class="accordion-item">
    <div class="accordion-header collapsed" id="heading_{{ index_tag.id }}" role="button" data-toggle="collapse" data-target="#collapse_{{ index_tag.id }}" aria-expanded="false" aria-controls="collapse_{{ index_tag.id }}">
        <h3 class="display-3">
        <span class="fa fa-fw fa-chevron-up"></span>
        {{ index_tag.name-long | capitalize }}
        <small class="text-secondary d-none d-md-inline">({% include includes-local/object-stats.html tag=index_tag.id %})</small>
        </h3>
    </div>
    <div class="collapse" id="collapse_{{ index_tag.id }}"  aria-labelledby="heading_{{ index_tag.id }}" data-parent="#accordionExample" markdown="1">
{:.lead}
{{ index_tag.description | markdownify }}

{% assign objects = site.infographics | concat: site.studies | concat: site.explainers | where_exp: "item", "item.tags contains index_tag.id" | sort: "weight" %}
{% include preview-blocks.html blocks=objects link=index_tag limit=6 %}

</div>
</div>
{% endfor %}
</div> <!-- accordion end -->

</div></div>
<div class="section"><div class="container clearfix" markdown="1">
{:#about .display-2}
## About our work

<div class="row about-us lead mb-5 justify-content-between">
<div class="col-12 col-md-6 pt-2 pt-md-4" markdown="1">

**We do research and analytical work**. We sift through the data, searching for bits that help a deeper understanding of climate change, its impacts and possible solutions. We accentuate the regional matters of Czechia and Europe but do not omit global views.

**We communicate to key audiences**. We create data visualizations, articles, podcasts or lectures for the general public and clients from both the private and public sectors.

</div>
<div class="col-12 col-md-6 col-lg-5 pt-4" markdown="1">
### We strive for

{:.arrow}
* **Clear and publicly accessible information** on climate change and possible pathways to a net-zero society
* **Political decisions grounded in data** and rigorous analyses
* **An educated and informed society**, a constructive public debate and high-quality news coverage
</div>

<div class="col-12 mt-3">
<a href="/about" class="btn btn-primary btn-md-lg"><i class="fas fa-fw fa-info"></i> More about our project</a>
</div>
</div>

{:.display-3}
### Awards

<div class="row about-us lead">
    <div class="col-12 col-md-6 col-lg-4 p-3 p-md-4 price">
        <div class="price-1"></div>
        <div>
            <strong>Award for the communication of climate change</strong> (2020) from the Czech Learned Society and United Nations Information Centre in Prague
        </div>
    </div>
    <div class="col-12 col-md-6 col-lg-4 p-3 p-md-4 price">
        <div class="price-2"></div>
        <div>
            First price in the Czech <strong>Climate Challenge</strong> accelerator (2020)
        </div>
    </div>
    <div class="col-12 col-md-6 col-lg-4 p-3 p-md-4 price">
        <div class="price-3"></div>
        <div>
            <strong>AFO Olomouc Award</strong> for a significant contribution to the popularization of science (2022)
        </div>
    </div>
</div>

</div></div>
<div class="section"><div class="container clearfix" markdown="1">

{:.display-2 .mb-3}
## Who is using our materials?

{:.lead}
Our infographics and texts are used by Czech and foreign institutions, news portals, consulting companies, schools and other actors.

<div class="logos mt-md-5 mb-md-4">
<img loading="eager" class="small" src="/assets-local/about/logo-cnb.png" alt="Czech National Bank">
<img loading="eager" class="small" src="/assets-local/about/logo-mzp.png" alt="Ministry of the Environment of the Czech Republic">
<img loading="eager" src="/assets-local/about/logo-pwc.png" alt="PwC">
<img loading="eager" class="small" src="/assets-local/about/logo-omg.png" alt="OMG Media Group">
<img loading="eager" src="/assets-local/about/logo-mckinsey.png" alt="McKinsey">
<img loading="eager" class="small" src="/assets-local/about/logo-seznam-zpravy.png" alt="Seznam Zprávy">
<img loading="eager" class="small" src="/assets-local/about/logo-irozhlas.png" alt="iRozhlas">
<img loading="eager" class="small" src="/assets-local/about/logo-respekt.png" alt="Respekt">
<img loading="eager" class="small" src="/assets-local/about/logo-deloitte.png" alt="Deloitte">
</div>

</div></div>
