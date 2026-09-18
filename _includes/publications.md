<h2 id="publications" style="margin: 2px 0px -15px;">Publications</h2>

<div class="publications">
<ol class="bibliography">

{% for link in site.data.publications.articles limit: 3 %}

<li>
<div class="pub-row">
  {% if link.image %}
  <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    <img src="{{ link.image }}" class="teaser img-fluid z-depth-1" style="width=100;height=40%">
    {% if link.conference_short %} 
    <abbr class="badge">{{ link.conference_short }}</abbr>
    {% endif %}
  </div>
  {% endif %}
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
      <div class="title">
        {% if link.pdf %}
        <a href="{{ link.pdf }}">{{ link.title }}</a>
        {% else %}
        {{ link.title }}
        {% endif %}
      </div>
      <div class="author">{{ link.authors }}</div>
      <div class="periodical">
        {% if link.journal %}
        {{ link.journal }}
        {% else %}
        {{ link.conference }}
        {% endif %}
      </div>
    <div class="links">
      {% if link.pdf %} 
      <a href="{{ link.pdf }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">PDF</a>
      {% endif %}
      {% if link.code %} 
      <a href="{{ link.code }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Code</a>
      {% endif %}
      {% if link.page %} 
      <a href="{{ link.page }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Project Page</a>
      {% endif %}
      {% if link.bibtex %} 
      <a href="{{ link.bibtex }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">BibTex</a>
      {% endif %}
      {% if link.notes %} 
      <strong> <i style="color:#e74d3c">{{ link.notes }}</i></strong>
      {% endif %}
      {% if link.others %} 
      {{ link.others }}
      {% endif %}
    </div>
  </div>
</div>
</li>
<br>

{% endfor %}

</ol>
{% if site.data.publications.articles.size > 3 %}
<p style="margin: 0px 0px 10px; font-size: 0.95rem;"><em>Selected; see my <a href="{{ site.cv_link }}"><autocolor>CV</autocolor></a> for the full list.</em></p>
{% endif %}
</div>


<h2 id="in-prep" style="margin: 2px 0px -15px;">In Prep</h2>

<div class="publications">
<ol class="bibliography">

{% for link in site.data.publications.in_prep limit: 3 %}

<li>
<div class="pub-row">
  {% if link.image %}
  <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    <img src="{{ link.image }}" class="teaser img-fluid z-depth-1" style="width=100;height=40%">
    {% if link.conference_short %} 
    <abbr class="badge">{{ link.conference_short }}</abbr>
    {% endif %}
  </div>
  {% endif %}
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
      <div class="title">{{ link.title }}</div>
      <div class="author">{{ link.authors }}</div>
      <div class="periodical">
        {% if link.venue %}
        {{ link.venue }}
        {% endif %}
        {% if link.expected %}
        {{ link.expected }}
        {% endif %}
      </div>
    <div class="links">
      {% if link.status %} 
      <strong> <i style="color:#e74d3c">{{ link.status }}</i></strong>
      {% endif %}
    </div>
  </div>
</div>
</li>
<br>

{% endfor %}

</ol>
{% if site.data.publications.in_prep.size > 3 %}
<p style="margin: 0px 0px 10px; font-size: 0.95rem;"><em>Selected; see my <a href="{{ site.cv_link }}"><autocolor>CV</autocolor></a> for the full list.</em></p>
{% endif %}
</div>


<h2 id="presentations" style="margin: 2px 0px -15px;">Presentations</h2>

<div class="publications">
<ol class="bibliography">

{% for link in site.data.publications.presentations limit: 3 %}

<li>
<div class="pub-row">
  {% if link.image %}
  <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    <img src="{{ link.image }}" class="teaser img-fluid z-depth-1" style="width=100;height=40%">
    {% if link.conference_short %} 
    <abbr class="badge">{{ link.conference_short }}</abbr>
    {% endif %}
  </div>
  {% endif %}
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
      <div class="title">
        {% if link.slides %}
        <a href="{{ link.slides }}">{{ link.title }}</a>
        {% else %}
        {{ link.title }}
        {% endif %}
      </div>
      <div class="author">{{ link.authors }}</div>
      <div class="periodical"><em>{{ link.conference }}</em>
      </div>
    <div class="links">
      {% if link.slides %} 
      <a href="{{ link.slides }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Slides</a>
      {% endif %}
      {% if link.notes %} 
      <strong> <i style="color:#e74d3c">{{ link.notes }}</i></strong>
      {% endif %}
      {% if link.others %} 
      {{ link.others }}
      {% endif %}
    </div>
  </div>
</div>
</li>
<br>

{% endfor %}

</ol>
{% if site.data.publications.presentations.size > 3 %}
<p style="margin: 0px 0px 10px; font-size: 0.95rem;"><em>Selected; see my <a href="{{ site.cv_link }}"><autocolor>CV</autocolor></a> for the full list.</em></p>
{% endif %}
</div>
