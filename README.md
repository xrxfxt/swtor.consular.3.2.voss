{% include gallery.html folder='/img' %}

OR
```
<div class="flow" markdown="1">
- list
</div>
```

{% if site.github.is_project_page %}
  <p class="view"><a href="{{ site.github.repository_url }}">View the Project on GitHub <small>{{ site.github.repository_nwo }}</small></a></p>
{% endif %}{% include gallery.html folder='/img' %}

OR
```
<div class="flow" markdown="1">
- list
</div>
```
{% for repository in site.github.public_repositories %}
  * [{{ repository.name }}]({{ repository.html_url }})
{% endfor %}
