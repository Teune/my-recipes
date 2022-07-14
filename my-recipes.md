---
layout: single
title: "My recipes"
---

{% for product in site.data.recipes.recipes %}
<span>{{ product.group }}:</span>
<ul>
    {% for item in product.items %}
    <li>{{ item.name }}</li>
    {% endfor %}
</ul>
{% endfor %}