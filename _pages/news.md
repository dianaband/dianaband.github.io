---
layout: post
title: news
permalink: /news/
---
<p style="font-size:14pt;color:#666;margin:5px;">{{ post.intro }}NEWS</p><hr><br/><br/>

{% for post in site.posts %}
<img src="{{ post.image_path }}" style="max-width:100%;">
<br>
<br>
<a class="post-title" href="{{ post.url }}" style="display:block;font-family:'Nanum Gothic',Helvetica,Arial,sans-serif;font-size:18pt;line-height:22pt;padding-bottom:10px;">{{ post.title }}</a>
<p style="font-size:12pt;color:#666;margin:5px;">{{ post.content }}</p>
<br><br><hr><br><br>
{% endfor %}
<style>
 a.post-title {
   text-decoration: none;
   color: #000;
 }
 a.post-title:hover {
   text-decoration: none;
   color: #999;
 }
</style>
