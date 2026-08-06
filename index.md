<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width,initial-scale=1">
<meta name="description" content="AutoIntel Intelligence turns hundreds of daily automotive stories into one scored, structured briefing: what matters, who's involved, and why.">
<meta property="og:title" content="AutoIntel Intelligence">
<meta property="og:description" content="Automotive industry intelligence, scored and structured. Not another rewrite — the signal, with sources.">
<meta property="og:type" content="website">
<meta property="og:url" content="https://autointel.news">
<meta name="twitter:card" content="summary_large_image">
<title>AutoIntel Intelligence — Automotive Industry Signal, Daily</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@500;600;700&family=IBM+Plex+Mono:wght@400;500;600&family=IBM+Plex+Sans:wght@400;500;600&display=swap" rel="stylesheet">
<style>
:root{
  --bg:#14171c;
  --panel:#1c2128;
  --panel-2:#20262e;
  --ink:#e7e9ec;
  --ink-dim:#a7adb6;
  --line:#2a3038;
  --amber:#f2a93b;
  --teal:#3ecf8e;
  --slate:#566072;
  --red:#e2604f;
}
*{box-sizing:border-box}
html,body{margin:0}
body{
  background:var(--bg);
  color:var(--ink);
  font-family:'IBM Plex Sans',Arial,sans-serif;
  font-size:15px;
  line-height:1.6;
}
h1,h2,h3,h4{
  font-family:'Space Grotesk',sans-serif;
  color:#fff;
  margin:0;
}
a{color:inherit;text-decoration:none}
.mono{font-family:'IBM Plex Mono',monospace}

/* ---------------- Ticker ---------------- */
.ticker{
  background:#0f1114;
  border-bottom:1px solid var(--line);
  overflow:hidden;
  white-space:nowrap;
  padding:9px 0;
}
.ticker-track{
  display:inline-flex;
  gap:36px;
  padding-left:36px;
  animation:tickerScroll 42s linear infinite;
}
.ticker-item{
  font-family:'IBM Plex Mono',monospace;
  font-size:12px;
  letter-spacing:0.03em;
  color:var(--ink-dim);
  display:inline-flex;
  align-items:center;
  gap:6px;
}
.ticker-item b{color:var(--ink);font-weight:500}
.ticker-icon{width:14px;height:14px;flex:none;display:inline-block;vertical-align:middle}
.ticker-up{color:var(--teal)}
.ticker-down{color:var(--red)}
.ticker-flat{color:var(--amber)}
@keyframes tickerScroll{
  from{transform:translateX(0)}
  to{transform:translateX(-50%)}
}
@media(prefers-reduced-motion:reduce){
  .ticker-track{animation:none}
  .ticker{overflow-x:auto}
}

/* ---------------- Masthead ---------------- */
.masthead{
  border-bottom:1px solid var(--line);
  background:var(--bg);
  position:sticky;
  top:0;
  z-index:50;
}
.masthead-row{
  max-width:1320px;
  margin:0 auto;
  padding:18px 24px 14px;
  display:flex;
  align-items:baseline;
  justify-content:space-between;
  gap:16px;
  flex-wrap:wrap;
}
.wordmark{
  font-size:22px;
  font-weight:700;
  letter-spacing:-0.01em;
}
.wordmark-sub{
  font-family:'IBM Plex Mono',monospace;
  font-size:10px;
  font-weight:500;
  letter-spacing:0.18em;
  color:var(--amber);
  margin-left:8px;
  vertical-align:middle;
}
.masthead-date{
  font-family:'IBM Plex Mono',monospace;
  font-size:11px;
  letter-spacing:0.08em;
  color:var(--ink-dim);
  text-transform:uppercase;
}
.section-nav{
  max-width:1320px;
  margin:0 auto;
  padding:0 24px 14px;
  display:flex;
  gap:18px;
  flex-wrap:wrap;
  font-size:12.5px;
}
.section-nav a{
  color:var(--ink-dim);
  border-bottom:2px solid transparent;
  padding-bottom:4px;
  transition:color .15s ease,border-color .15s ease;
}
.section-nav a:hover{color:var(--ink);border-color:var(--amber)}
.section-nav-toggle{
  display:none;
}

/* ---------------- Layout shell ---------------- */
.wrap{max-width:1320px;margin:0 auto;padding:32px 24px 64px}
.section-title{
  font-size:20px;
  margin-bottom:18px;
  display:flex;
  align-items:baseline;
  gap:10px;
}

/* ---------------- Hero / Featured story ---------------- */
.hero{margin-bottom:52px}
.hero-media{
  width:100%;
  aspect-ratio:800/450;
  border-radius:12px 12px 0 0;
  overflow:hidden;
  border:1px solid var(--line);
  border-bottom:none;
  background:var(--panel-2);
}
.hero-media img{width:100%;height:100%;object-fit:cover;display:block}
.hero-grid{border-top-left-radius:0;border-top-right-radius:0}
.eyebrow{
  font-family:'IBM Plex Mono',monospace;
  font-size:11px;
  letter-spacing:0.12em;
  color:var(--amber);
  display:block;
  margin-bottom:12px;
}
.hero-grid{
  display:grid;
  grid-template-columns:1.6fr 1fr;
  gap:36px;
  background:var(--panel);
  border:1px solid var(--line);
  border-radius:12px;
  padding:32px;
}
.hero-main h1{
  font-size:30px;
  line-height:1.25;
  margin-bottom:12px;
}
.dek{
  color:var(--ink-dim);
  font-size:14.5px;
  margin-bottom:20px;
  max-width:60ch;
}
.source-strip{
  display:flex;
  gap:16px;
  flex-wrap:wrap;
  align-items:center;
  font-size:12.5px;
  color:var(--ink-dim);
  padding-bottom:20px;
  margin-bottom:20px;
  border-bottom:1px solid var(--line);
}
.source-strip a{
  color:var(--amber);
  font-weight:500;
}
.source-strip a:hover{text-decoration:underline}
.chip-row{display:flex;flex-wrap:wrap;gap:8px}
.chip{
  font-family:'IBM Plex Mono',monospace;
  font-size:11px;
  padding:5px 10px;
  border-radius:999px;
  background:var(--panel-2);
  border:1px solid var(--line);
  color:var(--ink-dim);
  white-space:nowrap;
  display:inline-flex;
  align-items:center;
  gap:6px;
}
.chip-icon{width:16px;height:16px;flex:none;border-radius:3px}
.chip.entity-mfr{border-color:#3a4a3f;color:var(--teal)}
.chip.entity-gov{border-color:#4a3a2a;color:var(--amber)}
.chip.stock{
  display:inline-flex;
  align-items:center;
  gap:6px;
  color:var(--ink);
  border-color:var(--line);
}
.chip.stock .tk{font-weight:600;color:#fff}
.chip.stock .chg{font-weight:600}
.chip.stock.up .chg{color:var(--teal)}
.chip.stock.down .chg{color:var(--red)}

/* Entity data grid */
.entity-grid{
  display:grid;
  grid-template-columns:repeat(3,1fr);
  gap:20px 28px;
}
.entity-field{padding-top:2px}
.entity-field.wide{grid-column:1 / -1}
.ef-label{
  font-family:'IBM Plex Mono',monospace;
  font-size:10.5px;
  letter-spacing:0.1em;
  text-transform:uppercase;
  color:var(--ink-dim);
  display:block;
  margin-bottom:9px;
  font-weight:500;
}
.data-list{list-style:none;margin:0;padding:0;display:flex;flex-direction:column;gap:7px}
.data-list a{color:var(--ink-dim);font-size:13px;display:block}
.data-list a:hover{color:var(--teal)}
.timeline-list{list-style:none;margin:0;padding:0;display:flex;flex-direction:column;gap:10px}
.timeline-list li{
  display:flex;
  gap:12px;
  font-size:13px;
  color:var(--ink-dim);
  padding-left:14px;
  border-left:2px solid var(--line);
}
.timeline-list .t-date{
  font-family:'IBM Plex Mono',monospace;
  font-size:11px;
  color:var(--ink);
  white-space:nowrap;
  min-width:78px;
}

/* Gauge cluster */
.hero-gauges{
  display:grid;
  grid-template-columns:repeat(2, minmax(0,150px));
  gap:14px;
  align-content:start;
  justify-content:start;
}
.gauge{
  background:var(--panel-2);
  border:1px solid var(--line);
  border-radius:10px;
  padding:14px 12px 12px;
  text-align:center;
  max-width:150px;
}
.gauge svg{width:100%;max-width:100px;height:auto;display:block;margin:0 auto}
.gauge-value{
  font-family:'IBM Plex Mono',monospace;
  font-size:19px;
  font-weight:600;
  margin-top:-28px;
  display:block;
}
.gauge-label{
  font-family:'IBM Plex Mono',monospace;
  font-size:9.5px;
  letter-spacing:0.06em;
  color:var(--ink-dim);
  text-transform:uppercase;
  display:block;
  margin-top:2px;
}
.score-methodology{
  margin-top:18px;
  padding-top:18px;
  border-top:1px solid var(--line);
}
.score-methodology summary{
  cursor:pointer;
  font-family:'IBM Plex Mono',monospace;
  font-size:11.5px;
  color:var(--ink-dim);
  letter-spacing:0.03em;
  list-style:none;
}
.score-methodology summary::-webkit-details-marker{display:none}
.score-methodology summary:hover{color:var(--amber)}
.score-methodology dl{margin:14px 0 0;display:grid;grid-template-columns:1fr;gap:10px}
.score-methodology dt{
  font-family:'IBM Plex Mono',monospace;
  font-size:10.5px;
  letter-spacing:0.08em;
  text-transform:uppercase;
  color:var(--ink);
  margin-bottom:2px;
}
.score-methodology dd{margin:0;color:var(--ink-dim);font-size:12.5px;line-height:1.6}

/* ---------------- Dashboard / snapshot panels ---------------- */
.dashboard{margin-bottom:52px}
.dash-grid{
  display:grid;
  grid-template-columns:repeat(auto-fit,minmax(220px,1fr));
  gap:16px;
}
.stat-panel{
  background:var(--panel);
  border:1px solid var(--line);
  border-radius:10px;
  padding:18px;
}
.stat-panel h4{
  font-family:'IBM Plex Mono',monospace;
  font-size:10.5px;
  letter-spacing:0.1em;
  text-transform:uppercase;
  color:var(--ink-dim);
  margin-bottom:12px;
  font-weight:500;
  display:flex;
  align-items:center;
  gap:8px;
}
.panel-icon{width:32px;height:32px;flex:none}
.rank-list{list-style:none;margin:0;padding:0;display:flex;flex-direction:column;gap:9px}
.rank-list li{
  display:flex;
  justify-content:space-between;
  align-items:center;
  font-size:13px;
  gap:10px;
}
.rank-bar-wrap{flex:1;height:5px;background:var(--panel-2);border-radius:3px;overflow:hidden;margin:0 10px}
.rank-bar{height:100%;background:var(--teal);border-radius:3px}
.rank-count{font-family:'IBM Plex Mono',monospace;font-size:11px;color:var(--ink-dim);min-width:22px;text-align:right}
.tagcloud{display:flex;flex-wrap:wrap;gap:8px}
.tagcloud .chip{font-size:12px}
.tagcloud .chip.lg{font-size:14px;color:#fff;border-color:var(--amber)}

/* ---------------- Feature panels ---------------- */
.feature-panels{
  display:grid;
  grid-template-columns:repeat(auto-fit,minmax(280px,1fr));
  gap:16px;
  margin-bottom:52px;
}
.feature-panel{
  background:var(--panel);
  border:1px solid var(--line);
  border-radius:10px;
  padding:20px;
}
.feature-panel h3{font-size:15px;margin-bottom:14px;display:flex;align-items:center;gap:10px}
.fp-icon{width:40px;height:40px;flex:none;border-radius:8px}
.feature-panel .fp-row{
  display:block;
  padding:10px 0;
  border-top:1px solid var(--line);
}
.feature-panel .fp-row:first-of-type{border-top:none;padding-top:0}
.fp-row a{display:block;font-size:13.5px;margin-bottom:4px}
.fp-row a:hover{color:var(--amber)}
.fp-meta{font-family:'IBM Plex Mono',monospace;font-size:10.5px;color:var(--ink-dim);display:flex;gap:8px}

/* ---------------- Article table / rows ---------------- */
.sec-group{margin-bottom:48px}
.article-table{
  display:flex;
  flex-direction:column;
  border:1px solid var(--line);
  border-radius:10px;
  overflow:hidden;
}
.article-row{
  display:grid;
  grid-template-columns:52px 96px 1fr 200px;
  gap:16px;
  align-items:center;
  padding:14px 18px;
  background:var(--panel);
  border-bottom:1px solid var(--line);
  transition:background .15s ease;
}
.article-row:last-child{border-bottom:none}
.article-row:hover{background:var(--panel-2)}
.article-thumb{
  width:96px;
  aspect-ratio:120/68;
  border-radius:6px;
  overflow:hidden;
  background:var(--panel-2);
  border:1px solid var(--line);
}
.article-thumb img{width:100%;height:100%;object-fit:cover;display:block}
.score-chip{
  font-family:'IBM Plex Mono',monospace;
  font-size:13px;
  font-weight:600;
  width:40px;
  height:40px;
  border-radius:8px;
  display:flex;
  align-items:center;
  justify-content:center;
  background:var(--panel-2);
  border:1px solid var(--line);
  color:var(--amber);
}
.score-chip.high{color:var(--red);border-color:#4a2e2a}
.article-main a.headline{
  font-size:14.5px;
  font-weight:500;
  color:var(--ink);
  display:block;
  margin-bottom:5px;
}
.article-main a.headline:hover{color:var(--teal)}
.article-take{color:var(--ink-dim);font-size:13px;margin-bottom:7px}
.article-tags{display:flex;gap:6px;flex-wrap:wrap}
.article-tags .chip{font-size:10.5px;padding:3px 8px}
.article-source{
  text-align:right;
  font-family:'IBM Plex Mono',monospace;
  font-size:11px;
  color:var(--ink-dim);
  display:flex;
  flex-direction:column;
  gap:4px;
  align-items:flex-end;
}
.article-source a{color:var(--amber)}
.article-source a:hover{text-decoration:underline}


footer{
  border-top:1px solid var(--line);
  padding:36px 24px 48px;
}
.legal-note{
  max-width:1320px;
  margin:0 auto;
  color:var(--ink-dim);
  font-size:12.5px;
  line-height:1.7;
}

/* ---------------- Responsive ---------------- */
@media(max-width:900px){
  .wrap{padding:24px 16px 48px}
  .masthead-row{padding:14px 16px 12px}
  .section-nav-toggle{
    display:flex;
    align-items:center;
    gap:6px;
    margin:0 16px 12px;
    padding:8px 14px;
    background:var(--panel);
    border:1px solid var(--line);
    border-radius:8px;
    color:var(--ink-dim);
    font-family:'IBM Plex Mono',monospace;
    font-size:11.5px;
    letter-spacing:0.06em;
    text-transform:uppercase;
  }
  .section-nav-toggle .chev{transition:transform .2s ease}
  .section-nav-toggle[aria-expanded="true"] .chev{transform:rotate(180deg)}
  .section-nav{
    padding:0 16px 12px;
    flex-wrap:nowrap;
    overflow-x:auto;
    -webkit-overflow-scrolling:touch;
    scrollbar-width:none;
    max-height:0;
    opacity:0;
    padding-top:0;
    padding-bottom:0;
    margin-bottom:0;
    overflow:hidden;
    transition:max-height .25s ease,opacity .2s ease;
  }
  .section-nav.is-open{
    max-height:120px;
    opacity:1;
    padding-top:2px;
    padding-bottom:12px;
    overflow-x:auto;
  }
  .section-nav::-webkit-scrollbar{display:none}
  .section-nav a{white-space:nowrap;padding-bottom:8px}
  .hero-grid{grid-template-columns:1fr;padding:22px}
  .hero-main h1{font-size:24px}
  .hero-gauges{justify-content:center;gap:10px}
  .gauge{padding:10px 8px 10px;max-width:130px}
  .gauge svg{max-width:88px}
  .gauge-value{font-size:16px;margin-top:-24px}
  .gauge-label{font-size:8.5px}
  .entity-grid{grid-template-columns:repeat(2,1fr);gap:16px 20px}
  .dash-grid{grid-template-columns:repeat(auto-fit,minmax(160px,1fr))}
  .feature-panels{grid-template-columns:repeat(auto-fit,minmax(240px,1fr))}
  .section-title{font-size:18px}
  .article-row{grid-template-columns:52px 72px 1fr 200px}
  .article-thumb{width:72px}
}
@media(max-width:600px){
  .ticker-item{font-size:11px}
  .wordmark{font-size:19px}
  .masthead-date{display:none}
  .hero-main h1{font-size:21px}
  .dek{font-size:13.5px}
  .entity-grid{grid-template-columns:1fr}
  .source-strip{gap:10px 14px;font-size:12px}
  .dash-grid{grid-template-columns:repeat(2,minmax(0,1fr))}
  .stat-panel{padding:14px}
  .feature-panels{grid-template-columns:1fr}
  .article-row{grid-template-columns:40px 1fr;grid-template-areas:"score main" ". source";padding:12px 14px}
  .score-chip{grid-area:score;width:32px;height:32px;font-size:11px}
  .article-thumb{display:none}
  .article-main{grid-area:main}
  .article-source{grid-area:source;align-items:flex-start;text-align:left;margin-top:6px}
  .article-main a.headline{font-size:13.5px}
  .hero-gauges{grid-template-columns:repeat(2, minmax(0,110px));gap:8px}
  .gauge{max-width:110px;padding:8px 6px 8px}
  .gauge svg{max-width:76px}
  .gauge-value{font-size:14px;margin-top:-20px}
}
@media(max-width:380px){
  .gauge{max-width:96px;padding:7px 5px 7px}
  .gauge svg{max-width:66px}
  .gauge-value{font-size:12.5px;margin-top:-18px}
  .gauge-label{font-size:8px}
  .dash-grid{grid-template-columns:1fr}
}

.reveal{opacity:0;transform:translateY(16px);transition:opacity .5s ease,transform .5s ease}
.reveal.is-visible{opacity:1;transform:none}
@media(prefers-reduced-motion:reduce){.reveal{opacity:1;transform:none;transition:none}}
</style>
</head>
<body>

<div class="ticker" aria-label="Trending entities and topics">
  <div class="ticker-track" id="tickerTrack">
    <span class="ticker-item"><b>Tesla</b> NACS ecosystem expands <span class="ticker-up">▲</span></span>
    <span class="ticker-item"><b>EVgo</b> adds Tesla Superchargers <span class="ticker-up">▲</span></span>
    <span class="ticker-item"><b>Lucid</b> delays midsize SUV <span class="ticker-down">▼</span></span>
    <span class="ticker-item"><b>Volvo</b> drops lidar on EX90/ES90 <span class="ticker-flat">■</span></span>
    <span class="ticker-item"><b>UK EV Market</b> record July share <span class="ticker-up">▲</span></span>
    <span class="ticker-item"><b>GM–SAIC</b> JV extended to 2047 <span class="ticker-up">▲</span></span>
    <span class="ticker-item"><b>Solid‑state batteries</b> SK On–Factorial tie‑up <span class="ticker-up">▲</span></span>
    <span class="ticker-item"><b>Charging</b> retail co‑location surges <span class="ticker-up">▲</span></span>
    <span class="ticker-item"><b>BYD Denza</b> D9 launches in UK <span class="ticker-up">▲</span></span>
    <span class="ticker-item"><b>Hyundai</b> IONIQ 3 from ~$30k <span class="ticker-up">▲</span></span>
  </div>
</div>

<header class="masthead">
  <div class="masthead-row">
    <div class="wordmark">AutoIntel<span class="wordmark-sub">INTELLIGENCE</span></div>
    <div class="masthead-date" id="publishDate"></div>
  </div>
  <nav class="section-nav" id="sectionNav">
    <a href="#industry-news">Industry News</a>
    <a href="#electric-vehicles">Electric Vehicles</a>
    <a href="#manufacturers">Manufacturers</a>
    <a href="#dealers">Dealers</a>
    <a href="#suppliers">Suppliers</a>
    <a href="#government">Government</a>
    <a href="#technology">Technology</a>
    <a href="#finance">Finance</a>
    <a href="#international">International</a>
    <a href="#opinion">Opinion</a>
  </nav>
  <button class="section-nav-toggle" id="sectionNavToggle" aria-expanded="false" aria-controls="sectionNav">
    Sections <span class="chev">▾</span>
  </button>
</header>

<main class="wrap">

  <section class="hero reveal" id="featured">
    <span class="eyebrow">FEATURED STORY</span>
    <div class="hero-media">
      <img src="https://electrek.co/wp-content/uploads/sites/3/2026/08/evgo-tesla-partnership-1920x1080-1.jpg" alt="EVgo to deploy Tesla Superchargers across the US" width="800" height="450" loading="lazy">
    </div>
    <div class="hero-grid">
      <div class="hero-main">
        <h1>EVgo to deploy Tesla Superchargers across the US</h1>
        <p class="dek">EVgo will install Tesla V4 Supercharger hardware across its U.S. fast‑charging network with support for both NACS and CCS connectors.</p>

        <div class="source-strip">
          <span>Source: <b>electrive.com</b></span>
          <span>Aug 6, 2026</span>
          <a href="https://www.electrive.com/2026/08/06/evgo-to-deploy-tesla-superchargers-across-the-us/" target="_blank" rel="noopener">Read original →</a>
        </div>

        <div class="entity-grid">
          <div class="entity-field">
            <span class="ef-label">Manufacturers</span>
            <div class="chip-row">
              <span class="chip entity-mfr">Tesla</span>
            </div>
          </div>
          <div class="entity-field">
            <span class="ef-label">Suppliers</span>
            <div class="chip-row"><span class="chip">EVgo</span></div>
          </div>
          <div class="entity-field">
            <span class="ef-label">Countries</span>
            <div class="chip-row"><span class="chip">United States</span></div>
          </div>
          <div class="entity-field">
            <span class="ef-label">Government Agencies</span>
            <div class="chip-row">
              <span class="chip entity-gov">None cited</span>
            </div>
          </div>
          <div class="entity-field">
            <span class="ef-label">Public Companies</span>
            <div class="chip-row">
              <span class="chip stock up"><span class="tk">TSLA</span><span class="chg">▲</span></span>
              <span class="chip stock up"><span class="tk">EVGO</span><span class="chg">▲</span></span>
            </div>
          </div>
          <div class="entity-field">
            <span class="ef-label">Topics</span>
            <div class="chip-row">
              <span class="chip">Charging</span>
              <span class="chip">NACS</span>
              <span class="chip">Infrastructure</span>
              <span class="chip">Interoperability</span>
            </div>
          </div>
          <div class="entity-field wide">
            <span class="ef-label">Related Stories</span>
            <ul class="data-list">
              <li><a href="https://electrek.co/2026/08/05/evgo-branded-tesla-superchargers-are-coming/" target="_blank" rel="noopener">EVgo‑branded Tesla Superchargers are coming</a></li>
              <li><a href="https://www.greencarreports.com/news/1146051_gm-pilot-ev-charging-network-now-spans-over-25-states" target="_blank" rel="noopener">GM–Pilot EV fast‑charging network now in 25+ states</a></li>
              <li><a href="https://electrek.co/2026/08/04/evgo-is-putting-500-fast-chargers-where-americans-shop/" target="_blank" rel="noopener">EVgo to add 500+ fast chargers at shopping centers</a></li>
            </ul>
          </div>
          <div class="entity-field wide">
            <span class="ef-label">Timeline</span>
            <ul class="timeline-list">
              <li><span class="t-date mono">Aug 6, 2026</span><span>EVgo confirms nationwide deployment of Tesla V4 Supercharger hardware.</span></li>
              <li><span class="t-date mono">Aug 5, 2026</span><span>EVgo and Brixmor announce 500+ new DC fast-charging stalls at retail centers.</span></li>
              <li><span class="t-date mono">2025–2026</span><span>Automakers and networks accelerate NACS transition and multi‑standard support.</span></li>
            </ul>
          </div>
        </div>
      </div>

      <div class="hero-gauges">
        <div class="gauge">
          <svg viewBox="0 0 120 70"><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#2a3038" stroke-width="8"/><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#f2a93b" stroke-width="8" stroke-dasharray="157" stroke-dashoffset="15.7"/></svg>
          <span class="gauge-value mono">90</span>
          <span class="gauge-label">Importance</span>
        </div>
        <div class="gauge">
          <svg viewBox="0 0 120 70"><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#2a3038" stroke-width="8"/><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#3ecf8e" stroke-width="8" stroke-dasharray="157" stroke-dashoffset="31.4"/></svg>
          <span class="gauge-value mono">80</span>
          <span class="gauge-label">Editorial Quality</span>
        </div>
        <div class="gauge">
          <svg viewBox="0 0 120 70"><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#2a3038" stroke-width="8"/><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#e2604f" stroke-width="8" stroke-dasharray="157" stroke-dashoffset="23.55"/></svg>
          <span class="gauge-value mono">85</span>
          <span class="gauge-label">Industry Impact</span>
        </div>
        <div class="gauge">
          <svg viewBox="0 0 120 70"><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#2a3038" stroke-width="8"/><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#f2a93b" stroke-width="8" stroke-dasharray="157" stroke-dashoffset="34.54"/></svg>
          <span class="gauge-value mono">78</span>
          <span class="gauge-label">Reader Interest</span>
        </div>
      </div>
    </div>

    <details class="score-methodology">
      <summary>ⓘ How these scores are calculated</summary>
      <dl>
        <dt>Importance</dt><dd>Category priority (25%) + entity reach (40%) + financial/market magnitude (20%) + cross-source corroboration (15%).</dd>
        <dt>Editorial Quality</dt><dd>Fact specificity (40%) + publisher tier (30%) + attribution clarity (15%) + absence of press-release language (15%).</dd>
        <dt>Industry Impact</dt><dd>Business impact (40%) + dealer implications (30%) + market contradiction (20%) + regulatory/legal exposure (10%).</dd>
        <dt>Reader Interest</dt><dd>Named-brand prominence (35%) + topic heat (30%) + conflict/surprise angle (20%) + recency (15%). Proxy score — not yet based on real engagement data.</dd>
      </dl>
    </details>
  </section>

  <section class="dashboard reveal" id="snapshot">
    <h2 class="section-title">Industry Snapshot <span class="count">Week of Aug 5, 2026</span></h2>
    <div class="dash-grid">
      
      <div class="stat-panel">
        <h4><span class="panel-icon">📊</span>Top Manufacturers by Mentions</h4>
        <ul class="rank-list">
          <li><span>Tesla</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:95%"></span></span><span class="rank-count">95</span></li>
          <li><span>BYD</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:78%"></span></span><span class="rank-count">78</span></li>
          <li><span>Hyundai</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:70%"></span></span><span class="rank-count">70</span></li>
          <li><span>Volkswagen</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:66%"></span></span><span class="rank-count">66</span></li>
          <li><span>Mercedes‑Benz</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:60%"></span></span><span class="rank-count">60</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4><span class="panel-icon">🔌</span>Charging & Infrastructure</h4>
        <ul class="rank-list">
          <li><span>EVgo expansion</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:92%"></span></span><span class="rank-count">92</span></li>
          <li><span>NACS transition</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:84%"></span></span><span class="rank-count">84</span></li>
          <li><span>Retail co‑location</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:72%"></span></span><span class="rank-count">72</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4><span class="panel-icon">🏷️</span>Top Brands in Headlines</h4>
        <ul class="rank-list">
          <li><span>Cadillac</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:58%"></span></span><span class="rank-count">58</span></li>
          <li><span>Vauxhall</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:44%"></span></span><span class="rank-count">44</span></li>
          <li><span>Ferrari</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:40%"></span></span><span class="rank-count">40</span></li>
          <li><span>Volkswagen ID</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:38%"></span></span><span class="rank-count">38</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4><span class="panel-icon">🏦</span>Financial Moves</h4>
        <ul class="rank-list">
          <li><span>GM–SAIC JV renewal</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:88%"></span></span><span class="rank-count">88</span></li>
          <li><span>Base Power raises $1B</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:75%"></span></span><span class="rank-count">75</span></li>
          <li><span>Global Battery Materials M&amp;A</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:62%"></span></span><span class="rank-count">62</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4><span class="panel-icon">🧪</span>Emerging Tech Topics</h4>
        <div class="tagcloud">
          <span class="chip lg">Solid‑state</span>
          <span class="chip">Battery health</span>
          <span class="chip">Lidar strategy</span>
          <span class="chip">Robotaxis</span>
          <span class="chip">Software‑defined vehicles</span>
        </div>
      </div>

      <div class="stat-panel">
        <h4><span class="panel-icon">📈</span>EV Market Signals</h4>
        <ul class="rank-list">
          <li><span>UK EV share up</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:82%"></span></span><span class="rank-count">82</span></li>
          <li><span>Used EV repairs</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:64%"></span></span><span class="rank-count">64</span></li>
          <li><span>Retail pricing pressure</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:59%"></span></span><span class="rank-count">59</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4><span class="panel-icon">🏛️</span>Policy & Regulation</h4>
        <ul class="rank-list">
          <li><span>FCC inverter action</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:74%"></span></span><span class="rank-count">74</span></li>
          <li><span>UK grant updates</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:61%"></span></span><span class="rank-count">61</span></li>
          <li><span>NYC e‑bike rules</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:56%"></span></span><span class="rank-count">56</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4><span class="panel-icon">🌍</span>Regional Focus</h4>
        <div class="tagcloud">
          <span class="chip">United States</span>
          <span class="chip">United Kingdom</span>
          <span class="chip">China</span>
          <span class="chip">EU</span>
          <span class="chip">Nordics</span>
        </div>
      </div>

    </div>
  </section>

  <section class="feature-panels reveal">
    
    <div class="feature-panel">
      <h3><span class="fp-icon">🏭</span>Manufacturers</h3>
      <div class="fp-row">
        <a href="https://www.electrive.com/2026/08/06/saic-and-gm-extend-chinese-joint-venture-to-2047/" target="_blank" rel="noopener">GM and SAIC extend JV to 2047 and prep EV exports</a>
        <div class="fp-meta"><span>Score 83</span><span>Aug 6, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/new-mercedes-gla-ev-bigger-400-miles-range/" target="_blank" rel="noopener">New Mercedes GLA EV grows up with >400‑mile range</a>
        <div class="fp-meta"><span>Score 76</span><span>Jul 29, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.autocar.co.uk/car-news/new-cars/range-rover-skys-limit-price-bespoke-models" target="_blank" rel="noopener">Range Rover pushes bespoke commissions beyond £500k</a>
        <div class="fp-meta"><span>Score 68</span><span>Aug 6, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/hyundai-reveals-ioniq-3-prices-start-30000-interest-surges/" target="_blank" rel="noopener">Hyundai IONIQ 3 pricing lands around $30k</a>
        <div class="fp-meta"><span>Score 74</span><span>Jul 29, 2026</span></div>
      </div>
    </div>

    <div class="feature-panel">
      <h3><span class="fp-icon">🧠</span>Technology</h3>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">SK On and Factorial partner to scale solid‑state</a>
        <div class="fp-meta"><span>Score 79</span><span>Jul 29, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Volvo drops lidar on EX90/ES90 and compensates buyers</a>
        <div class="fp-meta"><span>Score 72</span><span>Jul 29, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.electrive.com/2026/08/05/study-air-exposure-accelerates-ageing-in-nickel-rich-batteries/" target="_blank" rel="noopener">Study flags air exposure ageing in nickel‑rich cathodes</a>
        <div class="fp-meta"><span>Score 66</span><span>Aug 5, 2026</span></div>
      </div>
    </div>

    <div class="feature-panel">
      <h3><span class="fp-icon">🏛️</span>Government</h3>
      <div class="fp-row">
        <a href="https://electrek.co/2026/08/05/fcc-bans-foreign-made-connected-solar-inverters/" target="_blank" rel="noopener">FCC curbs foreign‑made connected inverters</a>
        <div class="fp-meta"><span>Score 71</span><span>Aug 5, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.electrive.com/2026/08/05/uk-records-strongest-ev-july-to-date/" target="_blank" rel="noopener">UK posts strongest EV July across cars & vans</a>
        <div class="fp-meta"><span>Score 70</span><span>Aug 5, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.electrive.com/2026/08/05/india-approves-chargers-awaits-deployment/" target="_blank" rel="noopener">India approves 6,562 public chargers; deployment pending</a>
        <div class="fp-meta"><span>Score 63</span><span>Aug 5, 2026</span></div>
      </div>
    </div>

    <div class="feature-panel">
      <h3><span class="fp-icon">🏗️</span>Suppliers</h3>
      <div class="fp-row">
        <a href="https://www.autocar.co.uk/car-news/company-cars/used-ev-repair-scheme-looks-tackle-cliff-edge-residual-drops" target="_blank" rel="noopener">BCA launches battery repair hub for used EVs</a>
        <div class="fp-meta"><span>Score 67</span><span>Aug 6, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://chargedevs.com/newswire/tdk-releases-125-v-axial-aluminum-electrolytic-capac