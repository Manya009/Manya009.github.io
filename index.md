---
title: Home
layout: home
---
<link rel="stylesheet" href="/assets/css/style.css">
<div class="navbar">

<div><strong>Manish Patil</strong></div>

<div class="nav-links">
<a href="/">Home</a>
<a href="/projects">Projects</a>
<a href="/blog">Blog</a>
<a href="/about">About</a>
<a href="#contact">Contact</a>
<button onclick="toggleDark()">🌙</button>
</div>

</div>


<div class="hero">
<style>
.hero h1 {
  animation: fadeIn 1.2s ease;
}

@keyframes fadeIn {
  from {
    opacity: 0;
    transform: translateY(10px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}
</style>

<h1>Hi — I'm Manish Patil</h1>

<p><strong>AI / ML Engineer</strong> building models, experiments, and ML systems.</p>

<p>
📄 <a href="/resume.pdf" target="_blank">Resume</a> ·
💻 <a href="https://github.com/Manya009">GitHub</a> ·
🔗 <a href="https://www.linkedin.com/in manish-patil-1303aa215/">LinkedIn</a> ·
✍️ <a href="https://medium.com/@273manishp">Medium</a> ·
📊 <a href="https://www.kaggle.com/manishpatil009">Kaggle</a>
</p>

</div>


## Featured Projects

<div class="card-grid">

<div class="card">
<h3><a href="/projects/transformer-from-scratch">Transformer from Scratch</a></h3>
<p>Implemented a transformer architecture from scratch using PyTorch.</p>
</div>

<div class="card">
<h3><a href="/experiments/loss-landscape">Loss Landscape Visualizer</a></h3>
<p>Visualization tool for neural network loss landscapes.</p>
</div>

</div>



## Latest Writing

<div class="card-grid">

<div class="card">
<h3><a href="https://medium.com/@273manishp/loss-landscapes-part-1-325353f68e42">Loss Landscapes: Part 1</a></h3>
<p>Part 1 of learning basics of Deep learning by the perspective of Loss Landscapes.</p>
</div>

<div class="card">
<h3><a href="https://medium.com/@273manishp">More on Medium →</a></h3>
<p>Technical writing about ML, experiments, and learning notes.</p>
</div>

</div>

<script src="/assets/js/theme.js"></script>