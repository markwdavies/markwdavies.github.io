---
title: Home Page
layout: default
---

# {{ page.title }}
This site has been set up as a github hosted site to document my <a href="https://github.com/markwdavies" class="btn btn-github"><span class="icon"></span>code repos on github</a> and maybe some other stuff as well.
Currently a work in progress ...
<div>
<p>Details of my <a href="{% post_url 2023-11-28-RepoContents %}" class="btn">Stored Procs repository</a></p>
</div>

<p><h2>All Posts</h2></p>
<div>
    <table class="table table-primary table-striped text-start">
    {% tablerow post in site.posts cols:1 %} 
      {{ post.date | date: "%-d %b %Y" }} <a href="{{ post.url }}">{{ post.title }}</a>
    {% endtablerow %}
    </table>
</div>
