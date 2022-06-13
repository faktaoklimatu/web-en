---
layout: empty
title: Facts on climate
slug: index
sitemap: true
---
<div class="section intro">
    <div class="container">
        <h1 class="display-1" id="home">Fakta o změně<br>klimatu</h1>
        <span class="tagline">Veřejně dostupné<br>infografiky a datasety</span>
        <p class="mb-5">Shromažďujeme data o klimatu a klimatické změně, která poskytují vědecké instituce (ČHMÚ, NASA, Eurostat a jiné) a zpracováváme z nich grafy a infografiky pro <a href="/how-to-use" title="Jak používat naše materiály">další použití</a>.<br/>
            <a href="{{ site.fundraising }}" class="btn btn-primary mt-3"><i class="fas fa-fw fa-heart"></i> Podpořte nás</a>
            <a href="https://twitter.com/{{ site.twitter }}" target="_blank" class="btn btn-secondary mt-3"><i class="fab fa-fw fa-twitter"></i> Twitter</a>
            <a href="#o-projektu" class="btn btn-secondary mt-3"><i class="fas fa-fw fa-info"></i> O projektu</a>
        </p>
    </div>
</div>

{% assign sorted_index_tags = site.data.tags | where_exp: "item", "item.index-weight > 0" | sort: "index-weight" %}
<div class="section"><div class="container" markdown="1">
{: .display-2}
## Oblasti, kterým se věnujeme

{:.lead}
Klimatická změna je složitý komplex vzájemně provázaných jevů. Data, která sbíráme, třídíme a zpracováváme, se proto dotýkají různých oborů lidské činnosti – od ekonomiky přes politiku až po energetiku. Pro usnadnění orientace na webu třídíme naše materiály do níže uvedených kategorií.

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
## O nás a naší práci

{:.lead}
Projekt Fakta o klimatu usiluje o zkvalitnění společenské diskuse o klimatické změně.
Snažíme se dodávat srozumitelné údaje široké veřejnosti a vizuálně zpracovávat vědecké informace, aby bylo rozhodování ve věcech týkajících se klimatu založené na aktuálních a ověřených datech.

{:.lead}
Debata o klimatické změně je komplikovaná a na všech stranách plná zbytečných emocí, polopravd a mýtů. Chceme poutat pozornost na důležitá témata a stavět most mezi vědci a lidmi, kterých se změny klimatu týkají. A to jsou všichni lidé.

{:.lead}
Jsme tým profesionálů zabývajících se různými obory – přírodovědou, informatikou, pedagogikou nebo komunikací. Pracuje na dobrovolnické bázi a finance na provoz získáváme od dárců, nepracujeme na ničí objednávku. Při naší činnosti komunikujeme s politiky, energetickými firmami i aktivistickými hnutími. Fakta o klimatu jsou však nezávislý projekt, který může podpořit každý.

<div class="row">
  <a href="/about" class="btn btn-primary btn-lg col"><i class="fas fa-fw fa-info"></i> Více o projektu</a>
  <a href="{{ site.fundraising }}" class="btn btn-primary btn-lg col"><i class="fas fa-fw fa-heart"></i> Podpořte nás</a>
</div>

<a href="https://www.climate-kic.org/" class="no-ext-link-icon"><img class="index-logos float-right" src="/assets-local/img/logo-climate-kic.png" alt="Climate-KIC logo"/></a>
<a href="https://climatechallenge.impacthub.cz/" class="no-ext-link-icon"><img class="index-logos float-right" src="/assets-local/img/logo-climate-challenge.png" alt="Climate Challenge logo"/></a>

{:.lead}
V roce 2020 jsme zvítězili v akceleračním programu [Climate Challenge](https://climatechallenge.impacthub.cz/) pořádaným sítí podnikatelských inkubátorů [Impact Hub](https://impacthub.cz). V rámci toho náš projekt podpořila evropská iniciativa [Climate-KIC](https://www.climate-kic.org/), která hledá inovativní řešení na klimatickou krizi.

</div></div>
