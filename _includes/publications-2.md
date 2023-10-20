<h1 id="publications"></h1>

<h2 style="margin: 60px 0px -15px;">Publications</h2>

<br>
<ul>

{% for link in site.data.publications.main %}

 <li>
<a href="{{ link.pdf }}">{{ link.title }}</a>
  <br>
   {{ link.authors }}
  <br>
   <em>{{ link.conference }}</em> 
   <br>
   {% if link.pdf %} 
   [<a href="{{ link.pdf }}">PDF</a>]  
   {% endif %}
   {% if link.arxiv %} 
   [<a href="{{ link.arxiv }}">arXiv</a>]  
   {% endif %}
   {% if link.code %} 
   [<a href="{{ link.code }}">Code</a>]  
   {% endif %}
   {% if link.slides %} 
   [<a href="{{ link.code }}">Slides</a>]  
   {% endif %}
   {% if link.notes %} 
      <strong> <i style="color:#e74d3c">{{ link.notes }}</i></strong>
   {% endif %}
</li>
<br>

{% endfor %}

</ul>
