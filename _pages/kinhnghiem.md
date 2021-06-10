---
layout: default
title: Kinh Nghiệm
permalink: /kinh-nghiem/
---
<div>
  {% for category in site.categories %}
    {% if category[0] == "Life" %}
      <div class="container">
        <div class="row">
          <div class="col col-12 col-d-10 col-m-12 push-m-0 push-d-1">
            <div class="container__inner">
              <div class="contaniner__inner-box">
                <div class="row grid">
                  {% for post in category[1] %}
                  <div class="article col col-4 col-d-6 col-m-12 grid__post">
                    {% include article.html %}
                  </div>
                  {% endfor %}
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    {% endif %}
  {% endfor %}
</div>
