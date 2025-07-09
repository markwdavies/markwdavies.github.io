---
title: Home Page
layout: default
---

# {{ page.title }}
This site is a github Pages hosted site to document my <a href="https://github.com/markwdavies" class="btn btn-github"><span class="icon"></span>code repos on github</a>  ...
<div>
<p>Details of my <a href="{% post_url 2023-11-28-RepoContents %}" class="btn">Stored Procs repository</a></p>
</div>

<p><h2>Latest Posts</h2></p>
<div>
    <table class="table table-primary table-striped text-start">
    {% tablerow post in site.posts cols:1 limit:5 %} 
      {{ post.date | date: "%-d %b %Y" }} <a href="{{ post.url }}">{{ post.title }}</a>
    {% endtablerow %}
    </table>
</div>
