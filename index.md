---
layout: blog
title: Latest
---


<h3> To receive occasional updates from me, email mx [at] mxmarin.ca </h3>


{% for blog in site.tags.blog limit: 1 %}
<h1><a href="{{ blog.url }}" style="display: inline">{{ blog.title }}</a></h1>
<div class="post"> {{ blog.content }} </div> 
{% endfor %}

--

### Recent Posts 
{% for blog in site.tags.blog offset:1 limit:3 %}
<h2><a href="{{ blog.url }}" style="display: inline">{{ blog.title }}</a> - {{ blog.date | date_to_string }} </h2>
{% endfor %}

# [Read more](/archive)
