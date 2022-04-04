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
