
<style>
*{box-sizing:border-box;margin:0;padding:0}
.wrap{
  min-height:100vh;
  background:linear-gradient(160deg,#0d0d1a 0%,#16103a 40%,#0d1f2d 100%);
  padding:2rem 1.25rem 3rem;
  font-family:-apple-system,'SF Pro Display','Inter',sans-serif;
  color:#fff;
}
.glass{
  background:rgba(255,255,255,0.07);
  border:1px solid rgba(255,255,255,0.15);
  border-radius:22px;
  backdrop-filter:blur(20px);
  -webkit-backdrop-filter:blur(20px);
}
.glass-sm{
  background:rgba(255,255,255,0.05);
  border:1px solid rgba(255,255,255,0.1);
  border-radius:14px;
  backdrop-filter:blur(12px);
  -webkit-backdrop-filter:blur(12px);
}
.sec-label{
  font-size:.65rem;font-weight:500;letter-spacing:.14em;
  text-transform:uppercase;color:rgba(255,255,255,0.35);
  margin:0 0 .65rem .1rem;
}
.divider{height:1px;background:linear-gradient(90deg,transparent,rgba(255,255,255,0.1),transparent);margin:.8rem 0}
/* Hero */
.hero{text-align:center;padding:2.5rem 1.5rem 2rem;margin-bottom:1.25rem;position:relative;overflow:hidden}
.hero::before{content:'';position:absolute;top:-80px;left:50%;transform:translateX(-50%);
  width:320px;height:320px;
  background:radial-gradient(circle,rgba(120,90,255,0.28),transparent 65%);
  border-radius:50%;pointer-events:none}
.avatar{
  width:90px;height:90px;border-radius:50%;
  background:linear-gradient(135deg,#a78bfa,#60a5fa,#34d399);
  display:flex;align-items:center;justify-content:center;
  font-size:1.9rem;font-weight:600;
  margin:0 auto 1.1rem;
  border:2px solid rgba(255,255,255,0.25);
  color:#fff;letter-spacing:1px;
}
.hero h1{font-size:1.55rem;font-weight:600;margin-bottom:.35rem}
.hero .roles{font-size:.78rem;color:rgba(255,255,255,0.5);margin-bottom:.85rem;line-height:1.7}
.hero .tagline{font-size:.8rem;color:rgba(255,255,255,0.42);line-height:1.65;max-width:340px;margin:0 auto 1.4rem}
.pill-row{display:flex;justify-content:center;gap:8px;flex-wrap:wrap}
.contact-pill{
  display:flex;align-items:center;gap:6px;
  padding:5px 13px;
  background:rgba(255,255,255,0.09);
  border:1px solid rgba(255,255,255,0.18);
  border-radius:999px;
  font-size:.73rem;color:rgba(255,255,255,0.8);
  text-decoration:none;cursor:pointer;transition:background .2s;
}
.contact-pill:hover{background:rgba(255,255,255,0.16)}
.contact-pill i{font-size:13px}
/* Quote */
.quote-block{
  padding:1.1rem 1.3rem;
  margin-bottom:1.25rem;
  border-left:2px solid rgba(167,139,250,0.5);
  border-radius:0 14px 14px 0;
  background:rgba(167,139,250,0.07);
  border-top:1px solid rgba(167,139,250,0.12);
  border-right:1px solid rgba(167,139,250,0.12);
  border-bottom:1px solid rgba(167,139,250,0.12);
}
.quote-block p{font-size:.82rem;color:rgba(255,255,255,0.6);line-height:1.7;font-style:italic}
.quote-block .author{font-size:.7rem;color:rgba(255,255,255,0.3);margin-top:.5rem;font-style:normal}
/* 2-col grid */
.two-col{display:grid;grid-template-columns:1fr 1fr;gap:10px;margin-bottom:1.25rem}
.mini-card{padding:.9rem 1rem}
.mini-card .icon{
  width:32px;height:32px;border-radius:9px;
  display:flex;align-items:center;justify-content:center;
  font-size:16px;margin-bottom:.55rem;
}
.ic-purple{background:rgba(167,139,250,0.2);color:#a78bfa}
.ic-blue{background:rgba(96,165,250,0.2);color:#60a5fa}
.ic-green{background:rgba(52,211,153,0.2);color:#34d399}
.ic-amber{background:rgba(251,191,36,0.2);color:#fbbf24}
.ic-coral{background:rgba(251,146,60,0.2);color:#fb923c}
.ic-pink{background:rgba(244,114,182,0.2);color:#f472b6}
.mini-card .ct{font-size:.8rem;font-weight:500;margin-bottom:.2rem}
.mini-card .cs{font-size:.72rem;color:rgba(255,255,255,0.45);line-height:1.5}
/* Stack */
.stack-box{padding:1.1rem 1.2rem;margin-bottom:1.25rem}
.sg-label{font-size:.68rem;color:rgba(255,255,255,0.3);margin-bottom:.45rem}
.badge-row{display:flex;flex-wrap:wrap;gap:6px}
.badge{
  display:flex;align-items:center;gap:5px;
  padding:4px 10px;border-radius:8px;font-size:.72rem;font-weight:500;
  border:1px solid rgba(255,255,255,0.12);
  background:rgba(255,255,255,0.06);color:rgba(255,255,255,0.75);
}
.b-flutter{border-color:rgba(2,86,155,.5);background:rgba(2,86,155,.18);color:#7dd3fc}
.b-dart{border-color:rgba(1,117,194,.5);background:rgba(1,117,194,.18);color:#93c5fd}
.b-spring{border-color:rgba(109,179,63,.5);background:rgba(109,179,63,.15);color:#86efac}
.b-java{border-color:rgba(237,139,0,.4);background:rgba(237,139,0,.14);color:#fcd34d}
.b-laravel{border-color:rgba(255,45,32,.4);background:rgba(255,45,32,.12);color:#fca5a5}
.b-dotnet{border-color:rgba(81,43,212,.5);background:rgba(81,43,212,.2);color:#c4b5fd}
.b-react{border-color:rgba(97,218,251,.35);background:rgba(97,218,251,.09);color:#67e8f9}
.b-tailwind{border-color:rgba(6,182,212,.4);background:rgba(6,182,212,.12);color:#22d3ee}
.b-mysql{border-color:rgba(68,121,161,.5);background:rgba(68,121,161,.18);color:#93c5fd}
.b-mssql{border-color:rgba(204,41,39,.4);background:rgba(204,41,39,.13);color:#fca5a5}
/* Feature checks */
.check-grid{display:grid;grid-template-columns:1fr 1fr;gap:6px;margin-top:.6rem}
.check-item{display:flex;align-items:center;gap:6px;font-size:.74rem;color:rgba(255,255,255,0.6)}
.check-item i{font-size:13px;color:#34d399;flex-shrink:0}
/* Projects */
.proj-card{padding:1.2rem 1.25rem;margin-bottom:1rem}
.proj-header{display:flex;align-items:center;gap:10px;margin-bottom:.85rem}
.proj-icon{
  width:38px;height:38px;border-radius:11px;
  display:flex;align-items:center;justify-content:center;
  font-size:19px;flex-shrink:0;
}
.proj-name{font-size:.95rem;font-weight:600}
.proj-sub{font-size:.72rem;color:rgba(255,255,255,0.4);margin-top:.15rem}
.tech-tags{display:flex;flex-wrap:wrap;gap:5px;margin-top:.75rem;padding-top:.75rem;border-top:1px solid rgba(255,255,255,0.07)}
.tech-tag{
  padding:3px 9px;border-radius:6px;font-size:.68rem;
  background:rgba(255,255,255,0.07);border:1px solid rgba(255,255,255,0.1);
  color:rgba(255,255,255,0.55);
}
/* Learning */
.learn-wrap{padding:1rem 1.2rem;margin-bottom:1.25rem}
.learn-grid{display:grid;grid-template-columns:1fr 1fr;gap:6px;margin-top:.5rem}
.learn-item{
  display:flex;align-items:center;gap:7px;
  padding:6px 10px;
  background:rgba(167,139,250,0.08);
  border:1px solid rgba(167,139,250,0.18);
  border-radius:9px;
  font-size:.74rem;color:rgba(255,255,255,0.7);
}
.learn-item i{font-size:13px;color:#a78bfa}
/* Goals */
.goals-wrap{padding:1rem 1.2rem;margin-bottom:1.25rem}
.goal-item{display:flex;align-items:flex-start;gap:8px;padding:.45rem 0;font-size:.78rem;color:rgba(255,255,255,0.6);border-bottom:1px solid rgba(255,255,255,0.05)}
.goal-item:last-child{border-bottom:none}
.goal-item i{font-size:14px;color:#60a5fa;margin-top:1px;flex-shrink:0}
/* Stats */
.stats-wrap{padding:1.2rem;margin-bottom:1.25rem}
.stats-row{display:flex;gap:8px}
.stats-row img{flex:1;width:50%;border-radius:10px;border:1px solid rgba(255,255,255,0.08)}
.footer{text-align:center;font-size:.73rem;color:rgba(255,255,255,0.25);margin-top:1.5rem;letter-spacing:.05em}
</style>

<div class="wrap">

  <div class="glass hero">
    <div class="avatar">HR</div>
    <h1>Hi 👋 I'm Hoeun Raksa</h1>
    <p class="roles">Mobile App Developer &nbsp;·&nbsp; Flutter Developer &nbsp;·&nbsp; Backend Developer &nbsp;·&nbsp; Full-Stack Learner</p>
    <p class="tagline">Passionate about building scalable mobile applications, REST APIs, responsive interfaces, and solving real-world problems through code.</p>
    <div class="pill-row">
      <a class="contact-pill" href="mailto:hoeunraksa012@gmail.com"><i class="ti ti-mail" aria-hidden="true"></i>hoeunraksa012@gmail.com</a>
      <a class="contact-pill" href="https://github.com/HoeunRaksa" target="_blank"><i class="ti ti-brand-github" aria-hidden="true"></i>HoeunRaksa</a>
    </div>
  </div>

  <div class="glass-sm quote-block">
    <p>"Consistency beats motivation."</p>
    <p class="author">Keep learning · Keep building · Keep improving</p>
  </div>

  <p class="sec-label">About me</p>
  <div class="two-col">
    <div class="glass-sm mini-card">
      <div class="icon ic-purple"><i class="ti ti-device-mobile" aria-hidden="true"></i></div>
      <p class="ct">Mobile dev</p>
      <p class="cs">Flutter, Dart, Riverpod, GoRouter, animations</p>
    </div>
    <div class="glass-sm mini-card">
      <div class="icon ic-blue"><i class="ti ti-server" aria-hidden="true"></i></div>
      <p class="ct">Backend dev</p>
      <p class="cs">Spring Boot, JWT, REST APIs, Spring Security</p>
    </div>
    <div class="glass-sm mini-card">
      <div class="icon ic-green"><i class="ti ti-layout" aria-hidden="true"></i></div>
      <p class="ct">Frontend</p>
      <p class="cs">ReactJS, TailwindCSS, responsive UI design</p>
    </div>
    <div class="glass-sm mini-card">
      <div class="icon ic-amber"><i class="ti ti-database" aria-hidden="true"></i></div>
      <p class="ct">Database</p>
      <p class="cs">MySQL, SQL Server, design &amp; optimization</p>
    </div>
  </div>

  <p class="sec-label">Tech stack</p>
  <div class="glass-sm stack-box">
    <p class="sg-label">Mobile</p>
    <div class="badge-row">
      <span class="badge b-flutter"><i class="ti ti-brand-flutter" aria-hidden="true"></i>Flutter</span>
      <span class="badge b-dart"><i class="ti ti-diamond" aria-hidden="true"></i>Dart</span>
    </div>
    <div class="divider"></div>
    <p class="sg-label">Backend</p>
    <div class="badge-row">
      <span class="badge b-spring"><i class="ti ti-leaf" aria-hidden="true"></i>Spring Boot</span>
      <span class="badge b-java"><i class="ti ti-coffee" aria-hidden="true"></i>Java</span>
      <span class="badge b-laravel"><i class="ti ti-brand-laravel" aria-hidden="true"></i>Laravel</span>
      <span class="badge b-dotnet"><i class="ti ti-brand-windows" aria-hidden="true"></i>ASP.NET Core</span>
    </div>
    <div class="divider"></div>
    <p class="sg-label">Frontend</p>
    <div class="badge-row">
      <span class="badge b-react"><i class="ti ti-brand-react" aria-hidden="true"></i>React</span>
      <span class="badge b-tailwind"><i class="ti ti-wind" aria-hidden="true"></i>Tailwind CSS</span>
    </div>
    <div class="divider"></div>
    <p class="sg-label">Database</p>
    <div class="badge-row">
      <span class="badge b-mysql"><i class="ti ti-database" aria-hidden="true"></i>MySQL</span>
      <span class="badge b-mssql"><i class="ti ti-database" aria-hidden="true"></i>SQL Server</span>
    </div>
    <div class="divider"></div>
    <p class="sg-label">Tools</p>
    <div class="badge-row">
      <span class="badge"><i class="ti ti-brand-git" aria-hidden="true"></i>Git</span>
      <span class="badge"><i class="ti ti-brand-github" aria-hidden="true"></i>GitHub</span>
      <span class="badge"><i class="ti ti-api" aria-hidden="true"></i>Postman</span>
      <span class="badge"><i class="ti ti-brand-docker" aria-hidden="true"></i>Docker</span>
      <span class="badge"><i class="ti ti-code" aria-hidden="true"></i>VS Code</span>
      <span class="badge"><i class="ti ti-device-mobile" aria-hidden="true"></i>Android Studio</span>
      <span class="badge"><i class="ti ti-tools" aria-hidden="true"></i>IntelliJ</span>
      <span class="badge"><i class="ti ti-vector" aria-hidden="true"></i>Figma</span>
    </div>
  </div>

  <p class="sec-label">Technologies I've worked with</p>
  <div class="two-col" style="margin-bottom:1.25rem">
    <div class="glass-sm mini-card">
      <div class="icon ic-purple"><i class="ti ti-lock" aria-hidden="true"></i></div>
      <p class="ct">Authentication</p>
      <div class="check-grid" style="grid-template-columns:1fr">
        <div class="check-item"><i class="ti ti-check" aria-hidden="true"></i>JWT &amp; Refresh Token</div>
        <div class="check-item"><i class="ti ti-check" aria-hidden="true"></i>Email OTP verification</div>
        <div class="check-item"><i class="ti ti-check" aria-hidden="true"></i>Login &amp; authorization</div>
        <div class="check-item"><i class="ti ti-check" aria-hidden="true"></i>Spring Security</div>
      </div>
    </div>
    <div class="glass-sm mini-card">
      <div class="icon ic-blue"><i class="ti ti-api" aria-hidden="true"></i></div>
      <p class="ct">API</p>
      <div class="check-grid" style="grid-template-columns:1fr">
        <div class="check-item"><i class="ti ti-check" aria-hidden="true"></i>REST API design</div>
        <div class="check-item"><i class="ti ti-check" aria-hidden="true"></i>CRUD &amp; pagination</div>
        <div class="check-item"><i class="ti ti-check" aria-hidden="true"></i>JSON handling</div>
        <div class="check-item"><i class="ti ti-check" aria-hidden="true"></i>API integration</div>
      </div>
    </div>
    <div class="glass-sm mini-card">
      <div class="icon ic-green"><i class="ti ti-device-mobile" aria-hidden="true"></i></div>
      <p class="ct">Mobile features</p>
      <div class="check-grid" style="grid-template-columns:1fr">
        <div class="check-item"><i class="ti ti-check" aria-hidden="true"></i>Cart &amp; checkout</div>
        <div class="check-item"><i class="ti ti-check" aria-hidden="true"></i>QR payment</div>
        <div class="check-item"><i class="ti ti-check" aria-hidden="true"></i>Image upload</div>
        <div class="check-item"><i class="ti ti-check" aria-hidden="true"></i>Order tracking</div>
        <div class="check-item"><i class="ti ti-check" aria-hidden="true"></i>Search &amp; favorites</div>
      </div>
    </div>
    <div class="glass-sm mini-card">
      <div class="icon ic-coral"><i class="ti ti-server" aria-hidden="true"></i></div>
      <p class="ct">Backend features</p>
      <div class="check-grid" style="grid-template-columns:1fr">
        <div class="check-item"><i class="ti ti-check" aria-hidden="true"></i>User &amp; role mgmt</div>
        <div class="check-item"><i class="ti ti-check" aria-hidden="true"></i>Product &amp; category</div>
        <div class="check-item"><i class="ti ti-check" aria-hidden="true"></i>Order &amp; payment</div>
        <div class="check-item"><i class="ti ti-check" aria-hidden="true"></i>File upload API</div>
      </div>
    </div>
  </div>

  <p class="sec-label">Featured projects</p>

  <div class="glass proj-card">
    <div class="proj-header">
      <div class="proj-icon ic-blue" style="background:rgba(96,165,250,.15);border:1px solid rgba(96,165,250,.25)"><i class="ti ti-shopping-cart" aria-hidden="true"></i></div>
      <div>
        <p class="proj-name">ShopFlow</p>
        <p class="proj-sub">Full-stack shopping application</p>
      </div>
    </div>
    <div class="check-grid">
      <div class="check-item"><i class="ti ti-check" aria-hidden="true"></i>JWT &amp; email OTP auth</div>
      <div class="check-item"><i class="ti ti-check" aria-hidden="true"></i>Product listing</div>
      <div class="check-item"><i class="ti ti-check" aria-hidden="true"></i>Cart &amp; checkout</div>
      <div class="check-item"><i class="ti ti-check" aria-hidden="true"></i>Location management</div>
      <div class="check-item"><i class="ti ti-check" aria-hidden="true"></i>Order system</div>
      <div class="check-item"><i class="ti ti-check" aria-hidden="true"></i>Payment integration</div>
      <div class="check-item"><i class="ti ti-check" aria-hidden="true"></i>File upload</div>
      <div class="check-item"><i class="ti ti-check" aria-hidden="true"></i>Favorites &amp; profile</div>
    </div>
    <div class="tech-tags">
      <span class="tech-tag">Flutter</span><span class="tech-tag">Riverpod</span><span class="tech-tag">Spring Boot</span><span class="tech-tag">MySQL</span><span class="tech-tag">JWT</span>
    </div>
  </div>

  <div class="glass proj-card">
    <div class="proj-header">
      <div class="proj-icon" style="background:rgba(52,211,153,.15);border:1px solid rgba(52,211,153,.25);color:#34d399"><i class="ti ti-armchair" aria-hidden="true"></i></div>
      <div>
        <p class="proj-name">Furniture E-commerce</p>
        <p class="proj-sub">Mobile shopping app with QR payment</p>
      </div>
    </div>
    <div class="check-grid">
      <div class="check-item"><i class="ti ti-check" aria-hidden="true"></i>QR payment</div>
      <div class="check-item"><i class="ti ti-check" aria-hidden="true"></i>Order polling</div>
      <div class="check-item"><i class="ti ti-check" aria-hidden="true"></i>Provider state mgmt</div>
      <div class="check-item"><i class="ti ti-check" aria-hidden="true"></i>Cart &amp; checkout</div>
    </div>
    <div class="tech-tags">
      <span class="tech-tag">Flutter</span><span class="tech-tag">Provider</span><span class="tech-tag">Laravel</span><span class="tech-tag">MySQL</span>
    </div>
  </div>

  <div class="glass proj-card">
    <div class="proj-header">
      <div class="proj-icon" style="background:rgba(244,114,182,.15);border:1px solid rgba(244,114,182,.25);color:#f472b6"><i class="ti ti-plant" aria-hidden="true"></i></div>
      <div>
        <p class="proj-name">Flower Store API</p>
        <p class="proj-sub">Backend REST API project</p>
      </div>
    </div>
    <div class="check-grid">
      <div class="check-item"><i class="ti ti-check" aria-hidden="true"></i>Image upload</div>
      <div class="check-item"><i class="ti ti-check" aria-hidden="true"></i>Swagger docs</div>
    </div>
    <div class="tech-tags">
      <span class="tech-tag">ASP.NET Core</span><span class="tech-tag">C#</span><span class="tech-tag">MySQL</span>
    </div>
  </div>

  <div class="glass proj-card" style="margin-bottom:1.25rem">
    <div class="proj-header">
      <div class="proj-icon" style="background:rgba(251,191,36,.15);border:1px solid rgba(251,191,36,.25);color:#fbbf24"><i class="ti ti-school" aria-hidden="true"></i></div>
      <div>
        <p class="proj-name">Education Management Platform</p>
        <p class="proj-sub">Student &amp; teacher management system</p>
      </div>
    </div>
    <div class="check-grid">
      <div class="check-item"><i class="ti ti-check" aria-hidden="true"></i>Student management</div>
      <div class="check-item"><i class="ti ti-check" aria-hidden="true"></i>Teacher management</div>
      <div class="check-item"><i class="ti ti-check" aria-hidden="true"></i>Attendance system</div>
      <div class="check-item"><i class="ti ti-check" aria-hidden="true"></i>GPA system</div>
    </div>
    <div class="tech-tags">
      <span class="tech-tag">ReactJS</span><span class="tech-tag">TailwindCSS</span><span class="tech-tag">Laravel</span>
    </div>
  </div>

  <p class="sec-label">Currently learning</p>
  <div class="glass-sm learn-wrap">
    <div class="learn-grid">
      <div class="learn-item"><i class="ti ti-brand-docker" aria-hidden="true"></i>Docker</div>
      <div class="learn-item"><i class="ti ti-bolt" aria-hidden="true"></i>Redis</div>
      <div class="learn-item"><i class="ti ti-messages" aria-hidden="true"></i>Kafka</div>
      <div class="learn-item"><i class="ti ti-topology-star" aria-hidden="true"></i>Microservices</div>
      <div class="learn-item"><i class="ti ti-refresh" aria-hidden="true"></i>CI/CD</div>
      <div class="learn-item"><i class="ti ti-test-pipe" aria-hidden="true"></i>Testing</div>
      <div class="learn-item"><i class="ti ti-activity" aria-hidden="true"></i>Monitoring</div>
      <div class="learn-item"><i class="ti ti-cloud" aria-hidden="true"></i>Cloud deployment</div>
      <div class="learn-item"><i class="ti ti-box" aria-hidden="true"></i>Clean architecture</div>
      <div class="learn-item"><i class="ti ti-sitemap" aria-hidden="true"></i>System design</div>
    </div>
  </div>

  <p class="sec-label">Goals</p>
  <div class="glass-sm goals-wrap">
    <div class="goal-item"><i class="ti ti-target" aria-hidden="true"></i>Become strong in Flutter &amp; full-stack mobile dev</div>
    <div class="goal-item"><i class="ti ti-target" aria-hidden="true"></i>Improve backend architecture skills</div>
    <div class="goal-item"><i class="ti ti-target" aria-hidden="true"></i>Learn scalable systems &amp; DevOps</div>
    <div class="goal-item"><i class="ti ti-target" aria-hidden="true"></i>Build production-level applications</div>
    <div class="goal-item"><i class="ti ti-target" aria-hidden="true"></i>Contribute to open-source projects</div>
  </div>

  <p class="sec-label">GitHub stats</p>
  <div class="glass-sm stats-wrap">
    <div class="stats-row">
      <img src="https://github-readme-stats.vercel.app/api?username=HoeunRaksa&show_icons=true&theme=transparent&hide_border=true&title_color=a78bfa&text_color=94a3b8&icon_color=60a5fa" alt="GitHub stats" />
      <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=HoeunRaksa&layout=compact&theme=transparent&hide_border=true&title_color=a78bfa&text_color=94a3b8" alt="Top languages" />
    </div>
  </div>

  <div class="footer">⭐ &nbsp;Keep learning · Keep building · Keep improving &nbsp;⭐<br><span style="margin-top:.4rem;display:block">Thank you for visiting my profile</span></div>
</div>
