<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Youssif Salama — Portfolio</title>
<style>
  @import url('https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@400;500;600;700&family=Inter:wght@400;500;600&family=JetBrains+Mono:wght@400;500&display=swap');

  :root{
    --bg: #0B1220;
    --bg-card: #121B2E;
    --bg-card-hover: #16233B;
    --line: #24314A;
    --amber: #F2A93B;
    --amber-dim: #B67A22;
    --text: #EDEFF3;
    --muted: #8B93A7;
    --muted-2: #5C6885;
  }

  *{ margin:0; padding:0; box-sizing:border-box; }

  html,body{
    background: var(--bg);
    color: var(--text);
    font-family: 'Inter', sans-serif;
    -webkit-font-smoothing: antialiased;
  }

  a{ color: inherit; text-decoration: none; }

  ::selection{ background: var(--amber); color: #0B1220; }

  :focus-visible{
    outline: 2px solid var(--amber);
    outline-offset: 3px;
  }

  .wrap{
    max-width: 1080px;
    margin: 0 auto;
    padding: 0 28px;
  }

  /* ---------- HERO ---------- */
  .hero{
    padding: 96px 0 64px;
    border-bottom: 1px solid var(--line);
    position: relative;
    overflow: hidden;
  }

  .hero::before{
    content: "";
    position: absolute;
    top: -120px;
    right: -120px;
    width: 420px;
    height: 420px;
    background: radial-gradient(circle, rgba(242,169,59,0.10) 0%, rgba(242,169,59,0) 70%);
    pointer-events: none;
  }

  .eyebrow{
    font-family: 'JetBrains Mono', monospace;
    font-size: 13px;
    letter-spacing: 0.08em;
    text-transform: uppercase;
    color: var(--amber);
    display: flex;
    align-items: center;
    gap: 10px;
    margin-bottom: 22px;
  }

  .eyebrow::before{
    content: "";
    width: 7px;
    height: 7px;
    border-radius: 50%;
    background: var(--amber);
    box-shadow: 0 0 0 4px rgba(242,169,59,0.15);
  }

  .hero h1{
    font-family: 'Space Grotesk', sans-serif;
    font-weight: 700;
    font-size: clamp(36px, 6vw, 58px);
    line-height: 1.05;
    letter-spacing: -0.02em;
    max-width: 780px;
  }

  .hero h1 span{ color: var(--muted-2); }

  .hero p.lede{
    margin-top: 22px;
    max-width: 640px;
    font-size: 17px;
    line-height: 1.65;
    color: var(--muted);
  }

  .hero-links{
    margin-top: 34px;
    display: flex;
    flex-wrap: wrap;
    gap: 12px;
  }

  .pill-link{
    font-family: 'JetBrains Mono', monospace;
    font-size: 13px;
    padding: 10px 16px;
    border: 1px solid var(--line);
    border-radius: 999px;
    color: var(--text);
    transition: border-color .18s ease, color .18s ease, transform .18s ease;
  }

  .pill-link:hover{
    border-color: var(--amber);
    color: var(--amber);
    transform: translateY(-1px);
  }

  .pill-link.primary{
    background: var(--amber);
    color: #0B1220;
    border-color: var(--amber);
    font-weight: 500;
  }
  .pill-link.primary:hover{
    color: #0B1220;
    filter: brightness(1.08);
  }

  /* ---------- SECTION LABEL ---------- */
  .section-label{
    font-family: 'JetBrains Mono', monospace;
    font-size: 13px;
    letter-spacing: 0.08em;
    text-transform: uppercase;
    color: var(--muted-2);
    padding: 56px 0 22px;
    display: flex;
    align-items: center;
    gap: 16px;
  }
  .section-label::after{
    content: "";
    flex: 1;
    height: 1px;
    background: var(--line);
  }

  /* ---------- GRID ---------- */
  .grid{
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 22px;
    padding-bottom: 40px;
  }

  @media (max-width: 720px){
    .grid{ grid-template-columns: 1fr; }
  }

  .card{
    display: flex;
    flex-direction: column;
    background: var(--bg-card);
    border: 1px solid var(--line);
    border-radius: 14px;
    overflow: hidden;
    transition: border-color .2s ease, transform .2s ease, background .2s ease;
  }

  a.card:hover, a.card:focus-visible{
    border-color: var(--amber-dim);
    background: var(--bg-card-hover);
    transform: translateY(-3px);
  }

  .card-visual{
    height: 148px;
    background:
      radial-gradient(circle at 85% 0%, rgba(242,169,59,0.08), transparent 55%),
      repeating-linear-gradient(135deg, rgba(255,255,255,0.02) 0 1px, transparent 1px 26px);
    border-bottom: 1px solid var(--line);
    display: flex;
    align-items: center;
    justify-content: center;
    position: relative;
  }

  .card-visual svg{ width: 100%; height: 100%; }

  .card-body{
    padding: 22px 22px 24px;
    display: flex;
    flex-direction: column;
    flex: 1;
  }

  .card-top{
    display: flex;
    align-items: flex-start;
    justify-content: space-between;
    gap: 10px;
    margin-bottom: 6px;
  }

  .card h3{
    font-family: 'Space Grotesk', sans-serif;
    font-size: 19px;
    font-weight: 600;
    letter-spacing: -0.01em;
  }

  .card .arrow{
    flex-shrink: 0;
    color: var(--muted-2);
    transition: color .2s ease, transform .2s ease;
  }
  a.card:hover .arrow{ color: var(--amber); transform: translate(2px,-2px); }

  .card .role{
    font-family: 'JetBrains Mono', monospace;
    font-size: 12.5px;
    color: var(--amber-dim);
    margin-bottom: 12px;
  }

  .card p.desc{
    font-size: 14.5px;
    line-height: 1.6;
    color: var(--muted);
    flex: 1;
  }

  .tags{
    margin-top: 16px;
    display: flex;
    flex-wrap: wrap;
    gap: 6px;
  }

  .tag{
    font-family: 'JetBrains Mono', monospace;
    font-size: 11px;
    padding: 4px 9px;
    border-radius: 5px;
    background: rgba(255,255,255,0.04);
    border: 1px solid var(--line);
    color: var(--muted);
  }

  .card-flag{
    font-family: 'JetBrains Mono', monospace;
    font-size: 11px;
    color: var(--muted-2);
    margin-top: 14px;
  }

  /* ---------- FOOTER ---------- */
  footer{
    border-top: 1px solid var(--line);
    padding: 40px 0 60px;
    margin-top: 20px;
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    justify-content: space-between;
    gap: 16px;
  }
  footer .muted{ color: var(--muted-2); font-size: 13px; font-family: 'JetBrains Mono', monospace; }

  @media (prefers-reduced-motion: reduce){
    *{ transition: none !important; }
  }
</style>
</head>
<body>

  <div class="wrap">
    <section class="hero">
      <div class="eyebrow">Available for remote work</div>
      <h1>Youssif Salama<br><span>Full-stack engineer — marketplaces, fintech &amp; AI integration.</span></h1>
      <p class="lede">
        I build the logic that sits between two-sided systems that don't trust each other by default —
        matching engines, wallets, and state machines where money and timing have to reconcile correctly.
        Node.js · NestJS · Next.js · PostgreSQL · MongoDB · OpenAI / ElevenLabs / Gemini integration.
      </p>
      <div class="hero-links">
        <a class="pill-link primary" href="mailto:youssifsalama01@gmail.com">Email me</a>
        <a class="pill-link" href="https://linkedin.com/in/youssif-salama" target="_blank" rel="noopener">LinkedIn</a>
        <a class="pill-link" href="#" target="_blank" rel="noopener">GitHub — add your link</a>
      </div>
    </section>

    <div class="section-label">Projects</div>

    <div class="grid">

      <!-- Wasel -->
      <a class="card" href="https://wasel-fleet.com/" target="_blank" rel="noopener">
        <div class="card-visual">
          <svg viewBox="0 0 400 148" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M20 110 L110 60 L200 95 L290 40 L380 75" stroke="#F2A93B" stroke-width="2" stroke-linecap="round" opacity="0.55"/>
            <circle cx="20" cy="110" r="5" fill="#F2A93B"/>
            <circle cx="110" cy="60" r="5" fill="#EDEFF3" opacity="0.8"/>
            <circle cx="200" cy="95" r="5" fill="#EDEFF3" opacity="0.8"/>
            <circle cx="290" cy="40" r="5" fill="#EDEFF3" opacity="0.8"/>
            <circle cx="380" cy="75" r="6" fill="#F2A93B"/>
            <circle cx="380" cy="75" r="11" stroke="#F2A93B" stroke-width="1" opacity="0.4"/>
          </svg>
        </div>
        <div class="card-body">
          <div class="card-top">
            <h3>Wasel</h3>
            <svg class="arrow" width="18" height="18" viewBox="0 0 24 24" fill="none"><path d="M7 17L17 7M17 7H9M17 7V15" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/></svg>
          </div>
          <div class="role">Backend Developer · Logistics Marketplace</div>
          <p class="desc">Connects customers with truck providers. Built the supply/demand matching engine, offer flow, and the trip-lifecycle state machine — including refunds, cancellations, and wallet reconciliation.</p>
          <div class="tags"><span class="tag">Node.js</span><span class="tag">State Machines</span><span class="tag">Matching Engine</span></div>
        </div>
      </a>

      <!-- Lite Pay -->
      <div class="card">
        <div class="card-visual">
          <svg viewBox="0 0 400 148" fill="none" xmlns="http://www.w3.org/2000/svg">
            <rect x="40" y="44" width="320" height="60" rx="10" stroke="#EDEFF3" stroke-width="2" opacity="0.55"/>
            <circle cx="310" cy="74" r="14" fill="#F2A93B" opacity="0.9"/>
            <path d="M40 62 H360" stroke="#EDEFF3" stroke-width="1.5" opacity="0.25"/>
            <path d="M60 118 L100 118 M130 118 L170 118 M200 118 L240 118" stroke="#F2A93B" stroke-width="2" stroke-linecap="round" opacity="0.5"/>
          </svg>
        </div>
        <div class="card-body">
          <div class="card-top"><h3>Lite Pay</h3></div>
          <div class="role">Backend Developer (team) · E-Wallet Platform</div>
          <p class="desc">Real-time transaction processing, wallet balance tracking, and payment-gateway integration with webhook idempotency to prevent duplicate transactions.</p>
          <div class="tags"><span class="tag">Node.js</span><span class="tag">WebSockets</span><span class="tag">JWT / RBAC</span></div>
          <div class="card-flag">Link coming soon</div>
        </div>
      </div>

      <!-- Tech Bridge -->
      <div class="card">
        <div class="card-visual">
          <svg viewBox="0 0 400 148" fill="none" xmlns="http://www.w3.org/2000/svg">
            <circle cx="90" cy="55" r="6" fill="#EDEFF3" opacity="0.8"/>
            <circle cx="200" cy="35" r="6" fill="#F2A93B"/>
            <circle cx="310" cy="60" r="6" fill="#EDEFF3" opacity="0.8"/>
            <circle cx="140" cy="105" r="6" fill="#EDEFF3" opacity="0.8"/>
            <circle cx="260" cy="110" r="6" fill="#EDEFF3" opacity="0.8"/>
            <path d="M90 55 L200 35 M200 35 L310 60 M200 35 L140 105 M200 35 L260 110 M140 105 L260 110" stroke="#F2A93B" stroke-width="1.4" opacity="0.4"/>
          </svg>
        </div>
        <div class="card-body">
          <div class="card-top"><h3>Tech Bridge</h3></div>
          <div class="role">Full Stack Developer &amp; Team Lead · Graduation Project — 98/100</div>
          <p class="desc">AI-powered social &amp; job-matching platform. Integrated NLP models for content optimisation and moderation, reaching 94% moderation accuracy.</p>
          <div class="tags"><span class="tag">MERN</span><span class="tag">NLP / AI</span><span class="tag">Team Lead</span></div>
          <div class="card-flag">Link coming soon</div>
        </div>
      </div>

      <!-- AMF -->
      <div class="card">
        <div class="card-visual">
          <svg viewBox="0 0 400 148" fill="none" xmlns="http://www.w3.org/2000/svg">
            <rect x="40" y="30" width="120" height="88" rx="6" stroke="#EDEFF3" stroke-width="1.5" opacity="0.4"/>
            <rect x="175" y="30" width="185" height="38" rx="6" stroke="#F2A93B" stroke-width="1.8" opacity="0.8"/>
            <rect x="175" y="80" width="185" height="38" rx="6" stroke="#EDEFF3" stroke-width="1.5" opacity="0.4"/>
          </svg>
        </div>
        <div class="card-body">
          <div class="card-top"><h3>AMF</h3></div>
          <div class="role">Full Stack Developer (team) · Corporate Website + Custom CMS</div>
          <p class="desc">Built a custom headless CMS so the client manages all pages and content independently, with Next.js SSR/SSG for fast delivery and strong SEO.</p>
          <div class="tags"><span class="tag">Next.js</span><span class="tag">Headless CMS</span><span class="tag">SSR/SSG</span></div>
          <div class="card-flag">Link coming soon</div>
        </div>
      </div>

      <!-- Trendlix -->
      <div class="card">
        <div class="card-visual">
          <svg viewBox="0 0 400 148" fill="none" xmlns="http://www.w3.org/2000/svg">
            <circle cx="140" cy="74" r="34" stroke="#EDEFF3" stroke-width="1.5" opacity="0.4"/>
            <circle cx="260" cy="74" r="34" stroke="#F2A93B" stroke-width="1.8" opacity="0.8"/>
            <text x="128" y="80" fill="#EDEFF3" font-family="JetBrains Mono, monospace" font-size="14" opacity="0.6">EN</text>
            <text x="244" y="80" fill="#F2A93B" font-family="JetBrains Mono, monospace" font-size="14">AR</text>
          </svg>
        </div>
        <div class="card-body">
          <div class="card-top"><h3>Trendlix Digital Platform</h3></div>
          <div class="role">Full Stack Developer (solo on features) · Agency Platform</div>
          <p class="desc">Bilingual EN/AR platform with full RTL support from a single codebase. Led a restructuring into clean architecture that cut new-hire onboarding time.</p>
          <div class="tags"><span class="tag">Next.js</span><span class="tag">i18n / RTL</span><span class="tag">Clean Architecture</span></div>
          <div class="card-flag">Link coming soon</div>
        </div>
      </div>

      <!-- Arabtec -->
      <div class="card">
        <div class="card-visual">
          <svg viewBox="0 0 400 148" fill="none" xmlns="http://www.w3.org/2000/svg">
            <rect x="30" y="30" width="150" height="88" rx="6" stroke="#EDEFF3" stroke-width="1.5" opacity="0.4"/>
            <rect x="200" y="30" width="70" height="40" rx="6" stroke="#F2A93B" stroke-width="1.6" opacity="0.75"/>
            <rect x="280" y="30" width="80" height="40" rx="6" stroke="#EDEFF3" stroke-width="1.5" opacity="0.4"/>
            <rect x="200" y="78" width="160" height="40" rx="6" stroke="#EDEFF3" stroke-width="1.5" opacity="0.4"/>
          </svg>
        </div>
        <div class="card-body">
          <div class="card-top"><h3>Arabtec</h3></div>
          <div class="role">Frontend Developer (team) · Corporate Marketing Site</div>
          <p class="desc">Pixel-accurate, fully responsive marketing website with animated sections and optimised asset loading across desktop and mobile.</p>
          <div class="tags"><span class="tag">Next.js</span><span class="tag">Animation</span><span class="tag">Responsive</span></div>
          <div class="card-flag">Link coming soon</div>
        </div>
      </div>

      <!-- Opindoo -->
      <div class="card">
        <div class="card-visual">
          <svg viewBox="0 0 400 148" fill="none" xmlns="http://www.w3.org/2000/svg">
            <rect x="55" y="90" width="26" height="30" fill="#EDEFF3" opacity="0.35"/>
            <rect x="95" y="70" width="26" height="50" fill="#EDEFF3" opacity="0.5"/>
            <rect x="135" y="50" width="26" height="70" fill="#F2A93B" opacity="0.9"/>
            <rect x="175" y="64" width="26" height="56" fill="#EDEFF3" opacity="0.5"/>
            <rect x="215" y="40" width="26" height="80" fill="#F2A93B" opacity="0.6"/>
            <line x1="45" y1="120" x2="330" y2="120" stroke="#EDEFF3" stroke-width="1" opacity="0.25"/>
          </svg>
        </div>
        <div class="card-body">
          <div class="card-top"><h3>Opindoo (Alumax)</h3></div>
          <div class="role">Full Stack Developer (team) · Product Website &amp; Dashboard</div>
          <p class="desc">Redesigned the corporate site and overhauled the admin dashboard, extending the codebase across frontend UI and backend APIs to improve reliability.</p>
          <div class="tags"><span class="tag">Next.js</span><span class="tag">Dashboard</span><span class="tag">Full Stack</span></div>
          <div class="card-flag">Link coming soon</div>
        </div>
      </div>

    </div>

    <footer>
      <div class="muted">/// built by Youssif Salama</div>
      <div class="muted">youssifsalama01@gmail.com</div>
    </footer>
  </div>

</body>
</html>
