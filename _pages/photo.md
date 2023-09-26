---
title: "Photos"
permalink: /photo/
author_profile: true
redirect_from:
  - /photo.html
    
---

{% include base_path %}

<div>
	{% for image in site.static_files %}
	    {% if image.path contains '/images/' %}  
	        <img src="{{image.path}}" alt="{{ image.name }}" />
	    {% endif %}  
	{% endfor %}
</div>
