---
layout: blog
title: Latest
---


### To receive occasional updates from me, email mx [at] mxmarin.ca
### [Current projects](https//mxmarin.ca)
-----

<div style="padding: 30px">
{% for blog in site.tags.blog limit: 1 %}
<h1 style="text-indent: 25px"><a href="{{ blog.url }}" style="display: inline">{{ blog.title }}</a></h1>

<div class="post"> {{ blog.content }} </div> 
{% endfor %}
</div>
-----
<br>
{% include blurb.md %}
<br>

-----
<br>
## Previously: 
{% for blog in site.tags.blog offset:1 limit:3 %}
<h4><a href="{{ blog.url }}" style="display: inline">{{ blog.title }}</a> - {{ blog.date | date_to_string }} </h4>
{% endfor %}

<p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | relative_url }}">via RSS</a></p>


### [Read more](/archive)
