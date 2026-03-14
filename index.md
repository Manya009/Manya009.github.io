---
title: Home
layout: home
---

<link rel="stylesheet" href="/assets/css/style.css">

<div class="container">

<div class="navbar">
<div class="logo">Manish Patil</div>

<div class="nav-links">
<a href="/">Home</a>
<a href="/projects">Projects</a>
<a href="/research">Research</a>
<a href="/experience">Experience</a>
<a href="/education">Education</a>
<a href="/about">About</a>
</div>
</div>

<div class="hero">

<img src="/assets/img/profile.jpg" class="profile">

<div class="hero-text">

<h1>Manish Patil</h1>

<p class="subtitle">
AI / ML Engineer building models, experiments and ML systems.
</p>

<p>
📄 <a href="/resume.pdf">Resume</a> ·
💻 <a href="https://github.com/Manya009">GitHub</a> ·
🔗 <a href="https://www.linkedin.com/in/manish-patil-1303aa215/">LinkedIn</a> ·
✍️ <a href="https://medium.com/@273manishp">Medium</a> ·
📊 <a href="https://www.kaggle.com/manishpatil009">Kaggle</a>
</p>

</div>

</div>


<div class="section">

<h2>Featured Projects</h2>

<div class="card-grid">

{% for project in site.projects limit:3 %}

<div class="card">

<h3>
<a href="{{ project.url }}">{{ project.title }}</a>
</h3>

<p>{{ project.description }}</p>

</div>

{% endfor %}

</div>

</div>


<div class="section">

<h2>Latest Writing</h2>

<div class="card-grid">

{% for post in site.posts limit:2 %}

<div class="card">

<h3>
<a href="{{ post.url }}">{{ post.title }}</a>
</h3>

<p>{{ post.excerpt }}</p>

</div>

{% endfor %}

<div class="card">

<h3>
<a href="https://medium.com/@273manishp">
More on Medium →
</a>
</h3>

<p>Technical writing about ML systems and research.</p>

</div>

</div>

</div>

</div>