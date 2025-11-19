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

  <!-- Simple, modern CSS -->
  <style>
    :root{
      --bg:#071028;
      --card:#0c1320;
      --muted:#9fb0c8;
      --accent:#0ea5a4;
      --glass: rgba(255,255,255,0.03);
      --glass-2: rgba(255,255,255,0.02);
      --text:#e6eef8;
      --radius:12px;
      --maxw:1100px;
      font-family: Inter, ui-sans-serif, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
    }
    *{box-sizing:border-box}
    html,body{height:100%}
    body{
      margin:0;
      min-height:100%;
      background:
        radial-gradient(1200px 600px at 10% 10%, rgba(14,165,164,0.06), transparent 8%),
        radial-gradient(800px 400px at 90% 90%, rgba(96,165,250,0.04), transparent 6%),
        var(--bg);
      color:var(--text);
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
      padding:28px;
      display:flex;
      justify-content:center;
    }
    .wrap { width:100%; max-width:var(--maxw); }

    header{
      display:flex;
      align-items:center;
      justify-content:space-between;
      gap:20px;
      margin-bottom:20px;
    }
    .brand{
      display:flex;
      gap:16px;
      align-items:center;
    }
    .logo{
      width:68px; height:68px; border-radius:14px;
      background:linear-gradient(135deg,var(--accent),#60a5fa);
      display:flex;align-items:center;justify-content:center;
      color:#021022;font-weight:700;font-size:22px;box-shadow:0 8px 24px rgba(2,6,23,0.6);
    }
    nav a{
      color:var(--muted); text-decoration:none; margin-left:14px; font-size:15px;
    }
    nav a:hover{ color:var(--text) }

    .hero{
      background: linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));
      border-radius:var(--radius);
      padding:28px;
      display:flex;
      gap:24px;
      box-shadow: 0 8px 30px rgba(2,6,23,0.6);
      align-items:center;
      margin-bottom:18px;
    }
    .hero-left{flex:1}
    .hero-right{width:360px; min-width:260px}
    .title{font-size:28px; margin:0 0 6px 0}
    .subtitle{color:var(--muted); margin:0 0 14px 0}
    .cta{
      display:inline-block;
      background:var(--accent); color:#021022; font-weight:700;
      padding:10px 14px; border-radius:10px; text-decoration:none;
      margin-right:10px;
    }
    .ghost{
      display:inline-block; padding:10px 14px; border-radius:10px; background:var(--glass); color:var(--muted); text-decoration:none;
    }

    .grid{
      display:grid;
      grid-template-columns: 1fr 360px;
      gap:18px;
    }
    @media (max-width:980px){
      .grid{ grid-template-columns: 1fr; }
      .hero{ flex-direction:column; align-items:flex-start }
      .hero-right{ width:100% }
    }

    .card{
      background: linear-gradient(180deg,var(--card), rgba(7,10,20,0.6));
      border-radius:12px; padding:18px; color:var(--text);
      box-shadow: 0 8px 20px rgba(2,6,23,0.55);
    }

    h3{ margin:0 0 8px 0; font-size:16px; color:#e6f7ff }
    p.small{ color:var(--muted); margin:0 0 8px 0; line-height:1.6 }

    .badges{ margin:10px 0 0 0 }
    .badge{ display:inline-block; padding:6px 10px; border-radius:999px; background:var(--glass); color:var(--muted); margin-right:8px; font-size:13px }

    .skills{ display:flex; flex-wrap:wrap; gap:8px; margin-top:8px }
    .skill{ background:var(--glass-2); padding:8px 10px; border-radius:8px; font-size:13px; color:var(--muted) }

    .projects-grid{ display:grid; grid-template-columns: repeat(2,1fr); gap:12px; margin-top:12px }
    @media (max-width:640px){ .projects-grid{ grid-template-columns: 1fr } }
    .project{
      background: linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));
      padding:12px; border-radius:10px;
    }
    .project h4{ margin:0 0 6px 0; font-size:14px }
    .project p{ margin:0; color:var(--muted); font-size:13px }

    .timeline{ margin:12px 0 0 0; padding:0; list-style:none }
    .timeline li{ margin-bottom:12px }
    .role{ font-weight:700 }
    .company{ color:var(--muted); font-size:13px }

    footer{ text-align:center; color:var(--muted); font-size:13px; margin-top:18px }

    /* small utilities */
    .muted{ color:var(--muted); font-size:13px }
    .link{ color:var(--accent); text-decoration:none; font-weight:700 }
    .resume-button{ display:inline-block; padding:8px 12px; background:var(--glass); border-radius:8px; color:var(--muted); text-decoration:none; margin-left:8px }

    /* floating top-right resume */
    .top-actions{ display:flex; gap:10px; align-items:center }
  </style>
</head>
<body>
  <div class="wrap">

    <header>
      <div class="brand">
        <div class="logo">BB</div>
        <div>
          <div style="font-weight:700">Bhargav Bhandari</div>
          <div class="muted" style="font-size:13px">Data Engineer · ETL · Platform & Observability</div>
        </div>
      </div>

      <div class="top-actions">
        <a class="link" href="#projects">Projects</a>
        <a class="link" href="#contact">Contact</a>
        <a class="resume-button" href="Bhargav_Bhandari_CV.pdf" target="_blank" rel="noreferrer">Download Resume</a>
      </div>
    </header>

    <section class="hero" aria-labelledby="hero-title">
      <div class="hero-left">
        <h1 id="hero-title" class="title">Hi — I'm Bhargav</h1>
        <div class="subtitle">Data Engineer building scalable data platforms, ETL pipelines and observability for ML & analytics.</div>

        <p class="small">
          Practical experience with Python, Apache NiFi, Kafka (Strimzi), Debezium, Spark & Delta Lake, Dagster, and Kubernetes.
          I build resilient pipelines with monitoring, retries and automation so teams can ship data products reliably.
        </p>

        <div style="margin-top:12px;">
          <a class="cta" href="#contact">Hire / Contact</a>
          <a class="ghost" href="#projects">View Projects</a>
        </div>

        <div class="badges" style="margin-top:16px">
          <span class="badge">Python</span>
          <span class="badge">Spark</span>
          <span class="badge">Kafka</span>
          <span class="badge">Kubernetes</span>
        </div>
      </div>

      <aside class="hero-right card" aria-label="Quick info">
        <h3>Quick Info</h3>
        <p class="small"><strong>Location:</strong> Vapi, Gujarat</p>
        <p class="small"><strong>Email:</strong> <a class="link" href="mailto:bhargavbhandari90@gmail.com">bhargavbhandari90@gmail.com</a></p>
        <p class="small"><strong>Phone:</strong> +91 97371 74956</p>

        <hr style="border:none;border-top:1px solid rgba(255,255,255,0.03);margin:12px 0">

        <h3>Skills</h3>
        <div class="skills">
          <div class="skill">Python</div><div class="skill">SQL</div><div class="skill">Apache NiFi</div>
          <div class="skill">Kafka (Strimzi)</div><div class="skill">Debezium</div><div class="skill">Spark</div>
          <div class="skill">Delta Lake</div><div class="skill">Dagster</div><div class="skill">Kubernetes</div>
        </div>
      </aside>
    </section>

    <main class="grid" role="main">

      <!-- Left column -->
      <div>

        <section class="card" id="about">
          <h3>About</h3>
          <p class="small">
            Data Engineer with hands-on experience designing, deploying and optimizing end-to-end data infrastructure.
            I build observable, fault-tolerant pipelines and automation for data ingestion, CDC and ML workflows.
            Experienced working with on-prem clusters, streaming platforms, and storage automation. (Content adapted from resume.)
          </p>
        </section>

        <section class="card" id="projects" style="margin-top:12px">
          <h3>Selected Projects</h3>
          <div class="projects-grid">
            <article class="project">
              <h4>Omics Ingestion Pipeline</h4>
              <p>Resumable, parallelized Python ingestion with Prometheus metrics and directory-wise progress tracking. <br><a class="link" href="https://github.com/bhargav180620/omics-ingest" target="_blank" rel="noreferrer">Repo →</a></p>
            </article>

            <article class="project">
              <h4>On-prem Kubernetes Infra</h4>
              <p>Cluster provisioning, PV automation, monitoring dashboards (Prometheus/Grafana/Loki). <br><a class="link" href="https://github.com/bhargav180620/k8s-infra" target="_blank" rel="noreferrer">Repo →</a></p>
            </article>

            <article class="project">
              <h4>Debezium CDC PoC</h4>
              <p>Debezium connectors for MySQL → Kafka with Strimzi, connector configs and examples. <br><a class="link" href="https://github.com/bhargav180620/debezium-poc" target="_blank" rel="noreferrer">Repo →</a></p>
            </article>

            <article class="project">
              <h4>Prometheus-Monitored Downloader</h4>
              <p>Python downloader with retry/resume support, Prometheus metrics and directory progress aggregation. <br><a class="link" href="https://github.com/bhargav180620/ftp-downloader" target="_blank" rel="noreferrer">Repo →</a></p>
            </article>
          </div>

          <p class="muted" style="margin-top:10px">Tip: Replace repo links above with exact repo URLs or demos. Add screenshots by committing images to your repo and using <code>&lt;img&gt;</code> tags.</p>
        </section>

        <section class="card" style="margin-top:12px">
          <h3>Experience</h3>
          <ul class="timeline">
            <li>
              <div class="role">Data Engineer — Nuvo AI Pvt. Ltd.</div>
              <div class="company">June 2024 – Present</div>
              <div class="small">Designed and deployed on-prem Kubernetes cluster; built Dagster pipelines, integrated Grafana, Prometheus and Loki; implemented storage automation; PoC and ops for Debezium, Supabase and JupyterHub; developed resumable Python ingestion pipelines.</div>
            </li>
          </ul>
        </section>

        <section class="card" style="margin-top:12px">
          <h3>Education</h3>
          <p class="small"><strong>B.E. Computer Science</strong> — Laxmi Institute of Technology (2021–2024) — CGPA: 7.99</p>
          <p class="small"><strong>Diploma CSE</strong> — Government Polytechnic, Daman (2018–2021) — CGPA: 8.63</p>
        </section>

      </div>

      <!-- Right column -->
      <aside>

        <div class="card">
          <h3>Contact</h3>
          <p class="small"><strong>Email:</strong> <a class="link" href="mailto:bhargavbhandari90@gmail.com">bhargavbhandari90@gmail.com</a></p>
          <p class="small"><strong>Phone:</strong> +91 97371 74956</p>
          <p class="small"><strong>LinkedIn:</strong> <a class="link" href="https://www.linkedin.com/in/bhargav-bhandari-02a667268/" target="_blank" rel="noreferrer">bhargav-bhandari-02a667268</a></p>

          <hr style="border:none;border-top:1px solid rgba(255,255,255,0.03);margin:12px 0">

          <h3>Contact Form</h3>
          <!-- Simple JS mailto form -->
          <form id="contactForm" onsubmit="return sendMail(event)" style="display:flex;flex-direction:column;gap:8px">
            <input id="name" type="text" placeholder="Your name" required style="padding:8px;border-radius:8px;border:1px solid rgba(255,255,255,0.03);background:transparent;color:var(--text)">
            <input id="email" type="email" placeholder="Your email" required style="padding:8px;border-radius:8px;border:1px solid rgba(255,255,255,0.03);background:transparent;color:var(--text)">
            <textarea id="message" placeholder="Message" rows="4" required style="padding:8px;border-radius:8px;border:1px solid rgba(255,255,255,0.03);background:transparent;color:var(--text)"></textarea>
            <button type="submit" style="padding:10px;border-radius:10px;border:none;background:var(--accent);color:#021022;font-weight:700;cursor:pointer">Send Email</button>
          </form>
          <p class="muted" style="margin-top:8px">This opens your default email client with the message pre-filled.</p>
        </div>

        <div class="card" style="margin-top:12px">
          <h3>What I bring</h3>
          <p class="small">End-to-end pipeline ownership, focus on observability & automation, experience with on-prem infra and streaming/CDC architectures. I collaborate with AI/ML teams to productionize models and data.</p>
        </div>

      </aside>

    </main>

    <footer>
      <div class="muted">Built by Bhargav • <a class="link" href="https://github.com/bhargav180620" target="_blank" rel="noreferrer">GitHub</a></div>
    </footer>
  </div>

  <script>
    // contact form -> opens mailto with prefilled body
    function sendMail(e){
      e.preventDefault();
      const name = document.getElementById('name').value.trim();
      const email = document.getElementById('email').value.trim();
      const msg = document.getElementById('message').value.trim();
      const subject = encodeURIComponent('Contact from portfolio website — ' + name);
      const body = encodeURIComponent(`Name: ${name}\nEmail: ${email}\n\n${msg}`);
      // opens default mail client
      window.location.href = `mailto:bhargavbhandari90@gmail.com?subject=${subject}&body=${body}`;
      return false;
    }
  </script>
</body>
</html>
