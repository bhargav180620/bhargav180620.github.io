<!--
  Paste this file as README.md or index.md in your bhargav180620.github.io repo.
  Edit any text, links, or projects as you like.
-->

<style>
:root{
  --accent:#0ea5a4;
  --bg:#0f172a;
  --card:#0b1220;
  --muted:#94a3b8;
  --glass: rgba(255,255,255,0.03);
  font-family: Inter, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
}
body {
  background: linear-gradient(180deg, #020617 0%, #071029 60%);
  color: #e6eef8;
  line-height: 1.6;
  padding: 32px;
}
.main {
  max-width: 980px;
  margin: 0 auto;
}
.header {
  display:flex;
  gap:20px;
  align-items:center;
  margin-bottom: 20px;
}
.avatar {
  width:112px;
  height:112px;
  border-radius:12px;
  background: linear-gradient(135deg, var(--accent), #60a5fa);
  display:flex;
  align-items:center;
  justify-content:center;
  font-weight:700;
  font-size:34px;
  color:#021022;
  box-shadow: 0 6px 18px rgba(4,8,20,0.6);
}
.h1 { font-size:28px; margin:0; }
.h2 { color:var(--muted); margin:4px 0 0 0; font-size:14px; }
.card {
  background: linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));
  border-radius:12px;
  padding:18px;
  box-shadow: 0 6px 18px rgba(2,6,23,0.6);
  margin-bottom:18px;
}
.grid {
  display:grid;
  grid-template-columns: 1fr 320px;
  gap:18px;
}
@media (max-width:880px){ .grid { grid-template-columns: 1fr; } .header{flex-direction:row} }
.badge { display:inline-block; padding:6px 10px; border-radius:999px; background:var(--glass); color:var(--muted); font-size:13px; margin-right:8px; }
.skill { display:inline-block; margin:6px 8px 6px 0; padding:6px 10px; background:rgba(255,255,255,0.02); border-radius:8px; font-size:13px; color:#cfe9ff; }
.section-title { font-weight:700; color:#dbeafe; margin-bottom:8px; }
.contact-list { list-style:none; padding:0; margin:0; font-size:14px; color:var(--muted); }
.contact-list li { margin:8px 0; }
.cta {
  display:inline-block;
  margin-top:10px;
  background:var(--accent);
  color:#021022;
  padding:10px 14px;
  border-radius:10px;
  text-decoration:none;
  font-weight:700;
}
.small { font-size:13px; color:var(--muted); }
.timeline { list-style:none; padding:0; margin:0; }
.timeline li { margin-bottom:12px; }
.role { font-weight:700; color:#e6f7ff; }
.company { color:var(--muted); font-size:13px; }
.resume-link { color:var(--accent); font-weight:700; text-decoration:none; }
.footer { text-align:center; color:var(--muted); font-size:13px; margin-top:22px; }
.note { color:var(--muted); font-size:13px; margin-top:8px; }
</style>

<div class="main">

<div class="header">
  <div class="avatar">BB</div>
  <div>
    <h1 class="h1">Bhargav Bhandari</h1>
    <div class="h2">Data Engineer — building scalable data platforms, ETL & observability</div>
    <div style="margin-top:10px;">
      <span class="badge">Python</span>
      <span class="badge">Spark</span>
      <span class="badge">Kafka</span>
      <span class="badge">Kubernetes</span>
    </div>
  </div>
</div>

<div class="grid">

<!-- LEFT COLUMN -->
<div>

<div class="card">
  <div class="section-title">About</div>
  <div class="small">
    Data Engineer with experience designing, deploying, and optimizing scalable data infrastructure.
    Practical experience with Python, Apache NiFi, Kafka (Strimzi), Debezium, Spark, Dagster and Kubernetes.
    I focus on building observable, fault-tolerant pipelines and automations that help AI/ML teams and
    stakeholders ship insights faster. (Details from my resume). :contentReference[oaicite:1]{index=1}
  </div>
  <a class="cta" href="#contact">Contact Me</a>
  <div class="note">Tip: edit this intro to add what kind of roles you want (backend/data infra/ML infra).</div>
</div>

<div class="card">
  <div class="section-title">Experience</div>
  <ul class="timeline">
    <li>
      <div class="role">Data Engineer — Nuvo AI Pvt. Ltd.</div>
      <div class="company">June 2024 – Present</div>
      <div class="small">
        • Designed and deployed an on-prem Kubernetes cluster for critical apps and DBs. <br>
        • Built Dagster pipelines integrating Grafana, Prometheus, Loki and MinIO for observability. <br>
        • Implemented dynamic volume provisioning and automated storage workflows. <br>
        • Conducted PoCs for Debezium, Supabase, RavenDB and JupyterHub; owned deployments and troubleshooting. <br>
        • Built fault-tolerant Python pipelines with resume support and parallel ingestion for Omics datasets.
      </div>
    </li>
  </ul>
  <div class="note">(Experience summary taken from resume). :contentReference[oaicite:2]{index=2}</div>
</div>

<div class="card">
  <div class="section-title">Selected Skills</div>
  <div>
    <span class="skill">Python</span>
    <span class="skill">SQL</span>
    <span class="skill">Apache NiFi</span>
    <span class="skill">Kafka (Strimzi)</span>
    <span class="skill">Debezium</span>
    <span class="skill">Spark & Delta Lake</span>
    <span class="skill">Dagster</span>
    <span class="skill">Kubernetes</span>
    <span class="skill">Docker</span>
    <span class="skill">Prometheus</span>
    <span class="skill">Grafana</span>
    <span class="skill">Linux CLI</span>
  </div>
</div>

<div class="card">
  <div class="section-title">Projects (quick links)</div>
  <div class="small">
    • <strong>Data pipeline for Omics ingestion</strong> — resume mentions a parallelized, resumable ingestion pipeline. Add a repo link to show code. :contentReference[oaicite:3]{index=3}<br>
    • <strong>On-prem Kubernetes infra</strong> — cluster setup, storage automation, and monitoring dashboards. Add links to manifests or diagrams.<br>
    • <strong>Debezium PoC</strong> — CDC connector setup for MySQL/Postgres (proof-of-concept).
  </div>
  <div class="note">Replace the placeholders with links to your GitHub repos (example: /projects or direct repo URLs).</div>
</div>

<div class="card">
  <div class="section-title">Education</div>
  <div class="small">
    • Bachelor of Engineering, Computer Science — Laxmi Institute of Technology (2021–2024). CGPA: 7.99. :contentReference[oaicite:4]{index=4}<br>
    • Diploma in Computer Science Engineering — Government Polytechnic Daman (2018–2021). CGPA: 8.63. :contentReference[oaicite:5]{index=5}
  </div>
</div>

</div>

<!-- RIGHT COLUMN -->
<div>

<div class="card">
  <div class="section-title">Contact</div>
  <ul class="contact-list" id="contact">
    <li><strong>Email:</strong> <a class="resume-link" href="mailto:bhargavbhandari90@gmail.com">bhargavbhandari90@gmail.com</a></li>
    <li><strong>Phone:</strong> +91 97371 74956</li>
    <li><strong>LinkedIn:</strong> <a class="resume-link" href="https://www.linkedin.com/in/bhargav-bhandari-02a667268/">bhargav-bhandari-02a667268</a></li>
    <li><strong>Location:</strong> Vapi, Gujarat</li>
    <li><strong>Resume:</strong> <a class="resume-link" href="Bhargav_Bhandari_CV.pdf">Download PDF</a></li>
  </ul>
  <div class="note">Make sure `Bhargav_Bhandari_CV.pdf` is committed to the repo root (or update the link path accordingly).</div>
</div>

<div class="card">
  <div class="section-title">What I bring</div>
  <div class="small">
    • Hands-on data engineering with end-to-end pipeline ownership.<br>
    • Strong focus on observability (Prometheus, Grafana, Loki).<br>
    • Practical experience with infra automation (Kubernetes + storage).<br>
    • Collaboration with AI/ML teams to operationalize research workflows.
  </div>
</div>

<div class="card">
  <div class="section-title">Resume snapshot</div>
  <div class="small">
    This portfolio was generated from the resume content. For full details & references, download the resume above. :contentReference[oaicite:6]{index=6}
  </div>
</div>

<div class="card">
  <div class="section-title">Call to action</div>
  <div class="small">
    Looking for roles in Data Engineering, Platform Engineering, or Infrastructure for ML. If you'd like to collaborate or hire, reach out via email or LinkedIn.
  </div>
  <a class="cta" href="mailto:bhargavbhandari90@gmail.com">Let's talk</a>
</div>

</div> <!-- end RIGHT -->

</div> <!-- end grid -->

<div class="footer">
  Built by Bhargav — Data Engineer • View source on GitHub
</div>

</div>
