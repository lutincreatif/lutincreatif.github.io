---
layout: default
title: Goodies
permalink: /goodies/
---

<div class="album text-muted">
        <div class="container">

          <div class="row">

          {% for page in site.pages %}
            {% if page.category contains 'goodies' %}

            <div class="card">
              <img data-src="holder.js/100px280?theme=thumb" alt="Card image cap">
              <h4>{{ page.title }}</h4>
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
      </div>
