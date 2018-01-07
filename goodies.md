---
layout: default
title: Goodies
permalink: /goodies/
---
<h1>Goodies</h1>
  <div class="album text-muted">


          <div class="row">

          {% for page in site.pages %}
            {% if page.category contains 'goodies' %}

            <div class="card" >

              <a href="{{ site.download_site}}goodies/{{ page.file }}.zip"><img class="card-img-top"  src="{{ site.download_site}}goodies/{{ page.file }}.png" alt="{{ page.title }}" /></a>
              <h4><a href="{{ site.download_site}}goodies/{{ page.file }}.zip">{{ page.title }}</a></h4>
              <p class="card-text">{{ page.description }}</p>
              <p class="card-text">{% for format in page.formats %}
                <span class="badge badge-success">{{ format }}</span>
              {% endfor %}
              </p>
            </div>
            {% endif %}
          {% endfor %}




        </div>
      </div>
