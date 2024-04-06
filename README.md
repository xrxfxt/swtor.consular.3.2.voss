{% include gallery.html folder='/img' %}

OR
```
<div class="flow" markdown="1">
- list
</div>
```
{% for repository in site.github.public_repositories %}
  * [{{ repository.name }}]({{ repository.html_url }})
{% endfor %}
