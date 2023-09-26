---
layout: default
comments: false
title: "Photos"
permalink: /Photos/
author_profile: true
redirect_from:
  - /photo.html
    
---

<div>
	{% for image in site.static_files %}
	    {% if image.path contains '/images/shows' %}  
	        <img src="{{image.path}}" alt="{{ image.name }}" />
	    {% endif %}  
	{% endfor %}
</div>
