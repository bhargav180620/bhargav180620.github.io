<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Bhargav Bhandari — Data Engineer</title>
  <meta name="description" content="Bhargav Bhandari — Data Engineer. Building scalable data platforms, ETL, observability and infra for ML & analytics." />
  <meta property="og:title" content="Bhargav Bhandari — Data Engineer" />
  <meta property="og:description" content="Data Engineer focusing on pipelines, Kafka, Debezium, Spark, Dagster and Kubernetes." />
  <meta property="og:type" content="website" />
  
  <style>
    :root{
      --bg:#0a0e27;
      --card:#0f1629;
      --muted:#94a3b8;
      --accent:#06b6d4;
      --accent-hover:#0891b2;
      --glass: rgba(255,255,255,0.05);
      --text:#f1f5f9;
      --radius:16px;
      --maxw:1200px;
      font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
    }
    @keyframes gradientShift { 0%, 100% { background-position: 0% 50%; } 50% { background-position: 100% 50%; } }
    @keyframes float { 0%, 100% { transform: translateY(0px); } 50% { transform: translateY(-20px); } }
    @keyframes fadeInUp { from { opacity: 0; transform: translateY(30px);} to { opacity: 1; transform: translateY(0);} }
    @keyframes scaleIn { from { opacity: 0; transform: scale(0.95);} to { opacity: 1; transform: scale(1);} }
    * { box-sizing: border-box; margin: 0; padding: 0; }
    html { scroll-behavior: smooth; }
    body {
      margin: 0; min-height: 100vh; background: radial-gradient(circle at 20% 20%, rgba(6, 182, 212, 0.08) 0%, transparent 50%), radial-gradient(circle at 80% 80%, rgba(139, 92, 246, 0.06) 0%, transparent 50%), var(--bg);
      background-size: 100% 100%; animation: gradientShift 20s ease infinite; color: var(--text); -webkit-font-smoothing: antialiased; padding: 0; overflow-x: hidden;
    }
    .particles { position: fixed; top: 0; left: 0; width: 100%; height: 100%; pointer-events: none; z-index: 0; }
    .particle { position: absolute; background: radial-gradient(circle, rgba(6, 182, 212, 0.3), transparent); border-radius: 50%; animation: float 6s ease-in-out infinite; will-change: transform, opacity; }
    .particle[data-size="s"]{ width:4px; height:4px; }
    .particle[data-size="m"]{ width:8px; height:8px; }
    .particle[data-size="l"]{ width:14px; height:14px; }

    .wrap { position: relative; z-index: 1; width: 100%; max-width: var(--maxw); margin: 0 auto; padding: 20px; }
    header { display: flex; align-items: center; justify-content: space-between; padding: 20px 0; margin-bottom: 40px; animation: fadeInUp 0.8s ease; }
    .brand { display: flex; gap: 16px; align-items: center; }
    .logo { width: 60px; height: 60px; border-radius: 16px; background: linear-gradient(135deg, var(--accent), #8b5cf6); display: flex; align-items: center; justify-content: center; color: #fff; font-weight: 800; font-size: 24px; box-shadow: 0 10px 30px rgba(6, 182, 212, 0.3); transition: transform 0.18s ease, box-shadow 0.18s ease; cursor: grab; user-select: none; }
    .logo:active{ cursor: grabbing; }
    .brand-text h2 { font-size: 20px; margin-bottom: 2px; background: linear-gradient(135deg, var(--accent), #8b5cf6); -webkit-background-clip: text; -webkit-text-fill-color: transparent; background-clip: text; }
    .brand-text p { color: var(--muted); font-size: 13px; }
    nav { display: flex; gap: 24px; align-items: center; }
    nav a { color: var(--muted); text-decoration: none; font-weight: 500; transition: color 0.25s ease; position: relative; }
    nav a:hover { color: var(--accent); }
    nav a::after { content: ''; position: absolute; bottom: -4px; left: 0; width: 0; height: 2px; background: var(--accent); transition: width 0.3s ease; }
    nav a:hover::after { width: 100%; }
    .resume-btn { padding: 10px 20px; background: var(--glass); border: 1px solid rgba(6, 182, 212, 0.2); border-radius: 12px; color: var(--accent); font-weight: 600; transition: all 0.3s ease; }
    .resume-btn:hover { background: var(--accent); color: var(--bg); transform: translateY(-2px); box-shadow: 0 10px 25px rgba(6, 182, 212, 0.3); }

    /* Hero Section */
    .hero { display: grid; grid-template-columns: 1fr 380px; gap: 40px; margin-bottom: 60px; animation: fadeInUp 1s ease 0.2s backwards; }
    .hero-content { display: flex; flex-direction: column; justify-content: center; transform-origin: center; will-change: transform; }
    .hero h1 { font-size: clamp(2.5rem, 5vw, 4rem); margin-bottom: 20px; line-height: 1.1; background: linear-gradient(135deg, #fff 0%, var(--accent) 100%); -webkit-background-clip: text; -webkit-text-fill-color: transparent; background-clip: text; }
    .hero .tagline { font-size: clamp(1.1rem, 2vw, 1.4rem); color: var(--muted); margin-bottom: 24px; line-height: 1.6; }
    .hero .description { color: var(--muted); line-height: 1.8; margin-bottom: 32px; max-width: 70ch; }
    .cta-group { display: flex; gap: 16px; flex-wrap: wrap; margin-bottom: 32px; }
    .btn { padding: 14px 28px; border-radius: 12px; font-weight: 600; text-decoration: none; transition: all 0.25s ease; display: inline-flex; align-items: center; gap: 8px; }
    .btn-primary { background: linear-gradient(135deg, var(--accent), #8b5cf6); color: #fff; box-shadow: 0 8px 24px rgba(6, 182, 212, 0.3); }
    .btn-primary:hover { transform: translateY(-3px) scale(1.01); box-shadow: 0 12px 32px rgba(6, 182, 212, 0.45); }
    .btn-secondary { background: var(--glass); color: var(--text); border: 1px solid rgba(255,255,255,0.06); }
    .btn-secondary:hover { background: rgba(255,255,255,0.06); border-color: var(--accent); }
    .tech-stack { display: flex; flex-wrap: wrap; gap: 10px; }
    .tech-badge { padding: 8px 16px; background: var(--glass); border: 1px solid rgba(6, 182, 212, 0.2); border-radius: 20px; font-size: 13px; color: var(--accent); font-weight: 600; transition: transform 0.18s ease, box-shadow 0.18s ease; }
    .tech-badge:hover { transform: translateY(-4px); box-shadow: 0 8px 20px rgba(6,182,212,0.12); }

    .info-card { background: linear-gradient(135deg, var(--card), rgba(15, 22, 41, 0.8)); border: 1px solid rgba(255, 255, 255, 0.05); border-radius: var(--radius); padding: 30px; box-shadow: 0 20px 60px rgba(0, 0, 0, 0.5); backdrop-filter: blur(6px); animation: scaleIn 0.8s ease 0.4s backwards; transform-origin: center; will-change: transform, box-shadow; }
    .info-card:hover { box-shadow: 0 30px 80px rgba(0,0,0,0.6); transform: translateY(-6px); }

    .info-card h3 { font-size: 18px; margin-bottom: 20px; color: var(--accent); }
    .info-item { display: flex; align-items: flex-start; gap: 12px; margin-bottom: 16px; color: var(--muted); font-size: 14px; line-height: 1.6; }
    .info-item strong { color: var(--text); min-width: 70px; }
    .info-item a { color: var(--accent); text-decoration: none; }
    .divider { height: 1px; background: rgba(255, 255, 255, 0.05); margin: 24px 0; }
    .skills-grid { display: grid; grid-template-columns: repeat(3, 1fr); gap: 10px; margin-top: 16px; }
    .skill-tag { padding: 10px; background: rgba(6, 182, 212, 0.05); border: 1px solid rgba(6, 182, 212, 0.1); border-radius: 10px; font-size: 12px; text-align: center; color: var(--muted); transition: transform 0.18s ease, color 0.18s ease; }
    .skill-tag:hover { transform: translateY(-6px); color: var(--accent); border-color: var(--accent); }

    /* Cards */
    .card { background: linear-gradient(135deg, var(--card), rgba(15, 22, 41, 0.8)); border: 1px solid rgba(255, 255, 255, 0.05); border-radius: var(--radius); padding: 32px; margin-bottom: 24px; box-shadow: 0 20px 60px rgba(0, 0, 0, 0.5); transition: transform 0.3s ease, box-shadow 0.3s ease; animation: fadeInUp 1s ease backwards; }
    .card:hover { transform: translateY(-6px); box-shadow: 0 30px 80px rgba(0,0,0,0.65); }
    .project-card { background: rgba(255, 255, 255, 0.02); border: 1px solid rgba(255, 255, 255, 0.05); border-radius: 14px; padding: 24px; transition: all 0.3s ease; position: relative; overflow: hidden; }
    .project-card::before { content: ''; position: absolute; top: 0; left: 0; width: 100%; height: 3px; background: linear-gradient(90deg, var(--accent), #8b5cf6); transform: scaleX(0); transition: transform 0.3s ease; transform-origin: left; }
    .project-card:hover::before { transform: scaleX(1); }
    .project-link { color: var(--accent); text-decoration: none; font-weight: 600; }

    /* Timeline */
    .timeline { list-style: none; position: relative; padding-left: 30px; margin-top: 24px; }
    .timeline::before { content: ''; position: absolute; left: 0; top: 8px; bottom: 8px; width: 2px; background: linear-gradient(180deg, var(--accent), #8b5cf6); }

    /* Contact */
    .contact-form { display: flex; flex-direction: column; gap: 16px; margin-top: 24px; }
    .form-input { padding: 14px; background: rgba(255, 255, 255, 0.02); border: 1px solid rgba(255, 255, 255, 0.05); border-radius: 10px; color: var(--text); font-size: 14px; transition: all 0.3s ease; }
    .form-btn { padding: 14px; background: linear-gradient(135deg, var(--accent), #8b5cf6); border: none; border-radius: 10px; color: #fff; font-weight: 600; cursor: pointer; }

    footer { text-align: center; padding: 40px 0; color: var(--muted); font-size: 14px; margin-top: 60px; border-top: 1px solid rgba(255, 255, 255, 0.05); }

    /* Responsive */
    @media (max-width: 1024px) { .hero { grid-template-columns: 1fr; } .info-card { margin-top: 30px; } }
    @media (max-width: 768px) { body { padding: 0 16px; } header { flex-direction: column; gap: 20px; text-align: center; } nav { flex-direction: column; gap: 12px; } .hero h1 { font-size: 2.5rem; } .logo { margin: 0 auto; } }
    /* keyboard focus outlines for accessibility */
    .show-focus-outlines :focus { outline: 3px solid rgba(6,182,212,0.18); outline-offset: 3px; border-radius: 6px; }
  </style>
</head>
<body>
  <!-- Animated background particles (interactive) -->
  <div class="particles" aria-hidden="true"></div>

  <div class="wrap">
    <!-- Header -->
    <header>
      <div class="brand">
        <div class="logo" id="logo" aria-label="Bhargav Bhandari logo">BB</div>
        <div class="brand-text">
          <h2>Bhargav Bhandari</h2>
          <p>Data Engineer · ETL · Platform & Observability</p>
        </div>
      </div>
      
      <nav>
        <a href="#about">About</a>
        <a href="#projects">Projects</a>
        <a href="#experience">Experience</a>
        <a href="#contact">Contact</a>
        <a href="https://raw.githubusercontent.com/bhargav180620/bhargav180620.github.io/main/Bhargav_Bhandari_CV%20.pdf" class="resume-btn" id="resumeBtn">Resume</a>
      </nav>
    </header>

    <!-- Hero Section -->
    <section class="hero" id="hero">
      <div class="hero-content" id="heroContent">
        <h1>Hi, I'm Bhargav 👋</h1>
        <p class="tagline">Data Engineer building scalable data platforms & ML infrastructure</p>
        <p class="description">
          Practical experience with Python, Apache NiFi, Kafka (Strimzi), Debezium, Spark & Delta Lake, 
          Dagster, and Kubernetes. I build resilient pipelines with monitoring, retries and automation 
          so teams can ship data products reliably.
        </p>
        
        <div class="cta-group">
          <a href="#contact" class="btn btn-primary" id="contactBtn">
            <span>Get In Touch</span>
            <span>→</span>
          </a>
          <a href="#projects" class="btn btn-secondary">View Projects</a>
        </div>
        
        <div class="tech-stack" id="techStack">
          <span class="tech-badge">Python</span>
          <span class="tech-badge">Spark</span>
          <span class="tech-badge">Kafka</span>
          <span class="tech-badge">Kubernetes</span>
          <span class="tech-badge">Dagster</span>
        </div>
      </div>
      
      <aside class="info-card" id="infoCard">
        <h3>Quick Info</h3>
        <div class="info-item">
          <strong>Location:</strong>
          <span>Vapi, Gujarat, IN</span>
        </div>
        <div class="info-item">
          <strong>Email:</strong>
          <a href="mailto:bhargavbhandari90@gmail.com">bhargavbhandari90@gmail.com</a>
        </div>
        <div class="info-item">
          <strong>Phone:</strong>
          <span>+91 97371 74956</span>
        </div>
        
        <div class="divider"></div>
        
        <h3>Core Skills</h3>
        <div class="skills-grid">
          <div class="skill-tag">Python</div>
          <div class="skill-tag">SQL</div>
          <div class="skill-tag">Apache NiFi</div>
          <div class="skill-tag">Kafka</div>
          <div class="skill-tag">Debezium</div>
          <div class="skill-tag">Spark</div>
          <div class="skill-tag">Delta Lake</div>
          <div class="skill-tag">Dagster</div>
          <div class="skill-tag">Kubernetes</div>
        </div>
      </aside>
    </section>

    <!-- About Section -->
    <section class="card" id="about">
      <h3>About Me</h3>
      <p>
        Data Engineer with hands-on experience designing, deploying and optimizing end-to-end data infrastructure.
        I build observable, fault-tolerant pipelines and automation for data ingestion, CDC and ML workflows.
        Experienced working with on-prem clusters, streaming platforms, and storage automation. I thrive on solving 
        complex data challenges and making data infrastructure more reliable, scalable, and maintainable.
      </p>
    </section>

    <!-- Projects Section -->
    <section class="card" id="projects">
      <h3>Featured Projects</h3>
      <div class="projects-grid">
        <article class="project-card">
          <h4>Omics Ingestion Pipeline</h4>
          <p>
            Resumable, parallelized Python ingestion with Prometheus metrics and directory-wise progress tracking.
            Handles large-scale genomics data with automatic retry and recovery mechanisms.
          </p>
          <a href="https://github.com/bhargav180620/omics-ingest" class="project-link" target="_blank" rel="noreferrer">
            View Project →
          </a>
        </article>

        <article class="project-card">
          <h4>On-prem Kubernetes Infrastructure</h4>
          <p>
            Complete cluster provisioning, PV automation, and monitoring dashboards using Prometheus, Grafana, 
            and Loki for enterprise-grade observability.
          </p>
          <a href="https://github.com/bhargav180620/k8s-infra" class="project-link" target="_blank" rel="noreferrer">
            View Project →
          </a>
        </article>

        <article class="project-card">
          <h4>Debezium CDC Proof of Concept</h4>
          <p>
            Change Data Capture implementation with Debezium connectors for MySQL to Kafka streaming using 
            Strimzi operator, with comprehensive connector configurations.
          </p>
          <a href="https://github.com/bhargav180620/debezium-poc" class="project-link" target="_blank" rel="noreferrer">
            View Project →
          </a>
        </article>

        <article class="project-card">
          <h4>Prometheus-Monitored Downloader</h4>
          <p>
            Production-ready Python downloader with automatic retry/resume support, Prometheus metrics 
            integration, and directory progress aggregation for monitoring.
          </p>
          <a href="https://github.com/bhargav180620/ftp-downloader" class="project-link" target="_blank" rel="noreferrer">
            View Project →
          </a>
        </article>
      </div>
    </section>

    <!-- Experience Section -->
    <section class="card" id="experience">
      <h3>Experience</h3>
      <ul class="timeline">
        <li class="timeline-item">
          <div class="timeline-role">Data Engineer</div>
          <div class="timeline-company">Nuvo AI Pvt. Ltd. · June 2024 – Present</div>
          <p class="timeline-desc">
            Designed and deployed on-premises Kubernetes cluster with full observability stack. Built production 
            Dagster pipelines for ML workflows. Integrated Grafana, Prometheus, and Loki for comprehensive monitoring. 
            Implemented storage automation and orchestration. Led PoC initiatives for Debezium CDC, Supabase, and 
            JupyterHub. Developed resumable Python ingestion pipelines with retry mechanisms and progress tracking.
          </p>
        </li>
      </ul>
    </section>

    <!-- Education Section -->
    <section class="card">
      <h3>Education</h3>
      <div class="timeline-item" style="padding-left: 0;">
        <div class="timeline-role">B.E. Computer Science</div>
        <div class="timeline-company">Laxmi Institute of Technology · 2021–2024 · CGPA: 7.99</div>
      </div>
      <div class="timeline-item" style="padding-left: 0; margin-top: 20px;">
        <div class="timeline-role">Diploma in Computer Science & Engineering</div>
        <div class="timeline-company">Government Polytechnic, Daman · 2018–2021 · CGPA: 8.63</div>
      </div>
    </section>

    <!-- Contact Section -->
    <section class="card" id="contact">
      <h3>Let's Connect</h3>
      <p class="timeline-desc">If you'd like to collaborate, hire me, or chat about data engineering — drop a message below.</p>

      <form class="contact-form" action="#" onsubmit="return handleContactSubmit(event);">
        <input class="form-input" type="text" name="name" placeholder="Your name" required />
        <input class="form-input" type="email" name="email" placeholder="Your email" required />
        <input class="form-input" type="text" name="subject" placeholder="Subject" />
        <textarea class="form-input" name="message" placeholder="Message" required></textarea>
        <button class="form-btn" type="submit">Send Message</button>
      </form>
    </section>

    <footer>
      <p>Built by Bhargav — <a href="mailto:bhargavbhandari90@gmail.com">bhargavbhandari90@gmail.com</a></p>
    </footer>
  </div>

  <!-- Consolidated interactive JS (particles, parallax, draggable logo, hover effects, contact handler, defensive cleaning) -->
  <script>
    (function () {
      /* Shared variables used across features */
      const particlesEl = document.querySelector('.particles');
      const sizes = ['s','m','l'];

      // --- Particles generation ---
      function createParticles() {
        particlesEl.innerHTML = '';
        const PARTICLE_COUNT = Math.min(Math.max(Math.floor(window.innerWidth / 60), 12), 60);
        for (let i = 0; i < PARTICLE_COUNT; i++) {
          const p = document.createElement('div');
          p.className = 'particle';
          p.dataset.size = sizes[Math.floor(Math.random() * sizes.length)];
          p.style.left = Math.random() * 100 + '%';
          p.style.top = Math.random() * 100 + '%';
          p.style.opacity = (0.12 + Math.random() * 0.6).toFixed(2);
          p.style.transform = 'translate3d(0,0,0)';
          p.style.pointerEvents = 'none';
          particlesEl.appendChild(p);
        }
      }
      createParticles();

      // Recompute particles on resize (debounced)
      let resizeTimeout;
      window.addEventListener('resize', () => {
        clearTimeout(resizeTimeout);
        resizeTimeout = setTimeout(createParticles, 250);
      });

      // --- Parallax on mouse move for hero area ---
      const hero = document.getElementById('hero');
      const heroContent = document.getElementById('heroContent');
      const infoCard = document.getElementById('infoCard');
      const techStack = document.getElementById('techStack');

      function handleHeroMove(e) {
        const rect = hero.getBoundingClientRect();
        const x = (e.clientX - rect.left) / rect.width - 0.5; // -0.5..0.5
        const y = (e.clientY - rect.top) / rect.height - 0.5;
        // subtle 3D tilt for hero content
        heroContent.style.transform = `translateZ(0) rotateX(${(-y * 6).toFixed(2)}deg) rotateY(${(x * 6).toFixed(2)}deg)`;
        // info card moves slightly opposite
        infoCard.style.transform = `translate3d(${(-x * 12).toFixed(2)}px,${(-y * 8).toFixed(2)}px,0)`;

        // tech badges float
        Array.from(techStack.children).forEach((b, i) => {
          const dx = (x * (6 + i)) * (i % 2 ? 1 : -1);
          const dy = (y * (4 + i % 3));
          b.style.transform = `translate3d(${dx.toFixed(1)}px,${dy.toFixed(1)}px,0) rotate(${(dx / 8).toFixed(2)}deg)`;
        });

        // move particles with parallax effect based on mouse
        document.querySelectorAll('.particle').forEach((p, idx) => {
          const depth = p.dataset.size === 'l' ? 0.3 : (p.dataset.size === 'm' ? 0.5 : 0.8);
          const moveX = x * 40 * depth * (idx % 2 ? 1 : -1);
          const moveY = y * 30 * depth * (idx % 3 ? 1 : -1);
          p.style.transform = `translate3d(${moveX}px, ${moveY}px, 0)`;
        });
      }

      if (hero) {
        hero.addEventListener('pointermove', handleHeroMove);
        hero.addEventListener('pointerleave', () => {
          heroContent.style.transform = '';
          infoCard.style.transform = '';
          techStack.querySelectorAll('.tech-badge').forEach(b => b.style.transform = '');
          document.querySelectorAll('.particle').forEach(p => p.style.transform = '');
        });
      }

      // --- Draggable logo ---
      const logo = document.getElementById('logo');
      if (logo) {
        let dragging = false, startX = 0, startY = 0;
        logo.addEventListener('pointerdown', (e) => {
          dragging = true;
          startX = e.clientX;
          startY = e.clientY;
          logo.setPointerCapture && logo.setPointerCapture(e.pointerId);
          logo.style.transition = 'none';
        });
        window.addEventListener('pointermove', (e) => {
          if (!dragging) return;
          const dx = e.clientX - startX;
          const dy = e.clientY - startY;
          logo.style.position = 'relative';
          logo.style.left = dx + 'px';
          logo.style.top = dy + 'px';
          logo.style.transform = `translateZ(0) rotate(${dx / 12}deg) scale(1.02)`;
        });
        window.addEventListener('pointerup', (e) => {
          if (!dragging) return;
          dragging = false;
          logo.releasePointerCapture && logo.releasePointerCapture(e.pointerId);
          // animate back to original spot
          logo.style.transition = 'all 400ms cubic-bezier(.2,.9,.3,1)';
          logo.style.left = '0px';
          logo.style.top = '0px';
          logo.style.transform = '';
          setTimeout(() => { logo.style.transition = ''; }, 500);
        });
      }

      // --- Hover shine & subtle shadows on buttons ---
      document.querySelectorAll('.btn').forEach(btn => {
        btn.addEventListener('mousemove', (e) => {
          const r = btn.getBoundingClientRect();
          const px = e.clientX - r.left;
          const py = e.clientY - r.top;
          btn.style.boxShadow = `0 12px 30px rgba(6,182,212,0.12), ${ (px - r.width / 2) / 10 }px ${ (py - r.height / 2) / 10 }px 40px rgba(11,78,99,0.04)`;
        });
        btn.addEventListener('mouseleave', () => btn.style.boxShadow = '');
      });

      // --- Respect prefers-reduced-motion, but add other interactive effects otherwise ---
      if (!window.matchMedia || !window.matchMedia('(prefers-reduced-motion: reduce)').matches) {
        // Project card tilt
        document.querySelectorAll('.project-card').forEach(card => {
          card.style.transformOrigin = 'center';
          card.addEventListener('pointermove', (e) => {
            const r = card.getBoundingClientRect();
            const x = (e.clientX - r.left) / r.width - 0.5;
            const y = (e.clientY - r.top) / r.height - 0.5;
            const tiltX = (y * 10).toFixed(2);
            const tiltY = (x * -10).toFixed(2);
            const tx = (x * 6).toFixed(1);
            const ty = (y * -6).toFixed(1);
            card.style.transform = `perspective(600px) rotateX(${tiltX}deg) rotateY(${tiltY}deg) translate3d(${tx}px, ${ty}px, 0)`;
            card.style.transition = 'transform 0s';
          });
          card.addEventListener('pointerleave', () => {
            card.style.transition = 'transform 320ms cubic-bezier(.2,.9,.3,1)';
            card.style.transform = '';
          });
        });

        // Timeline item lift
        document.querySelectorAll('.timeline-item').forEach(item => {
          item.addEventListener('pointerenter', () => {
            item.style.transition = 'transform 220ms ease, box-shadow 220ms ease';
            item.style.transform = 'translateY(-6px)';
            item.style.boxShadow = '0 18px 50px rgba(2,6,23,0.6)';
          });
          item.addEventListener('pointerleave', () => {
            item.style.transform = '';
            item.style.boxShadow = '';
          });
        });

        // Info items slight parallax on move
        document.querySelectorAll('.info-item').forEach(info => {
          info.addEventListener('pointermove', (e) => {
            const r = info.getBoundingClientRect();
            const x = (e.clientX - r.left) / r.width - 0.5;
            const y = (e.clientY - r.top) / r.height - 0.5;
            info.style.transform = `translate3d(${(x * 6).toFixed(1)}px, ${(y * -4).toFixed(1)}px, 0)`;
            info.style.transition = 'transform 0s';
          });
          info.addEventListener('pointerleave', () => { info.style.transform = ''; info.style.transition = 'transform 220ms ease'; });
        });
      }

      // --- Keyboard accessibility: focus outlines for keyboard users only (fire once) ---
      function handleFirstTab(e) {
        if (e.key === 'Tab') {
          document.body.classList.add('show-focus-outlines');
          window.removeEventListener('keydown', handleFirstTab);
        }
      }
      window.addEventListener('keydown', handleFirstTab);

      // --- Defensive: remove stray doctype-like text nodes inserted in body ---
      function cleanDoctypeText() {
        const walker = document.createTreeWalker(document.body, NodeFilter.SHOW_TEXT, null);
        const nodes = [];
        let n;
        while (n = walker.nextNode()) nodes.push(n);
        nodes.forEach(node => {
          if (!node.nodeValue) return;
          const cleaned = node.nodeValue.replace(/<\s*(!?doctype|ldoctype)[^>]*>/ig, '');
          if (cleaned !== node.nodeValue) node.nodeValue = cleaned;
        });
      }
      // run it now and also on DOMContentLoaded to be defensive
      cleanDoctypeText();
      document.addEventListener('DOMContentLoaded', cleanDoctypeText);

      // --- Resume download handler (forces download via a hidden anchor) ---
      (function attachResumeHandler() {
        const resumeBtn = document.getElementById('resumeBtn') || document.querySelector('.resume-btn');
        const resumeHref = 'https://raw.githubusercontent.com/bhargav180620/bhargav180620.github.io/main/Bhargav_Bhandari_CV%20.pdf';
        if (resumeBtn) {
          resumeBtn.addEventListener('click', function (e) {
            // allow Ctrl/Meta+click and right-click open in new tab by checking modifier keys
            if (e.ctrlKey || e.metaKey || e.button === 1) {
              return; // fall back to default browser behavior
            }
            e.preventDefault();
            const a = document.createElement('a');
            a.href = resumeHref;
            a.download = 'Bhargav_Bhandari_CV.pdf';
            document.body.appendChild(a);
            a.click();
            a.remove();
          });
        }
      })();

      // --- Contact form handler: opens default mail client with prefilled details ---
      window.handleContactSubmit = function (e) {
        e.preventDefault();
        const form = e.target;
        const name = form.name ? form.name.value.trim() : '';
        const email = form.email ? form.email.value.trim() : '';
        const subject = form.subject ? form.subject.value.trim() : 'Contact from portfolio';
        const message = form.message ? form.message.value.trim() : '';

        const to = 'bhargavbhandari90@gmail.com';
        const bodyParts = [];
        if (name) bodyParts.push('Name: ' + name);
        if (email) bodyParts.push('Email: ' + email);
        if (message) {
          if (bodyParts.length) bodyParts.push(''); // blank line between metadata and message
          bodyParts.push(message);
        }
        // Use '\n' explicitly for newlines; ensure it's encoded properly
        const body = encodeURIComponent(bodyParts.join('\n'));
        const mailto = `mailto:${encodeURIComponent(to)}?subject=${encodeURIComponent(subject)}&body=${body}`;
        // Redirect to mail client
        window.location.href = mailto;
        return false;
      };

      // --- Entry animation for hero elements (small stagger) ---
      window.requestAnimationFrame(() => {
        document.querySelectorAll('.hero-content > *').forEach((el, i) => {
          el.style.opacity = 0;
          el.style.transform = 'translateY(10px)';
          setTimeout(() => {
            el.style.transition = 'all 420ms cubic-bezier(.2,.9,.3,1)';
            el.style.opacity = 1;
            el.style.transform = 'translateY(0)';
          }, 120 * i);
        });
      });

    })();
  </script>
</body>
</html>
