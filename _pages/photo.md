---
title: "Photos"
permalink: /images/
author_profile: true
redirect_from:
  - /photo.html
    
---

{% include base_path %}

<div>
	{% for image in images %}
	    {% if image.path contains '/images/shows' %}  
	        <img src="{{image.path}}" alt="{{ image.name }}" />
	    {% endif %}  
	{% endfor %}
</div>
