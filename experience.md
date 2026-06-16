---
title: Experience
layout: page
permalink: /experience/
---

<link rel="stylesheet" href="/assets/css/style.css">

<style>
/* ── Reference letter cards ─────────────────── */
.ref-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
  gap: 14px;
  margin-top: 4px;
}
.ref-card {
  background: var(--bg2);
  border: 1px solid var(--border);
  border-radius: var(--r-lg);
  padding: 20px;
  cursor: pointer;
  transition: border-color .2s, transform .2s, background .2s;
  display: flex;
  flex-direction: column;
  gap: 10px;
  position: relative;
  overflow: hidden;
}
.ref-card::after {
  content: '';
  position: absolute;
  inset: 0;
  background: radial-gradient(circle at top left, rgba(56,189,248,0.04), transparent 60%);
  pointer-events: none;
}
.ref-card:hover {
  border-color: rgba(56,189,248,0.3);
  transform: translateY(-2px);
  background: var(--bg3);
}
.ref-avatar {
  width: 44px; height: 44px;
  border-radius: 50%;
  background: var(--cyan-dim);
  border: 1px solid var(--border2);
  display: flex; align-items: center; justify-content: center;
  font-family: var(--font-head);
  font-weight: 700;
  font-size: 1rem;
  color: var(--accent2);
  flex-shrink: 0;
}
.ref-info { display: flex; flex-direction: column; gap: 2px; }
.ref-name  { font-family: var(--font-head); font-size: 0.95rem; font-weight: 600; color: var(--text-hi); }
.ref-title { font-size: 0.78rem; color: var(--muted); font-family: var(--font-mono); }
.ref-company { font-size: 0.78rem; color: var(--accent2); font-family: var(--font-mono); }
.ref-cta {
  margin-top: auto;
  display: inline-flex;
  align-items: center;
  gap: 6px;
  font-family: var(--font-mono);
  font-size: 0.72rem;
  color: var(--muted);
  border: 1px solid rgba(56,189,248,0.12);
  border-radius: 4px;
  padding: 5px 12px;
  transition: color .15s, border-color .15s, background .15s;
  width: fit-content;
}
.ref-card:hover .ref-cta {
  color: var(--accent2);
  border-color: var(--border2);
  background: var(--cyan-dim);
}
.ref-no-image {
  font-size: 0.78rem;
  color: var(--muted);
  font-style: italic;
  margin-top: 4px;
}

/* ── Lightbox ───────────────────────────────── */
.lightbox-overlay {
  display: none;
  position: fixed;
  inset: 0;
  z-index: 1000;
  background: rgba(5,12,26,0.92);
  backdrop-filter: blur(8px);
  align-items: flex-start;
  justify-content: center;
  padding: 24px;
  overflow-y: auto;
}
.lightbox-overlay.open { display: flex; }
.lightbox-inner {
  position: relative;
  max-width: 680px;
  width: 100%;
  margin: auto;
  padding-top: 48px;
  padding-bottom: 32px;
}
.lightbox-close {
  position: fixed;
  top: 20px;
  right: 28px;
  background: var(--bg3);
  border: 1px solid var(--border2);
  border-radius: var(--r);
  color: var(--muted);
  font-size: 0.78rem;
  font-family: var(--font-mono);
  padding: 6px 14px;
  cursor: pointer;
  transition: color .15s, background .15s;
  z-index: 1001;
  letter-spacing: 0.04em;
}
.lightbox-close:hover { color: var(--text-hi); background: var(--bg4); }
.lightbox-caption {
  margin-top: 14px;
  text-align: center;
  font-family: var(--font-mono);
  font-size: 0.72rem;
  color: var(--muted);
  letter-spacing: 0.03em;
}
.lightbox-loading {
  padding: 60px 40px;
  text-align: center;
  color: var(--muted);
  font-family: var(--font-mono);
  font-size: 0.78rem;
  letter-spacing: 0.04em;
}
.lightbox-no-pdf {
  background: var(--bg3);
  border: 1px dashed var(--border2);
  border-radius: var(--r-lg);
  padding: 60px 40px;
  text-align: center;
  color: var(--muted);
  font-size: 0.875rem;
  line-height: 1.7;
}
/* PDF canvas pages */
.pdf-page-canvas {
  width: 100%;
  display: block;
  border: 1px solid var(--border);
  user-select: none;
  -webkit-user-select: none;
}
.pdf-page-canvas:first-child { border-radius: var(--r-lg) var(--r-lg) 0 0; }
.pdf-page-canvas:last-child  { border-radius: 0 0 var(--r-lg) var(--r-lg); }
.pdf-page-canvas:only-child  { border-radius: var(--r-lg); }
.pdf-page-canvas + .pdf-page-canvas { border-top: none; }
</style>

<div class="site-wrap">

<nav class="navbar">
  <div class="container">
    <a href="/" class="nav-logo">Manish Patil</a>
    <div class="nav-links">
      <a href="/">Home</a>
      <a href="/experience/" class="active">Experience</a>
      <a href="/projects/">Projects</a>
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
        <h2>Experience</h2>
      </div>

      <div class="timeline">

        <div class="timeline-item">
          <div class="timeline-meta">
            <div class="timeline-date">Jun 2024 – Jul 2025</div>
            <div class="timeline-company">CypherSOL · Mumbai</div>
          </div>
          <div class="timeline-content">
            <h3>Data Scientist</h3>
            <ul>
              <li>Built end-to-end deep-learning OCR system automating financial document extraction across 50+ document types — drove ~10% sales uplift directly tied to commercial revenue</li>
              <li>Co-built <strong>CypherTrace</strong> — a forensic fund-tracing product covering FIFO-based tracing, flow-of-funds reconstruction, and risky transaction flagging; received external funding and helped crack a real money laundering case within its first month of deployment</li>
              <li>Designed forensic analytics pipelines (entity resolution, FIFO tracing, anomaly detection) deployed for Mumbai's Anti-Terrorism Squad and Economic Offences Wing; pitched the product to ATS and EOW officials alongside the CEO</li>
              <li>Architected scalable ETL pipeline processing 10,000+ monthly bank documents, improving extraction accuracy by 35% through advanced preprocessing and feature engineering</li>
              <li>Built FastAPI inference layer on AWS EC2 with Nginx load balancing — sub-2s latency under daily production traffic</li>
              <li>Instituted CI/CD practices (GitHub Actions, Docker, MLflow) reducing model drift by 40% and accelerating iteration cycles by 3×</li>
              <li>Mentored junior data scientists on annotation workflows, ML evaluation, and pipeline best practices; enforced privacy-first design across all systems handling sensitive financial and law enforcement data</li>
            </ul>
          </div>
        </div>

        <div class="timeline-item">
          <div class="timeline-meta">
            <div class="timeline-date">Apr 2023 – May 2024</div>
            <div class="timeline-company">CypherSOL · Mumbai</div>
          </div>
          <div class="timeline-content">
            <h3>Data Science Intern</h3>
            <ul>
              <li>Refactored the core financial data extraction pipeline architecture for improved scalability and accuracy across diverse unstructured document formats</li>
              <li>Built a regex-based entity classification system that outperformed ML approaches at early scale for noisy financial document data — became the foundation for the later hybrid NER system</li>
              <li>Automated bank statement analysis workflows, reducing manual processing time and supporting prototyping of new data models</li>
              <li>Reduced pipeline failure rates when processing unstructured financial documents, improving overall platform stability</li>
            </ul>
          </div>
        </div>

        <div class="timeline-item">
          <div class="timeline-meta">
            <div class="timeline-date">Jul 2023 – Nov 2023</div>
            <div class="timeline-company">Intel Corporation · Hybrid</div>
          </div>
          <div class="timeline-content">
            <h3>AI Intern</h3>
            <ul>
              <li>Built two production chatbots — a customer-support assistant and a crypto-portfolio manager — deployed as part of Intel's AI applied research teams</li>
              <li>Developed NLP and computer vision pipelines: sentiment analysis on 1,000+ feedback entries, text summarisation, and MTCNN-based person identification — improving model detection accuracy by 15%</li>
              <li>Standardised data preprocessing workflows and improved model detection accuracy through feature engineering</li>
            </ul>
          </div>
        </div>

      </div>
    </section>

    <!-- ── Letters of Reference ─────────────────── -->
    <section class="section">
      <div class="section-header">
        <h2>Letters of Reference</h2>
        <span class="count">2</span>
      </div>

      <p style="font-size:0.875rem; color:var(--muted); margin-bottom:28px; max-width:560px; line-height:1.75;">
        The following letters are from the leadership team at CypherSOL Fintech India Pvt Ltd, where I worked as a Data Scientist for over two years.
      </p>

      <div class="ref-grid">

        <div class="ref-card" onclick="openLightbox('ref-imran-sable')">
          <div style="display:flex; align-items:center; gap:14px;">
            <div class="ref-avatar">IS</div>
            <div class="ref-info">
              <div class="ref-name">Mr. Imran Sable</div>
              <div class="ref-title">Chief Executive Officer</div>
              <div class="ref-company">CypherSOL Fintech India Pvt Ltd</div>
            </div>
          </div>
          <div class="ref-cta">
            <svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round">
              <path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"/>
              <polyline points="14 2 14 8 20 8"/>
            </svg>
            View letter
          </div>
        </div>

        <div class="ref-card" onclick="openLightbox('ref-shamlata-poojary')">
          <div style="display:flex; align-items:center; gap:14px;">
            <div class="ref-avatar">SP</div>
            <div class="ref-info">
              <div class="ref-name">Ms. Shamlata Poojary</div>
              <div class="ref-title">Chief Technology Officer &amp; Managing Director</div>
              <div class="ref-company">CypherSOL Fintech India Pvt Ltd</div>
            </div>
          </div>
          <div class="ref-cta">
            <svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round">
              <path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"/>
              <polyline points="14 2 14 8 20 8"/>
            </svg>
            View letter
          </div>
        </div>

      </div>
    </section>

  </div>
</main>

<!-- ── Lightbox overlay ────────────────────────── -->
<div class="lightbox-overlay" id="lightbox" onclick="closeLightboxOnBackdrop(event)">
  <div class="lightbox-inner">
    <button class="lightbox-close" onclick="closeLightbox()">✕ close</button>
    <div id="lightbox-content"></div>
    <div class="lightbox-caption" id="lightbox-caption"></div>
  </div>
</div>

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

<!-- PDF.js — renders PDF to canvas so no browser download toolbar appears -->
<script src="https://cdnjs.cloudflare.com/ajax/libs/pdf.js/3.11.174/pdf.min.js"></script>
<script>
pdfjsLib.GlobalWorkerOptions.workerSrc =
  'https://cdnjs.cloudflare.com/ajax/libs/pdf.js/3.11.174/pdf.worker.min.js';

const refs = {
  'ref-imran-sable': {
    pdf: '/assets/img/references/ref-imran-sable.pdf',
    caption: 'Letter of Reference — Mr. Imran Sable, CEO · CypherSOL Fintech India Pvt Ltd'
  },
  'ref-shamlata-poojary': {
    pdf: '/assets/img/references/ref-shamlata-poojary.pdf',
    caption: 'Letter of Reference — Ms. Shamlata Poojary, CTO & MD · CypherSOL Fintech India Pvt Ltd'
  }
};

async function openLightbox(id) {
  const ref      = refs[id];
  const overlay  = document.getElementById('lightbox');
  const content  = document.getElementById('lightbox-content');
  const caption  = document.getElementById('lightbox-caption');

  overlay.classList.add('open');
  overlay.scrollTop = 0;
  document.body.style.overflow = 'hidden';
  caption.textContent = ref.caption;
  content.innerHTML   = '<div class="lightbox-loading">Loading…</div>';

  try {
    const pdf = await pdfjsLib.getDocument(ref.pdf).promise;
    content.innerHTML = '';

    for (let p = 1; p <= pdf.numPages; p++) {
      const page     = await pdf.getPage(p);
      // Scale to fill ~680px container width at 96dpi
      const baseVP   = page.getViewport({ scale: 1 });
      const scale    = 680 / baseVP.width * 1.8;
      const viewport = page.getViewport({ scale });

      const canvas   = document.createElement('canvas');
      canvas.width   = viewport.width;
      canvas.height  = viewport.height;
      canvas.className = 'pdf-page-canvas';

      // Block right-click and drag so the PDF can't be trivially saved
      canvas.addEventListener('contextmenu', e => e.preventDefault());
      canvas.addEventListener('dragstart',   e => e.preventDefault());

      await page.render({ canvasContext: canvas.getContext('2d'), viewport }).promise;
      content.appendChild(canvas);
    }
  } catch (err) {
    const filename = ref.pdf.split('/').pop();
    content.innerHTML =
      '<div class="lightbox-no-pdf">Letter not yet uploaded.<br>' +
      '<span style="font-size:0.78rem;font-family:var(--font-mono);color:var(--accent2);">' +
      'assets/img/references/' + filename + '</span></div>';
  }
}

function closeLightbox() {
  document.getElementById('lightbox').classList.remove('open');
  document.body.style.overflow = '';
  document.getElementById('lightbox-content').innerHTML = '';
}

function closeLightboxOnBackdrop(e) {
  if (e.target === document.getElementById('lightbox')) closeLightbox();
}

document.addEventListener('keydown', e => { if (e.key === 'Escape') closeLightbox(); });
</script>
