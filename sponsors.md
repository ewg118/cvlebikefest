---
layout: default
title: CVLEBIKEFEST p/b The Dairy Market Sponsors
permalink: /sponsors/
---

## {{page.title}}

CVLEBIKEFEST is made possible by our sponsors, who support the club financially and/or with in-kind 
contributions.

{% for sponsor in site.data.sponsors %}

<div class="row section">
    <div class="col-md-3 text-center">
        {% if sponsor.image %}
        <a href="{{sponsor.url}}">
            <img src="{{site.baseurl}}/images/{{sponsor.image}}" alt="{{sponsor.name}} Logo" class="block-image"/>
        </a>
        {% endif %}        
    </div>
    <div class="col-md-9">
        <h4><a href="{{sponsor.url}}" title="{{sponsor.name}}">{{sponsor.name}}</a></h4>
        <p>{{sponsor.desc}}</p>
    </div>
</div>

{% endfor %}

### Prizes and Primes
The following local businesses have offered goods and services as prizes and primes for the criterium races and Charlottesville Community Bikes' online auction fundraiser.

{% for prize in site.data.prizes %}

<div class="row section">
    <div class="col-md-3 text-center">
        {% if prize.image %}
        <a href="{{prize.url}}">
            <img src="{{site.baseurl}}/images/{{prize.image}}" alt="{{prize.name}} Logo" class="block-image"/>
        </a>
        {% endif %}        
    </div>
    <div class="col-md-9">
        <h4><a href="{{prize.url}}" title="{{prize.name}}">{{prize.name}}</a></h4>
        <p>{{prize.desc}}</p>
    </div>
</div>

{% endfor %}
