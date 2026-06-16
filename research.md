---
title: Research
layout: page
permalink: /research/
---

<link rel="stylesheet" href="/assets/css/style.css">

<div class="site-wrap">

<nav class="navbar">
  <div class="container">
    <a href="/" class="nav-logo">Manish Patil</a>
    <div class="nav-links">
      <a href="/">Home</a>
      <a href="/experience/">Experience</a>
      <a href="/projects/">Projects</a>
      <a href="/education/">Education</a>
      <a href="/research/" class="active">Research</a>
      <a href="/about/">About</a>
    </div>
  </div>
</nav>

<main>
  <div class="container">
    <section class="section" style="border-top:none; padding-top: 56px;">
      <div class="section-header">
        <h2>Research &amp; Publications</h2>
        <span class="count">2</span>
      </div>

      <!-- ── MSc Dissertation (In Progress) ──── -->
      <div class="pub-card" style="margin-bottom: 20px;">
        <div class="card-tags" style="margin-bottom:14px;">
          <span class="tag" style="background:rgba(52,211,153,0.1); color:#34d399; border:1px solid rgba(52,211,153,0.2);">In Progress</span>
          <span class="tag">MSc Dissertation</span>
          <span class="tag">PAC-Bayes</span>
          <span class="tag">Probabilistic Deep Learning</span>
        </div>

        <h3>Certifying Deep Learning Classifier Predictions with High Confidence</h3>

        <p style="margin-top:10px;">
          This dissertation investigates an alternative paradigm for training neural networks in which each weight
          learns a <em>probability distribution</em> rather than a single fixed value — capturing both the most
          likely weight and the uncertainty around it. The work applies <strong style="color:var(--text-hi); font-weight:500;">PAC-Bayes theory</strong>,
          a framework from statistical learning theory, to train these probabilistic networks and derive
          <strong style="color:var(--text-hi); font-weight:500;">risk certificates</strong> — mathematically rigorous bounds on
          how well the model is expected to generalise to unseen data.
        </p>

        <p style="margin-top:12px; font-size:0.875rem; color:var(--muted); line-height:1.75;">
          Unlike standard deep learning, where a trained model provides no formal guarantee about future
          performance, PAC-Bayes bounds offer provable statistical guarantees. The central question is whether
          probabilistic neural networks trained under this framework can simultaneously achieve high predictive
          accuracy <em>and</em> produce reliable, non-vacuous guarantees.
        </p>

        <p><strong style="color:var(--text-hi); font-weight:500; display:block; margin-top:16px;">Research contributions:</strong></p>
        <ul style="list-style:none; display:flex; flex-direction:column; gap:8px; margin-top:8px;">
          <li style="font-size:0.875rem; color:var(--muted); padding-left:16px; position:relative;">
            <span style="position:absolute;left:0;color:var(--accent);">›</span>
            Reproducing published PAC-Bayes training results on MNIST to validate the theoretical framework against prior work
          </li>
          <li style="font-size:0.875rem; color:var(--muted); padding-left:16px; position:relative;">
            <span style="position:absolute;left:0;color:var(--accent);">›</span>
            Extending experiments to FashionMNIST and additional datasets to assess how the framework holds under distribution shift and increased task difficulty
          </li>
          <li style="font-size:0.875rem; color:var(--muted); padding-left:16px; position:relative;">
            <span style="position:absolute;left:0;color:var(--accent);">›</span>
            Evaluating the tightness and practical utility of the derived risk certificates — are the bounds informative enough to be useful, or do they collapse to vacuous guarantees?
          </li>
          <li style="font-size:0.875rem; color:var(--muted); padding-left:16px; position:relative;">
            <span style="position:absolute;left:0;color:var(--accent);">›</span>
            Analysing the accuracy–certificate trade-off: understanding when and why tighter guarantees come at the cost of predictive performance
          </li>
        </ul>

        <div style="margin-top: 18px; display: flex; flex-wrap: wrap; gap: 8px;">
          <span style="font-family:var(--font-mono); font-size:0.7rem; color:var(--muted); background:var(--bg3); border:1px solid var(--border); border-radius:4px; padding:3px 9px;">Bayesian Deep Learning</span>
          <span style="font-family:var(--font-mono); font-size:0.7rem; color:var(--muted); background:var(--bg3); border:1px solid var(--border); border-radius:4px; padding:3px 9px;">Statistical Learning Theory</span>
          <span style="font-family:var(--font-mono); font-size:0.7rem; color:var(--muted); background:var(--bg3); border:1px solid var(--border); border-radius:4px; padding:3px 9px;">Generalisation Bounds</span>
          <span style="font-family:var(--font-mono); font-size:0.7rem; color:var(--muted); background:var(--bg3); border:1px solid var(--border); border-radius:4px; padding:3px 9px;">PyTorch</span>
          <span style="font-family:var(--font-mono); font-size:0.7rem; color:var(--muted); background:var(--bg3); border:1px solid var(--border); border-radius:4px; padding:3px 9px;">MNIST · FashionMNIST</span>
          <span style="font-family:var(--font-mono); font-size:0.7rem; color:var(--muted); background:var(--bg3); border:1px solid var(--border); border-radius:4px; padding:3px 9px;">Uncertainty Quantification</span>
        </div>

        <div class="pub-meta" style="margin-top:20px;">
          <strong style="color:var(--text-hi);">University of Manchester</strong> — MSc Artificial Intelligence<br>
          Global Future Scholar · Expected completion: September 2026
        </div>
      </div>

      <div class="pub-card">
        <div class="card-tags" style="margin-bottom:14px;">
          <span class="tag amber">Published</span>
          <span class="tag">GenAI</span>
          <span class="tag">Creative AI</span>
        </div>

        <h3 style="display:flex; align-items:center; gap:10px;">
          STUDIOS AI: AI-Powered Creative Content Generation Platform
          <a href="https://www.jetir.org/view?paper=JETIR2404742" target="_blank"
             title="Open paper"
             style="display:inline-flex; align-items:center; justify-content:center; width:26px; height:26px; border-radius:5px; border:1px solid var(--border2); color:var(--accent2); background:var(--cyan-dim); flex-shrink:0; transition:background .15s, border-color .15s;"
             onmouseover="this.style.background='rgba(56,189,248,0.22)'; this.style.borderColor='var(--accent2)'"
             onmouseout="this.style.background='var(--cyan-dim)'; this.style.borderColor='var(--border2)'">
            <svg width="13" height="13" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round">
              <path d="M18 13v6a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V8a2 2 0 0 1 2-2h6"/>
              <polyline points="15 3 21 3 21 9"/>
              <line x1="10" y1="14" x2="21" y2="3"/>
            </svg>
          </a>
        </h3>

        <p>Explores an AI system capable of generating professional stories, poetry, and images from text prompts. The platform integrates GPT-3.5/4 and Stable Diffusion XL to democratise creative content generation for non-technical users.</p>

        <p><strong style="color:var(--text-hi); font-weight:500;">Key contributions:</strong></p>
        <ul style="list-style:none; display:flex; flex-direction:column; gap:8px; margin-top:8px;">
          <li style="font-size:0.875rem; color:var(--muted); padding-left:16px; position:relative;">
            <span style="position:absolute;left:0;color:var(--accent);">›</span>
            Developed a custom prompt engineering framework and content moderation system
          </li>
          <li style="font-size:0.875rem; color:var(--muted); padding-left:16px; position:relative;">
            <span style="position:absolute;left:0;color:var(--accent);">›</span>
            Achieved 99% safe content generation rate
          </li>
          <li style="font-size:0.875rem; color:var(--muted); padding-left:16px; position:relative;">
            <span style="position:absolute;left:0;color:var(--accent);">›</span>
            Improved content relevance scores by 45%
          </li>
          <li style="font-size:0.875rem; color:var(--muted); padding-left:16px; position:relative;">
            <span style="position:absolute;left:0;color:var(--accent);">›</span>
            Reduced creative prototyping time by 75%, enabling 10× faster professional content generation
          </li>
        </ul>

        <div class="pub-meta">
          <strong style="color:var(--text-hi);">JETIR</strong> — Journal of Emerging Technologies and Innovative Research<br>
          UGC Approved · Journal No. 63975 · Impact Factor 7.95 · Volume 11, Issue 4
        </div>
      </div>

    </section>
  </div>
</main>

<footer class="site-footer">
  <div class="container">
    <span class="footer-copy">© 2026 Manish Patil</span>
    <div class="footer-links">
      <a href="https://github.com/Manya009" target="_blank">GitHub</a>
      <a href="https://www.linkedin.com/in/manish-patil-1303aa215/" target="_blank">LinkedIn</a>
      <a href="mailto:273manishp@gmail.com">Email</a>
    </div>
  </div>
</footer>

</div>