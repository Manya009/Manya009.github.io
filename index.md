---
title: Home
layout: home
---

<div class="site-wrap">

<nav class="navbar">
  <div class="container">
    <span class="nav-logo">Manish Patil</span>
    <div class="nav-links">
      <a href="/" class="active">Home</a>
      <a href="/projects/">Projects</a>
      <a href="/research/">Research</a>
      <a href="/experience/">Experience</a>
      <a href="/education/">Education</a>
      <a href="/about/">About</a>
    </div>
  </div>
</nav>

<main>
  <div class="container">

    <!-- ── Hero ──────────────────────────── -->
    <section class="hero">
      <div class="hero-text">

        <div class="hero-tag">MSc AI · University of Manchester</div>

        <h1>Manish<br><span>Patil</span></h1>

        <p class="hero-bio">
          <strong>AI / ML Engineer</strong> building production-grade ML systems —
          OCR pipelines, RAG chatbots, agentic platforms, and forensic analytics.
          Currently reading <strong>MSc AI at Manchester</strong> on a Global Future Scholarship.
        </p>

        <div class="hero-links">
          <a href="/resume.pdf">📄 Resume</a>
          <a href="https://github.com/Manya009" target="_blank">⌥ GitHub</a>
          <a href="https://www.linkedin.com/in/manish-patil-1303aa215/" target="_blank">in LinkedIn</a>
          <a href="https://medium.com/@273manishp" target="_blank">✍ Medium</a>
          <a href="https://www.kaggle.com/manishpatil009" target="_blank">⬡ Kaggle</a>
        </div>

        <div class="hero-stats">
          <div class="stat-item">
            <span class="stat-num">2+</span>
            <span class="stat-label">yrs industry</span>
          </div>
          <div class="stat-item">
            <span class="stat-num">50+</span>
            <span class="stat-label">doc types</span>
          </div>
          <div class="stat-item">
            <span class="stat-num">10k+</span>
            <span class="stat-label">docs/month</span>
          </div>
        </div>

      </div>

      <div class="hero-avatar">
        <div class="avatar-ring">
          <div class="avatar-inner">
            <img src="/assets/img/profile.jpeg" alt="Manish Patil"
                 onerror="this.style.display='none';this.nextElementSibling.style.display='flex'">
            <span class="avatar-fallback" style="display:none">MP</span>
          </div>
        </div>
        <div class="avatar-badge">🎓 Global Future Scholar</div>
      </div>
    </section>

    <!-- ── Featured Projects ──────────────── -->
    <section class="section">
      <div class="section-header">
        <h2>Featured Projects</h2>
        <a href="/projects/" class="see-all">All projects →</a>
      </div>

      <div class="card-grid">

        <div class="card">
          <div class="card-tags">
            <span class="tag">LangGraph</span>
            <span class="tag">MCP</span>
            <span class="tag amber">2026</span>
          </div>
          <h3>Nexus — Agentic Research Platform</h3>
          <p>Multi-agent system for autonomous research and report generation. Uses LangGraph + Pydantic for stability, MCP for secure tool-calling, and LangSmith for observability — reducing hallucination by 25%.</p>
        </div>

        <div class="card">
          <div class="card-tags">
            <span class="tag">RAG</span>
            <span class="tag">FastAPI</span>
            <span class="tag green">Hackathon</span>
          </div>
          <h3>Shakti — Expert RAG Chatbot</h3>
          <p>Production RAG chatbot for electrical substation queries. Reached Smart India Hackathon Finals. Cut query resolution time 60%, deployed on AWS EC2 supporting 200+ concurrent users at &lt;2s latency.</p>
        </div>

        <div class="card">
          <div class="card-tags">
            <span class="tag">GPT-4</span>
            <span class="tag">Stable Diffusion</span>
            <span class="tag amber">Published</span>
          </div>
          <h3>Studios AI — Content Generation</h3>
          <p>AI platform generating stories, poetry, and images from text prompts. 75% reduction in creative prototyping time, 99% safe generation rate, published in JETIR (Impact Factor 7.95).</p>
        </div>

      </div>
    </section>

    <!-- ── Skills ────────────────────────── -->
    <section class="section">
      <div class="section-header">
        <h2>Technical Skills</h2>
      </div>
      <div class="skills-grid">
        <span class="skill-pill">Python</span>
        <span class="skill-pill">PyTorch</span>
        <span class="skill-pill">TensorFlow</span>
        <span class="skill-pill">LangChain</span>
        <span class="skill-pill">LangGraph</span>
        <span class="skill-pill">FastAPI</span>
        <span class="skill-pill">Django</span>
        <span class="skill-pill">RAG Pipelines</span>
        <span class="skill-pill">Vector DBs</span>
        <span class="skill-pill">NLP</span>
        <span class="skill-pill">Computer Vision</span>
        <span class="skill-pill">MCP</span>
        <span class="skill-pill">Docker</span>
        <span class="skill-pill">AWS</span>
        <span class="skill-pill">CI/CD</span>
        <span class="skill-pill">SQL</span>
        <span class="skill-pill">Pandas</span>
        <span class="skill-pill">HuggingFace</span>
        <span class="skill-pill">Pydantic</span>
        <span class="skill-pill">OCR</span>
      </div>
    </section>

    <!-- ── Latest Writing ─────────────────── -->
    <section class="section">
      <div class="section-header">
        <h2>Latest Writing</h2>
      </div>
      <div class="card-grid">

        {% if site.data.medium_posts and site.data.medium_posts.size > 0 %}
          {% for post in site.data.medium_posts %}
          <div class="card">
            <div class="card-tags"><span class="tag">Medium</span></div>
            <h3><a href="{{ post.url }}" target="_blank">{{ post.title }}</a></h3>
            <p>{{ post.description }}</p>
          </div>
          {% endfor %}
        {% endif %}

        <div class="card">
          <div class="card-tags"><span class="tag">Medium</span></div>
          <h3><a href="https://medium.com/@273manishp" target="_blank">More on Medium →</a></h3>
          <p>Technical writing on ML systems, RAG architectures, and AI engineering in production.</p>
        </div>

      </div>
    </section>

  </div>
</main>

<footer class="site-footer">
  <div class="container">
    <span class="footer-copy">© 2025 Manish Patil</span>
    <div class="footer-links">
      <a href="https://github.com/Manya009" target="_blank">GitHub</a>
      <a href="https://www.linkedin.com/in/manish-patil-1303aa215/" target="_blank">LinkedIn</a>
      <a href="mailto:273manishp@gmail.com">Email</a>
    </div>
  </div>
</footer>

</div>