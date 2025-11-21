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
    
    @keyframes gradientShift {
      0%, 100% { background-position: 0% 50%; }
      50% { background-position: 100% 50%; }
    }
    
    @keyframes float {
      0%, 100% { transform: translateY(0px); }
      50% { transform: translateY(-20px); }
    }
    
    @keyframes fadeInUp {
      from {
        opacity: 0;
        transform: translateY(30px);
      }
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }
    
    @keyframes scaleIn {
      from {
        opacity: 0;
        transform: scale(0.95);
      }
      to {
        opacity: 1;
        transform: scale(1);
      }
    }
    
    * { box-sizing: border-box; margin: 0; padding: 0; }
    
    html { scroll-behavior: smooth; }
    
    body {
      margin: 0;
      min-height: 100vh;
      background: 
        radial-gradient(circle at 20% 20%, rgba(6, 182, 212, 0.08) 0%, transparent 50%),
        radial-gradient(circle at 80% 80%, rgba(139, 92, 246, 0.06) 0%, transparent 50%),
        var(--bg);
      background-size: 100% 100%;
      animation: gradientShift 20s ease infinite;
      color: var(--text);
      -webkit-font-smoothing: antialiased;
      padding: 0;
      overflow-x: hidden;
    }
    
    /* Animated background particles */
    .particles {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      pointer-events: none;
      z-index: 0;
    }
    
    .particle {
      position: absolute;
      background: radial-gradient(circle, rgba(6, 182, 212, 0.3), transparent);
      border-radius: 50%;
      animation: float 6s ease-in-out infinite;
    }
    
    .particle:nth-child(1) { width: 3px; height: 3px; top: 20%; left: 20%; animation-delay: 0s; }
    .particle:nth-child(2) { width: 4px; height: 4px; top: 60%; left: 80%; animation-delay: 2s; }
    .particle:nth-child(3) { width: 2px; height: 2px; top: 40%; left: 60%; animation-delay: 4s; }
    .particle:nth-child(4) { width: 3px; height: 3px; top: 80%; left: 30%; animation-delay: 1s; }
    .particle:nth-child(5) { width: 4px; height: 4px; top: 10%; left: 70%; animation-delay: 3s; }
    
    .wrap {
      position: relative;
      z-index: 1;
      width: 100%;
      max-width: var(--maxw);
      margin: 0 auto;
      padding: 20px;
    }
    
    /* Header */
    header {
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 20px 0;
      margin-bottom: 40px;
      animation: fadeInUp 0.8s ease;
    }
    
    .brand {
      display: flex;
      gap: 16px;
      align-items: center;
    }
    
    .logo {
      width: 60px;
      height: 60px;
      border-radius: 16px;
      background: linear-gradient(135deg, var(--accent), #8b5cf6);
      display: flex;
      align-items: center;
      justify-content: center;
      color: #fff;
      font-weight: 800;
      font-size: 24px;
      box-shadow: 0 10px 30px rgba(6, 182, 212, 0.3);
      transition: transform 0.3s ease, box-shadow 0.3s ease;
    }
    
    .logo:hover {
      transform: translateY(-3px) rotate(5deg);
      box-shadow: 0 15px 40px rgba(6, 182, 212, 0.5);
    }
    
    .brand-text h2 {
      font-size: 20px;
      margin-bottom: 2px;
      background: linear-gradient(135deg, var(--accent), #8b5cf6);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
    }
    
    .brand-text p {
      color: var(--muted);
      font-size: 13px;
    }
    
    nav {
      display: flex;
      gap: 24px;
      align-items: center;
    }
    
    nav a {
      color: var(--muted);
      text-decoration: none;
      font-weight: 500;
      transition: color 0.3s ease;
      position: relative;
    }
    
    nav a:hover {
      color: var(--accent);
    }
    
    nav a::after {
      content: '';
      position: absolute;
      bottom: -4px;
      left: 0;
      width: 0;
      height: 2px;
      background: var(--accent);
      transition: width 0.3s ease;
    }
    
    nav a:hover::after {
      width: 100%;
    }
    
    .resume-btn {
      padding: 10px 20px;
      background: var(--glass);
      border: 1px solid rgba(6, 182, 212, 0.2);
      border-radius: 12px;
      color: var(--accent);
      font-weight: 600;
      transition: all 0.3s ease;
    }
    
    .resume-btn:hover {
      background: var(--accent);
      color: var(--bg);
      transform: translateY(-2px);
      box-shadow: 0 10px 25px rgba(6, 182, 212, 0.3);
    }
    
    /* Hero Section */
    .hero {
      display: grid;
      grid-template-columns: 1fr 380px;
      gap: 40px;
      margin-bottom: 60px;
      animation: fadeInUp 1s ease 0.2s backwards;
    }
    
    .hero-content {
      display: flex;
      flex-direction: column;
      justify-content: center;
    }
    
    .hero h1 {
      font-size: clamp(2.5rem, 5vw, 4rem);
      margin-bottom: 20px;
      line-height: 1.1;
      background: linear-gradient(135deg, #fff 0%, var(--accent) 100%);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
    }
    
    .hero .tagline {
      font-size: clamp(1.1rem, 2vw, 1.4rem);
      color: var(--muted);
      margin-bottom: 24px;
      line-height: 1.6;
    }
    
    .hero .description {
      color: var(--muted);
      line-height: 1.8;
      margin-bottom: 32px;
    }
    
    .cta-group {
      display: flex;
      gap: 16px;
      flex-wrap: wrap;
      margin-bottom: 32px;
    }
    
    .btn {
      padding: 14px 28px;
      border-radius: 12px;
      font-weight: 600;
      text-decoration: none;
      transition: all 0.3s ease;
      display: inline-flex;
      align-items: center;
      gap: 8px;
    }
    
    .btn-primary {
      background: linear-gradient(135deg, var(--accent), #8b5cf6);
      color: #fff;
      box-shadow: 0 8px 24px rgba(6, 182, 212, 0.3);
    }
    
    .btn-primary:hover {
      transform: translateY(-2px);
      box-shadow: 0 12px 32px rgba(6, 182, 212, 0.5);
    }
    
    .btn-secondary {
      background: var(--glass);
      color: var(--text);
      border: 1px solid rgba(255, 255, 255, 0.1);
    }
    
    .btn-secondary:hover {
      background: rgba(255, 255, 255, 0.08);
      border-color: var(--accent);
    }
    
    .tech-stack {
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
    }
    
    .tech-badge {
      padding: 8px 16px;
      background: var(--glass);
      border: 1px solid rgba(6, 182, 212, 0.2);
      border-radius: 20px;
      font-size: 13px;
      color: var(--accent);
      font-weight: 600;
      transition: all 0.3s ease;
    }
    
    .tech-badge:hover {
      background: rgba(6, 182, 212, 0.1);
      transform: translateY(-2px);
    }
    
    /* Info Card */
    .info-card {
      background: linear-gradient(135deg, var(--card), rgba(15, 22, 41, 0.8));
      border: 1px solid rgba(255, 255, 255, 0.05);
      border-radius: var(--radius);
      padding: 30px;
      box-shadow: 0 20px 60px rgba(0, 0, 0, 0.5);
      backdrop-filter: blur(10px);
      animation: scaleIn 0.8s ease 0.4s backwards;
    }
    
    .info-card h3 {
      font-size: 18px;
      margin-bottom: 20px;
      color: var(--accent);
    }
    
    .info-item {
      display: flex;
      align-items: flex-start;
      gap: 12px;
      margin-bottom: 16px;
      color: var(--muted);
      font-size: 14px;
      line-height: 1.6;
    }
    
    .info-item strong {
      color: var(--text);
      min-width: 70px;
    }
    
    .info-item a {
      color: var(--accent);
      text-decoration: none;
      transition: color 0.3s ease;
    }
    
    .info-item a:hover {
      color: var(--accent-hover);
      text-decoration: underline;
    }
    
    .divider {
      height: 1px;
      background: rgba(255, 255, 255, 0.05);
      margin: 24px 0;
    }
    
    .skills-grid {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 10px;
      margin-top: 16px;
    }
    
    .skill-tag {
      padding: 10px;
      background: rgba(6, 182, 212, 0.05);
      border: 1px solid rgba(6, 182, 212, 0.1);
      border-radius: 10px;
      font-size: 12px;
      text-align: center;
      color: var(--muted);
      transition: all 0.3s ease;
    }
    
    .skill-tag:hover {
      background: rgba(6, 182, 212, 0.1);
      border-color: var(--accent);
      color: var(--accent);
      transform: translateY(-2px);
    }
    
    /* Cards */
    .card {
      background: linear-gradient(135deg, var(--card), rgba(15, 22, 41, 0.8));
      border: 1px solid rgba(255, 255, 255, 0.05);
      border-radius: var(--radius);
      padding: 32px;
      margin-bottom: 24px;
      box-shadow: 0 20px 60px rgba(0, 0, 0, 0.5);
      transition: transform 0.3s ease, box-shadow 0.3s ease;
      animation: fadeInUp 1s ease backwards;
    }
    
    .card:hover {
      transform: translateY(-4px);
      box-shadow: 0 25px 70px rgba(0, 0, 0, 0.6);
    }
    
    .card h3 {
      font-size: 24px;
      margin-bottom: 16px;
      color: var(--text);
    }
    
    .card p {
      color: var(--muted);
      line-height: 1.8;
    }
    
    /* Projects Grid */
    .projects-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 20px;
      margin-top: 24px;
    }
    
    .project-card {
      background: rgba(255, 255, 255, 0.02);
      border: 1px solid rgba(255, 255, 255, 0.05);
      border-radius: 14px;
      padding: 24px;
      transition: all 0.3s ease;
      position: relative;
      overflow: hidden;
    }
    
    .project-card::before {
      content: '';
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 3px;
      background: linear-gradient(90deg, var(--accent), #8b5cf6);
      transform: scaleX(0);
      transition: transform 0.3s ease;
    }
    
    .project-card:hover {
      background: rgba(255, 255, 255, 0.04);
      border-color: var(--accent);
      transform: translateY(-4px);
    }
    
    .project-card:hover::before {
      transform: scaleX(1);
    }
    
    .project-card h4 {
      font-size: 18px;
      margin-bottom: 12px;
      color: var(--text);
    }
    
    .project-card p {
      font-size: 14px;
      color: var(--muted);
      line-height: 1.6;
      margin-bottom: 16px;
    }
    
    .project-link {
      color: var(--accent);
      text-decoration: none;
      font-weight: 600;
      font-size: 14px;
      display: inline-flex;
      align-items: center;
      gap: 6px;
      transition: gap 0.3s ease;
    }
    
    .project-link:hover {
      gap: 10px;
    }
    
    /* Timeline */
    .timeline {
      list-style: none;
      position: relative;
      padding-left: 30px;
      margin-top: 24px;
    }
    
    .timeline::before {
      content: '';
      position: absolute;
      left: 0;
      top: 8px;
      bottom: 8px;
      width: 2px;
      background: linear-gradient(180deg, var(--accent), #8b5cf6);
    }
    
    .timeline-item {
      position: relative;
      margin-bottom: 32px;
    }
    
    .timeline-item::before {
      content: '';
      position: absolute;
      left: -35px;
      top: 6px;
      width: 12px;
      height: 12px;
      background: var(--accent);
      border-radius: 50%;
      box-shadow: 0 0 0 4px rgba(6, 182, 212, 0.2);
    }
    
    .timeline-role {
      font-size: 18px;
      font-weight: 700;
      color: var(--text);
      margin-bottom: 4px;
    }
    
    .timeline-company {
      font-size: 14px;
      color: var(--accent);
      margin-bottom: 12px;
    }
    
    .timeline-desc {
      color: var(--muted);
      line-height: 1.7;
      font-size: 14px;
    }
    
    /* Contact Form */
    .contact-form {
      display: flex;
      flex-direction: column;
      gap: 16px;
      margin-top: 24px;
    }
    
    .form-input {
      padding: 14px;
      background: rgba(255, 255, 255, 0.02);
      border: 1px solid rgba(255, 255, 255, 0.05);
      border-radius: 10px;
      color: var(--text);
      font-size: 14px;
      transition: all 0.3s ease;
    }
    
    .form-input:focus {
      outline: none;
      border-color: var(--accent);
      background: rgba(255, 255, 255, 0.04);
    }
    
    .form-input::placeholder {
      color: var(--muted);
    }
    
    textarea.form-input {
      resize: vertical;
      min-height: 120px;
      font-family: inherit;
    }
    
    .form-btn {
      padding: 14px;
      background: linear-gradient(135deg, var(--accent), #8b5cf6);
      border: none;
      border-radius: 10px;
      color: #fff;
      font-weight: 600;
      cursor: pointer;
      transition: all 0.3s ease;
    }
    
    .form-btn:hover {
      transform: translateY(-2px);
      box-shadow: 0 10px 30px rgba(6, 182, 212, 0.4);
    }
    
    /* Footer */
    footer {
      text-align: center;
      padding: 40px 0;
      color: var(--muted);
      font-size: 14px;
      margin-top: 60px;
      border-top: 1px solid rgba(255, 255, 255, 0.05);
    }
    
    footer a {
      color: var(--accent);
      text-decoration: none;
      transition: color 0.3s ease;
    }
    
    footer a:hover {
      color: var(--accent-hover);
    }
    
    /* Responsive */
    @media (max-width: 1024px) {
      .hero {
        grid-template-columns: 1fr;
      }
      
      .info-card {
        margin-top: 30px;
      }
    }
    
    @media (max-width: 768px) {
      body {
        padding: 0 16px;
      }
      
      header {
        flex-direction: column;
        gap: 20px;
        text-align: center;
      }
      
      nav {
        flex-direction: column;
        gap: 12px;
      }
      
      .hero h1 {
        font-size: 2.5rem;
      }
      
      .cta-group {
        flex-direction: column;
      }
      
      .btn {
        justify-content: center;
      }
      
      .skills-grid {
        grid-template-columns: repeat(2, 1fr);
      }
      
      .projects-grid {
        grid-template-columns: 1fr;
      }
    }
    
    @media (max-width: 480px) {
      .logo {
        width: 50px;
        height: 50px;
        font-size: 20px;
      }
      
      .hero h1 {
        font-size: 2rem;
      }
      
      .card {
        padding: 20px;
      }
      
      .skills-grid {
        grid-template-columns: 1fr;
      }
    }
  </style>
</head>
<body>
  <!-- Animated background particles -->
  <div class="particles">
    <div class="particle"></div>
    <div class="particle"></div>
    <div class="particle"></div>
    <div class="particle"></div>
    <div class="particle"></div>
  </div>

  <div class="wrap">
    <!-- Header -->
    <header>
      <div class="brand">
        <div class="logo">BB</div>
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
        <a href="Bhargav_Bhandari_CV.pdf" class="resume-btn" target="_blank" rel="noreferrer">Resume</a>
      </nav>
    </header>

    <!-- Hero Section -->
    <section class="hero">
      <div class="hero-content">
        <h1>Hi, I'm Bhargav 👋</h1>
        <p class="tagline">Data Engineer building scalable data platforms & ML infrastructure</p>
        <p class="description">
          Practical experience with Python, Apache NiFi, Kafka (Strimzi), Debezium, Spark & Delta Lake, 
          Dagster, and Kubernetes. I build resilient pipelines with monitoring, retries and automation 
          so teams can ship data products reliably.
        </p>
        
        <div class="cta-group">
          <a href="#contact" class="btn btn-primary">
            <span>Get In Touch</span>
            <span>→</span>
          </a>
          <a href="#projects" class="btn btn-secondary">View Projects</a>
        </div>
        
        <div class="tech-stack">
          <span class="tech-badge">Python</span>
          <span class="tech-badge">Spark</span>
          <span class="tech-badge">Kafka</span>
          <span class="tech-badge">Kubernetes</span>
          <span class="tech-badge">Dagster</span>
        </div>
      </div>
      
      <aside class="info-card">
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
