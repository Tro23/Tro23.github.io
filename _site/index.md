---
layout: default
title: My Projects
---

# Welcome to Tro23's GitHub Projects

<nav>
    <a href="/">Home</a> |
    <a href="/projects/">Projects</a> |
    <a href="/blog/">Blog</a>
</nav>

## My Projects
<ul>
   {% for project in site.data.projects %}
    <li>
        <a href="{{ project.url }}"><strong>{{ project.name }}</strong></a>: {{ project.description }}
    </li>
    {% endfor %}
</ul>

<h3>Site Data Debugging</h3>
<pre>{{ site.data | jsonify }}</pre>

<footer>
    <p>&copy; 2024 Rohit T. Built with Jekyll.</p>
</footer>


