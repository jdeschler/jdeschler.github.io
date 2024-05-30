<h2 id="otherwork" style="margin: 2px 0px -15px;">Other Work and Writing</h2>

<div class="publications">
<ol class="bibliography">

{% for link in site.data.otherworks.main %}

<li class="workingpaper">
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
      <div class="title">{{ link.title }}</div>
      {% if link.author %} 
      <div class="author">{{ link.authors }}</div>
      {% endif %}
      {% if link.conference %} 
      <div class="periodical"><em>{{ link.conference }}</em>
      {% endif %}
      {% if link.notes %} 
      <strong> <i style="color:#e74d3c">{{ link.notes }}</i></strong>
      {% endif %}  </div>
  <div class="links">
    {% if link.pdf %} 
    <a href="{{ link.pdf }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">PDF</a>
    {% endif %}
  </div>
</li>

<br>

{% endfor %}

</ol>
</div>