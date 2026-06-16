---
title: Projects
layout: page
permalink: /projects/
---

<link rel="stylesheet" href="/assets/css/style.css">

<style>
/* ── Filter bar ─────────────────────────────── */
.filter-bar {
  display: flex;
  flex-wrap: wrap;
  gap: 8px;
  margin-bottom: 36px;
}
.filter-btn {
  font-family: var(--font-mono);
  font-size: 0.75rem;
  color: var(--muted);
  background: transparent;
  border: 1px solid rgba(56,189,248,0.15);
  border-radius: var(--r);
  padding: 6px 14px;
  cursor: pointer;
  letter-spacing: 0.03em;
  transition: border-color .2s, color .2s, background .2s;
}
.filter-btn:hover,
.filter-btn.active {
  color: var(--accent2);
  border-color: var(--border2);
  background: var(--cyan-dim);
}

/* ── Project card extras ────────────────────── */
.card .card-metrics {
  margin-top: 14px;
  display: flex;
  flex-wrap: wrap;
  gap: 6px;
}
.metric {
  font-family: var(--font-mono);
  font-size: 0.7rem;
  color: var(--green);
  background: rgba(52,211,153,0.08);
  border: 1px solid rgba(52,211,153,0.2);
  border-radius: 4px;
  padding: 3px 8px;
}
.card-title-row {
  display: flex;
  align-items: flex-start;
  justify-content: space-between;
  gap: 10px;
  margin-bottom: 8px;
}
.card-title-row h3 { margin-bottom: 0; }
.card-gh-link {
  flex-shrink: 0;
  font-family: var(--font-mono);
  font-size: 0.7rem;
  color: var(--muted);
  border: 1px solid rgba(56,189,248,0.12);
  border-radius: 4px;
  padding: 3px 9px;
  transition: color .15s, border-color .15s;
  white-space: nowrap;
}
.card-gh-link:hover { color: var(--accent2); border-color: var(--border2); }
.card p { font-size: 0.88rem; color: var(--muted); line-height: 1.65; }
.card h3 {
  font-family: var(--font-head);
  font-size: 1rem;
  font-weight: 600;
  color: var(--text-hi);
  letter-spacing: -0.01em;
  line-height: 1.3;
}
.tag        { background: rgba(56,189,248,0.1); color: var(--accent2); border: 1px solid rgba(56,189,248,0.2); }
.tag.amber  { background: rgba(251,191,36,0.1); color: var(--amber);   border: 1px solid rgba(251,191,36,0.2); }
.tag.green  { background: rgba(52,211,153,0.1); color: var(--green);   border: 1px solid rgba(52,211,153,0.2); }
.tag.purple { background: rgba(167,139,250,0.1); color: #a78bfa;       border: 1px solid rgba(167,139,250,0.2); }
.tag {
  font-family: var(--font-mono);
  font-size: 0.7rem;
  border-radius: 4px;
  padding: 2px 8px;
  letter-spacing: 0.02em;
}

/* ── Project category hidden logic ─────────── */
.proj-card { display: block; }
.proj-card.hidden { display: none; }
</style>

<div class="site-wrap">

<nav class="navbar">
  <div class="container">
    <a href="/" class="nav-logo">Manish Patil</a>
    <div class="nav-links">
      <a href="/">Home</a>
      <a href="/experience/">Experience</a>
      <a href="/projects/" class="active">Projects</a>
      <a href="/education/">Education</a>
      <a href="/research/">Research</a>
      <a href="/about/">About</a>
    </div>
  </div>
</nav>

<main>
  <div class="container">
    <section class="section" style="border-top:none; padding-top: 56px;">
      <div class="section-header">
        <h2>Projects</h2>
        <span class="count">10</span>
      </div>

      <div class="filter-bar">
        <button class="filter-btn active" data-filter="all">All</button>
        <button class="filter-btn" data-filter="llm">AI / LLM</button>
        <button class="filter-btn" data-filter="backend">Backend</button>
        <button class="filter-btn" data-filter="data">Data Science</button>
      </div>

      <div class="card-grid">

        <!-- ── 1. Nexus ─────────────────────────── -->
        <div class="card proj-card" data-category="llm">
          <div class="card-tags">
            <span class="tag">LangGraph</span>
            <span class="tag">MCP</span>
            <span class="tag">LangSmith</span>
            <span class="tag amber">Agentic AI</span>
          </div>
          <div class="card-title-row">
            <h3>Nexus — Agentic Research Platform</h3>
            <a href="https://github.com/Manya009" target="_blank" class="card-gh-link">↗ GitHub</a>
          </div>
          <p>Enterprise-grade multi-agent research system built with LangGraph and Pydantic for structured, stable agentic orchestration across local filesystems and external APIs.</p>
          <div class="card-metrics">
            <span class="metric">Sub-500ms RAG latency</span>
            <span class="metric">25% ↓ hallucination rate</span>
            <span class="metric">Reproducible CI/CD releases</span>
          </div>
        </div>

        <!-- ── 2. Shakti ────────────────────────── -->
        <div class="card proj-card" data-category="llm">
          <div class="card-tags">
            <span class="tag">RAG</span>
            <span class="tag">FastAPI</span>
            <span class="tag">AWS EC2</span>
            <span class="tag green">SIH Finalist</span>
          </div>
          <div class="card-title-row">
            <h3>Shakti — Expert RAG Chatbot</h3>
            <a href="https://github.com/Manya009" target="_blank" class="card-gh-link">↗ GitHub</a>
          </div>
          <p>Production RAG chatbot for electrical substation maintenance queries over 500+ technical documents. Built for Smart India Hackathon 2024 National Finals and deployed on AWS EC2.</p>
          <div class="card-metrics">
            <span class="metric">60% ↓ query resolution time</span>
            <span class="metric">85% retrieval accuracy</span>
            <span class="metric">200+ concurrent users &lt;2s</span>
          </div>
        </div>

        <!-- ── 3. Studios AI ────────────────────── -->
        <div class="card proj-card" data-category="llm">
          <div class="card-tags">
            <span class="tag">GPT-4</span>
            <span class="tag">Stable Diffusion XL</span>
            <span class="tag">Django</span>
            <span class="tag amber">Published</span>
          </div>
          <div class="card-title-row">
            <h3>Studios AI — Creative Content Platform</h3>
            <a href="https://github.com/Manya009" target="_blank" class="card-gh-link">↗ GitHub</a>
          </div>
          <p>AI platform integrating GPT-4 and Stable Diffusion XL for professional story, poetry, and image generation. Includes a custom prompt engineering framework and content moderation pipeline. Research published in JETIR (Impact Factor 7.95).</p>
          <div class="card-metrics">
            <span class="metric">75% ↓ prototyping time</span>
            <span class="metric">99% safe generation rate</span>
            <span class="metric">JETIR IF 7.95</span>
          </div>
        </div>

        <!-- ── 4. CuisineRAG Plus ─────────────── -->
        <div class="card proj-card" data-category="llm">
          <div class="card-tags">
            <span class="tag">GraphRAG</span>
            <span class="tag">Knowledge Graphs</span>
            <span class="tag">BM25</span>
            <span class="tag purple">Research</span>
          </div>
          <div class="card-title-row">
            <h3>CuisineRAG Plus — GraphRAG Extension</h3>
            <a href="https://github.com/Manya009" target="_blank" class="card-gh-link">↗ GitHub</a>
          </div>
          <p>Extended the CuisineRAG hybrid RAG system with a GraphRAG layer to enable relational reasoning across entities — ingredients, techniques, and dishes — that flat vector search cannot capture. Benchmarked against non-RAG and hybrid RAG baselines using ROUGE, BERTScore, and MRR.</p>
          <div class="card-metrics">
            <span class="metric">Multi-hop reasoning</span>
            <span class="metric">ROUGE / BERTScore / MRR eval</span>
          </div>
        </div>

        <!-- ── 5. CuisineRAG ─────────────────── -->
        <div class="card proj-card" data-category="llm">
          <div class="card-tags">
            <span class="tag">Hybrid Search</span>
            <span class="tag">FAISS</span>
            <span class="tag">HuggingFace</span>
            <span class="tag">Reranking</span>
          </div>
          <div class="card-title-row">
            <h3>CuisineRAG — Hybrid RAG System</h3>
            <a href="https://github.com/Manya009" target="_blank" class="card-gh-link">↗ GitHub</a>
          </div>
          <p>Production-grade hybrid RAG combining dense retrieval (FAISS + MiniLM/Qwen) with BM25 sparse retrieval via Reciprocal Rank Fusion. Cross-encoder reranker delivered the largest single accuracy improvement. Rigorously evaluated against non-RAG baseline across six metrics.</p>
          <div class="card-metrics">
            <span class="metric">Dense + sparse + reranking</span>
            <span class="metric">BLEU / Precision@K / Recall@K</span>
          </div>
        </div>

        <!-- ── 6. Ticket Management System ────── -->
        <div class="card proj-card" data-category="backend">
          <div class="card-tags">
            <span class="tag">FastAPI</span>
            <span class="tag">XGBoost</span>
            <span class="tag">Docker Compose</span>
            <span class="tag">JWT / RBAC</span>
          </div>
          <div class="card-title-row">
            <h3>Ticket Management System</h3>
            <a href="https://github.com/Manya009" target="_blank" class="card-gh-link">↗ GitHub</a>
          </div>
          <p>Full-stack ML-powered ticket management system with XGBoost priority prediction integrated asynchronously via Celery, JWT authentication with Redis-backed token revocation, and production multi-service deployment via Docker Compose.</p>
          <div class="card-metrics">
            <span class="metric">7 services / 3 FastAPI instances</span>
            <span class="metric">Async ML inference via Celery</span>
            <span class="metric">Nginx load balancing</span>
          </div>
        </div>

        <!-- ── 7. Telco Churn Prediction ──────── -->
        <div class="card proj-card" data-category="backend">
          <div class="card-tags">
            <span class="tag">XGBoost</span>
            <span class="tag">MLflow</span>
            <span class="tag">FastAPI</span>
            <span class="tag">Gradio</span>
          </div>
          <div class="card-title-row">
            <h3>Telco Churn Prediction Pipeline</h3>
            <a href="https://github.com/Manya009" target="_blank" class="card-gh-link">↗ GitHub</a>
          </div>
          <p>End-to-end churn prediction system with XGBoost, MLflow experiment tracking for full reproducibility, FastAPI model serving, Gradio UI for interactive testing, and a fully automated CI/CD pipeline pushing Docker images to Docker Hub on every commit.</p>
          <div class="card-metrics">
            <span class="metric">Full MLflow reproducibility</span>
            <span class="metric">Auto CI/CD to Docker Hub</span>
          </div>
        </div>

        <!-- ── 8. Ticket Classification ────────── -->
        <div class="card proj-card" data-category="data">
          <div class="card-tags">
            <span class="tag">NLP</span>
            <span class="tag">scikit-learn</span>
            <span class="tag">W&amp;B</span>
            <span class="tag">Text Classification</span>
          </div>
          <div class="card-title-row">
            <h3>Support Ticket Classification</h3>
            <a href="https://github.com/Manya009" target="_blank" class="card-gh-link">↗ GitHub</a>
          </div>
          <p>Rigorous multi-class text classification project focused on systematic model comparison — from classical ML baselines to gradient boosting — with documented failure modes at each stage. All experiments tracked on Weights & Biases with cross-fold statistical analysis.</p>
          <div class="card-metrics">
            <span class="metric">Statistical cross-validation</span>
            <span class="metric">W&amp;B experiment tracking</span>
          </div>
        </div>

        <!-- ── 9. E-Commerce EDA ───────────────── -->
        <div class="card proj-card" data-category="data">
          <div class="card-tags">
            <span class="tag">EDA</span>
            <span class="tag">A/B Testing</span>
            <span class="tag">Hypothesis Testing</span>
            <span class="tag">RFM Segmentation</span>
          </div>
          <div class="card-title-row">
            <h3>E-Commerce Customer Behaviour Analysis</h3>
            <a href="https://github.com/Manya009" target="_blank" class="card-gh-link">↗ GitHub</a>
          </div>
          <p>End-to-end data science project on the Olist Brazilian E-Commerce dataset (100,000+ orders). Covers EDA, A/B test design with statistical power analysis, five hypothesis tests with Bonferroni correction, RFM customer segmentation, and business KPI dashboard — communicated as a business-facing report.</p>
          <div class="card-metrics">
            <span class="metric">100,000+ orders</span>
            <span class="metric">5 validated hypotheses</span>
            <span class="metric">8 business KPIs</span>
          </div>
        </div>

        <!-- ── 10. Power BI Fraud Dashboard ────── -->
        <div class="card proj-card" data-category="data">
          <div class="card-tags">
            <span class="tag">Power BI</span>
            <span class="tag">SHAP</span>
            <span class="tag">Fraud Detection</span>
            <span class="tag amber">Fintech</span>
          </div>
          <div class="card-title-row">
            <h3>Fraud Detection &amp; Risk Analytics Dashboard</h3>
            <a href="https://github.com/Manya009" target="_blank" class="card-gh-link">↗ GitHub</a>
          </div>
          <p>Real-time interactive fraud detection command centre in Power BI translating ML model outputs and SHAP explainability into actionable insights for risk and fraud teams. Advanced Power Query data modelling with schema mismatch resolution. Heavy calculations pushed upstream to Python for production-grade performance.</p>
          <div class="card-metrics">
            <span class="metric">SHAP explainability layer</span>
            <span class="metric">Real-time interactive dashboard</span>
            <span class="metric">Multi-dataset Power Query model</span>
          </div>
        </div>

      </div><!-- /card-grid -->
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

<script>
(function () {
  const btns  = document.querySelectorAll('.filter-btn');
  const cards = document.querySelectorAll('.proj-card');

  btns.forEach(btn => {
    btn.addEventListener('click', () => {
      btns.forEach(b => b.classList.remove('active'));
      btn.classList.add('active');

      const filter = btn.dataset.filter;
      cards.forEach(card => {
        if (filter === 'all' || card.dataset.category === filter) {
          card.classList.remove('hidden');
        } else {
          card.classList.add('hidden');
        }
      });
    });
  });
})();
</script>
