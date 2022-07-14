---
layout: empty
title: Fakta o klimatu
slug: index
sitemap: true
---
<div class="section intro">
    <div class="container">
        <h1 class="display-1" id="home">Facts on Climate Change</h1>
        <span class="tagline"><br>Free infographics and datasets</span>
        <p class="mb-5">We collect various climate change data provided by Czech and international research and monitoring institutions (CHMI, NASA, Eurostat, etc.) and present this data in our graphs and infographics for <a href="/how-to-use" title="How to use our materials">further use</a>.<br/>
            <a href="{{ site.fundraising }}" class="btn btn-primary mt-3"><i class="fas fa-fw fa-heart"></i> Support us</a>
            <a href="https://twitter.com/{{ site.twitter }}" target="_blank" class="btn btn-secondary mt-3"><i class="fab fa-fw fa-twitter"></i> Twitter</a>
            <a href="#o-projektu" class="btn btn-secondary mt-3"><i class="fas fa-fw fa-info"></i> More about project</a>
        </p>
    </div>
</div>

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
{:#o-projektu .display-2}
## About us and our work

{:.lead}
We would like to contribute to a more evidence-based Czech public debate about climate change.
We create easy-to-understand visual and text materials and communicate the latest research findings to support key decisions in the Czech Republic that are related to climate change and a transition to a net zero economy.

{:.lead}
The debate about climate change is complicated and full of emotions, half-truths and myths. We want to highlight the most important issues and build bridges between scientists and all people affected by climate change. Which means all people.

{:.lead}
We are a team of professionals with various skills and expertise – science, IT, communication and teaching – and we communicate with journalists, politicians, stakeholders as well as activists. We are an independent think tank and our budget is based on donations and grants.

<div class="row">
  <a href="/about" class="btn btn-primary btn-lg col"><i class="fas fa-fw fa-info"></i> More about our project</a>
  <a href="{{ site.fundraising }}" class="btn btn-primary btn-lg col"><i class="fas fa-fw fa-heart"></i> Support us</a>
</div>

<a href="https://www.climate-kic.org/" class="no-ext-link-icon"><img class="index-logos float-right" src="/assets-local/img/logo-climate-kic.png" alt="Climate-KIC logo"/></a>
<a href="https://climatechallenge.impacthub.cz/" class="no-ext-link-icon"><img class="index-logos float-right" src="/assets-local/img/logo-climate-challenge.png" alt="Climate Challenge logo"/></a>

{:.lead}
In 2020, we received the best project award in the [Climate Challenge](https://climatechallenge.impacthub.cz/) Acceleration Program, which is organized by a network of business incubators called [Impact Hub](https://impacthub.cz) and we were supported by [Climate-KIC](https://www.climate-kic.org/), the European initiative searching for innovative solutions to the current climate crisis.

</div></div>
