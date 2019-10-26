---
layout: page
---

Hello! You  have reached the personal webpage of Leila Alimehr, this website is my personal space where
I put my ongoing activities.

Interested in Accounting and finaance. 

If you are interested in collaborating and doing some great work, please reach out to me via:

<div class="contact-buttons" style="line-height:160%;margin-left:30px;margin-top:10px">
<p>
<link rel="stylesheet" href="//maxcdn.bootstrapcdn.com/font-awesome/4.3.0/css/font-awesome.min.css">
<link rel="stylesheet" href="//leilaalimehr.github.io/css/academicons.css">
  <a href="mailto:leila.alimehr@gmail.com" target="_blank" style="color:#855f65;"><i class="fa fa-envelope" style="font-size:1em"></i> &nbsp; Email<br></a>
<a href="https://github.com/leilaalimehr" target="_blank" style="color:#0e5295;"><i class="fa fa-github" aria-hidden="true"></i> &nbsp; GitHub<br></a>
<a href="https://www.linkedin.com/in/leila-alimehr-23833a27/" target="_blank" style="color:#363636;"><i class="fa fa-linkedin" style="font-size:1em"></i> &nbsp; LinkedIn<br></a>
</p>
</div>

<br>



---
Leila Alimehr's Blog
---
<h1>{{ page.title }}</h1>
<h3>Accounting's blog: <a  href="https://leilaalimehr.github.io/accounting/">Accounting</a></h3>
<br>
<br>
<ul class="posts">

  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a></li>
  {% endfor %}
    
</ul>
