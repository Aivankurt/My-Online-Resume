<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>My Online Resume</title>

  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">

  <style>
    :root{
      --accent: #3cc4c9; 
      --muted: #666;
      --bg: #f6f6f6;
      --paper: #ffffff;
      --text: #111;
      --sidebar-width: 320px;
      --max-width: 1000px;
      --gutter: 28px;
    }


    *{box-sizing:border-box}
    html,body{height:100%}
    body{
      margin:0;
      font-family: "Poppins", system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
      background:var(--bg);
      color:var(--text);
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
      padding:24px;
      display:flex;
      justify-content:center;
      align-items:flex-start;
    }


    .resume-wrap{
      max-width: var(--max-width);
      width:100%;
      display:flex;
      gap:var(--gutter);
      background:linear-gradient(#bff0f2 0 130px, var(--paper) 130px);
      border:1px solid rgba(0,0,0,0.06);
      box-shadow:0 8px 30px rgba(0,0,0,0.06);
      overflow:hidden;
    }


    .sidebar{
      width:var(--sidebar-width);
      background:transparent;
      border-right:1px solid rgba(0,0,0,0.06);
      padding:24px;
      display:flex;
      flex-direction:column;
      gap:18px;
      align-items:stretch;
    }


    .photo-card{
      background:#fff;
      padding:8px;
      border:1px solid rgba(0,0,0,0.06);
      display:flex;
      justify-content:center;
      align-items:center;
    }


    .photo-card img{
      width:100%;
      height:auto;
      display:block;
      object-fit:cover;
    }


    .contact, .section{
      background:#fff;
      padding:14px;
      border-radius:6px;
      border:1px solid rgba(0,0,0,0.04);
    }


    .contact .item{ display:flex; gap:10px; align-items:flex-start; margin-bottom:10px; color:var(--muted); font-size:14px }
    .contact .item svg{ width:18px; height:18px; margin-top:2px; opacity:0.85 }

    h3.section-title{
      margin:0 0 10px 0;
      font-size:16px;
      letter-spacing:0.6px;
      color:#111;
    }


    .muted { color:var(--muted); font-size:14px; }

    .main{
      flex:1;
      padding:26px 30px;
      display:flex;
      flex-direction:column;
      gap:18px;
      min-width:0;
    }


    .header{
      display:flex;
      justify-content:space-between;
      align-items:flex-start;
      gap:12px;
    }
    .name-block{
      display:flex;
      flex-direction:column;
      gap:6px;
    }
    .name-block h1{
      margin:0;
      font-size:28px;
      letter-spacing:1px;
    }
    .jobtitle{
      margin:0;
      font-weight:600;
      color:var(--muted);
      font-size:14px;
    }

    .profile{
      background:#fff;
      padding:16px;
      border-radius:6px;
      border:1px solid rgba(0,0,0,0.04);
      color:var(--muted);
      line-height:1.5;
    }

    .work{
      background:#fff;
      padding:16px;
      border-radius:6px;
      border:1px solid rgba(0,0,0,0.04);
    }
    .job{
      margin-bottom:14px;
    }
    .job h4{ margin:0 0 6px 0; font-size:16px }
    .job .period { font-size:13px; color:var(--muted); margin-bottom:8px }
    .job p { margin:0; color:var(--muted); line-height:1.5; font-size:14px }

    .skills{
      display:flex;
      gap:12px;
      flex-wrap:wrap;
    }
    .skill-pill{
      padding:8px 10px;
      background:linear-gradient(0deg,#fbfbfb,#fff);
      border:1px solid rgba(0,0,0,0.04);
      border-radius:999px;
      font-size:13px;
      color:var(--muted);
    }

    .section-footer { color:var(--muted); font-size:13px; }

    .accent-band{
      position:absolute;
      left:0;
      top:0;
      height:110px;
      width:100%;
      background:var(--accent);
      z-index:0;
    }

    .resume-wrap .main .header, .resume-wrap .sidebar .photo-card{
      position:relative;
      z-index:2;
    }

   
    @media (max-width:880px){
      body{padding:12px;}
      .resume-wrap{flex-direction:column; max-width:760px}
      .sidebar{width:100%; border-right:none; border-bottom:1px solid rgba(0,0,0,0.06)}
    }

    @media print{
      body{padding:0; background:white}
      .resume-wrap{box-shadow:none; border:none; background:transparent}
      .accent-band{display:none}
    }
  </style>
</head>
<body>
  <div class="resume-wrap" role="article" aria-label="Resume">
    <div class="accent-band" aria-hidden="true"></div>

    <aside class="sidebar">
      <div class="photo-card" aria-hidden="false">

        <img src="https://im.ge/i/d67a7142-00fa-4ed9-855c-336c52c73935.ntN8Aq" alt=" My Profile Picture" />
      </div>

      <div class="contact">
        <h3 class="section-title">Contact</h3>
        <div class="item"><svg viewBox="0 0 24 24" fill="none"><path d="M21 16.5v3a1.5 1.5 0 0 1-1.5 1.5h-15A1.5 1.5 0 0 1 3 19.5v-15A1.5 1.5 0 0 1 4.5 3H11" stroke="#000" stroke-width="1.2" stroke-linecap="round" stroke-linejoin="round"/></svg><div>+63 912 345 6789</div></div>
        <div class="item"><svg viewBox="0 0 24 24" fill="none"><path d="M4 4h16v16H4z" stroke="#000" stroke-width="1.2" stroke-linecap="round" stroke-linejoin="round"/></svg><div>ordonez.aivankurt@gmail.com</div></div>
        <div class="item"><svg viewBox="0 0 24 24" fill="none"><path d="M12 2C8 2 5 4.5 5 8c0 5.5 7 12 7 12s7-6.5 7-12c0-3.5-3-6-7-6z" stroke="#000" stroke-width="1.2" stroke-linecap="round" stroke-linejoin="round"/></svg><div>Imus Cavite<br/>Philippines</div></div>
      </div>

      <div class="section">
        <h3 class="section-title">Education</h3>
        <div><strong>Bachelor of Information Technology</strong><br/>
        Cavite State University<br/>
        2027 — 2031</div>
      </div>

      <div class="section">
        <h3 class="section-title">Expertise</h3>
        <ul class="muted" style="padding-left:18px; margin:0;">
          <li>Software Development</li>
          <li>Systems Administration</li>
          <li>Cloud Computing</li>
          <li>Cybersecurity</li>
        </ul>
      </div>

      <div class="section">
        <h3 class="section-title">Language</h3>
        <div class="muted">English &amp; Tagalog</div>
      </div>
    </aside>

  
    <main class="main">
      <div class="header">
        <div class="name-block">
          <h1>ORDOÑEZ AIVAN KURT S.</h1>
          <div class="jobtitle">Multi-Modal Innovator</div>
        </div>
        <div style="text-align:right; min-width:160px;">
            
        </div>
      </div>

      <section class="profile">
        <h3 class="section-title">Profile</h3>
        <p class="muted">Fifteen years of experiential learning, development, and AI-human collaboration. Known for revolutionizing how humans interact with intelligent systems. Award-winning speaker, futurist, and creator of immersive multimedia experiences combining voice, visuals, and emotion. Committed to ethical, accessible, and creative AI development.</p>
      </section>

      <section class="work">
        <h3 class="section-title">Work Experience</h3>

        <div class="job">
          <h4>Chief Multimodal Experience Architect — NeuroViva Systems Inc.</h4>
          <div class="period">2019 — Present</div>
          <p>Led the launch of "NeuroWorlds," the first real-time AI-generated dream simulator. Designed printed emotional interfaces for users with neurodivergent conditions and coordinated cross-functional teams in product delivery.</p>
        </div>

        <div class="job">
          <h4>AI/Human Systems Consultant — UN Department of Human-Robot Harmony</h4>
         <div class="period">2016 — 2019</div>
          <p>Facilitated policy design between AI cities and human governments. Created empathy modules for humanoid assistants in post-crisis therapy zones. Delivered public talks on ethics and storytelling.</p>
        </div>

      </section>

      <section class="section" style="padding:16px;">
        <h3 class="section-title">Technical Skills</h3>
        <div class="skills" style="margin-top:8px">
          <div class="skill-pill">Dream-simulation architectures</div>
          <div class="skill-pill">Ethical algorithm engineering</div>
          <div class="skill-pill">Voice + audio design</div>
          <div class="skill-pill">Human-AI interaction</div>
          <div class="skill-pill">Cloud deployment</div>
          <div class="skill-pill">Cybersecurity</div>
        </div>
      </section>

      <section class="section" style="padding:16px;">
        <h3 class="section-title">References</h3>
        <div class="section-footer">Available upon request · Contact for full reference list</div>
      </section>

    </main>
  </div>
</body>
</html>
