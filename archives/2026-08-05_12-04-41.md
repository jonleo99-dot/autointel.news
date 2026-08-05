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
.section-title .count{
  font-family:'IBM Plex Mono',monospace;
  font-size:11px;
  color:var(--ink-dim);
  font-weight:400;
}

/* ---------------- Hero / Featured story ---------------- */
.hero{margin-bottom:52px}
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
}
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

/* Entity data grid (replaces narrative exec-summary / impact prose) */
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
}
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
.feature-panel h3{font-size:15px;margin-bottom:14px}
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
  grid-template-columns:52px 1fr 200px;
  gap:16px;
  align-items:center;
  padding:14px 18px;
  background:var(--panel);
  border-bottom:1px solid var(--line);
  transition:background .15s ease;
}
.article-row:last-child{border-bottom:none}
.article-row:hover{background:var(--panel-2)}
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
    <span class="ticker-item"><b>BMW</b> product review <span class="ticker-down">▼</span></span>
    <span class="ticker-item"><b>China</b> demand <span class="ticker-down">▼</span></span>
    <span class="ticker-item"><b>Hybrid demand</b> <span class="ticker-up">▲</span></span>
    <span class="ticker-item"><b>Rivian</b> margins <span class="ticker-up">▲</span></span>
    <span class="ticker-item"><b>NHTSA</b> suspension probe <span class="ticker-flat">■</span></span>
    <span class="ticker-item"><b>BYD</b> EV range <span class="ticker-up">▲</span></span>
    <span class="ticker-item"><b>Tesla</b> China unit <span class="ticker-flat">■</span></span>
    <span class="ticker-item"><b>Luminar</b> lidar exit <span class="ticker-down">▼</span></span>
    <span class="ticker-item"><b>DS</b> UK sales <span class="ticker-down">▼</span></span>
    <span class="ticker-item"><b>Genesis</b> flagship SUV <span class="ticker-up">▲</span></span>
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

  <!--
    FEATURED STORY CONTRACT
    Selection: highest ImportanceScore across today's analyzed articles.
    This section is DATA-FIRST: no executive-summary or industry-impact
    prose. The one-sentence {{FEATURED_DEK}} is a plain factual statement
    only — everything else is structured entity/topic/timeline data
    extracted from the article, not written analysis.
  -->
  <section class="hero reveal" id="featured">
    <span class="eyebrow">FEATURED STORY</span>
    <div class="hero-grid">
      <div class="hero-main">
        <h1>US opens probe into 1.2 million Tesla Model 3 and Model Y over front-suspension failures</h1>
        <p class="dek">The National Highway Traffic Safety Administration launched a preliminary investigation into 2018–2020 Model 3 and 2021–2023 Model Y vehicles for potential separation of the front lower lateral link.</p>

        <div class="source-strip">
          <span>Source: <b>electrive</b></span>
          <span>Aug 3, 2026</span>
          <a href="https://www.electrive.com/2026/08/03/nhtsa-opens-probe-into-1-2-million-teslas/" target="_blank" rel="noopener">Read original →</a>
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
            <div class="chip-row"></div>
          </div>
          <div class="entity-field">
            <span class="ef-label">Countries</span>
            <div class="chip-row"><span class="chip">United States</span></div>
          </div>
          <div class="entity-field">
            <span class="ef-label">Government Agencies</span>
            <div class="chip-row">
              <span class="chip entity-gov">NHTSA</span>
            </div>
          </div>
          <div class="entity-field">
            <span class="ef-label">Public Companies</span>
            <div class="chip-row">
              <span class="chip stock down"><span class="tk">TSLA</span><span class="chg">-1.8%</span></span>
            </div>
          </div>
          <div class="entity-field">
            <span class="ef-label">Topics</span>
            <div class="chip-row">
              <span class="chip">Safety</span>
              <span class="chip">Recall/Investigation</span>
              <span class="chip">Government</span>
            </div>
          </div>
          <div class="entity-field wide">
            <span class="ef-label">Related Stories</span>
            <ul class="data-list">
              <li><a href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">NHTSA probes 1.2M Tesla Model 3/Model Y over suspension failures (Electrek)</a></li>
              <li><a href="https://www.autocar.co.uk/car-news/business-corporate/cheap-cars-hit-tesla-profits-tech-pivot-stalls" target="_blank" rel="noopener">Cheap cars hit Tesla profits as tech pivot stalls (Autocar)</a></li>
              <li><a href="https://electrek.co/2026/07/28/tesla-sues-cybertruck-supplier-angstrom-tooling/" target="_blank" rel="noopener">Tesla sues Cybertruck supplier amid standoff (Electrek)</a></li>
              <li><a href="https://electrek.co/2026/08/04/tesla-china-sales-crash-exports-surge-h1-2026/" target="_blank" rel="noopener">Tesla China sales are crashing as exports surge (Electrek)</a></li>
            </ul>
          </div>
          <div class="entity-field wide">
            <span class="ef-label">Timeline</span>
            <ul class="timeline-list">
              <li><span class="t-date mono">Aug 03, 2026</span><span>NHTSA confirms preliminary evaluation into 1.2M Tesla Model 3/Y for lower lateral link separations.</span></li>
              <li><span class="t-date mono">Jul 31, 2026</span><span>Multiple outlets report new complaints triggering the federal probe.</span></li>
              <li><span class="t-date mono">2018–2023</span><span>Model years under scrutiny span 2018–2020 (Model 3) and 2021–2023 (Model Y).</span></li>
            </ul>
          </div>
        </div>
      </div>

      <div class="hero-gauges">
        <div class="gauge">
          <svg viewBox="0 0 120 70"><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#2a3038" stroke-width="8"/><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#f2a93b" stroke-width="8" stroke-dasharray="157" stroke-dashoffset="9.42"/></svg>
          <span class="gauge-value mono">94</span>
          <span class="gauge-label">Importance</span>
        </div>
        <div class="gauge">
          <svg viewBox="0 0 120 70"><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#2a3038" stroke-width="8"/><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#3ecf8e" stroke-width="8" stroke-dasharray="157" stroke-dashoffset="34.54"/></svg>
          <span class="gauge-value mono">78</span>
          <span class="gauge-label">Editorial Quality</span>
        </div>
        <div class="gauge">
          <svg viewBox="0 0 120 70"><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#2a3038" stroke-width="8"/><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#e2604f" stroke-width="8" stroke-dasharray="157" stroke-dashoffset="18.84"/></svg>
          <span class="gauge-value mono">88</span>
          <span class="gauge-label">Industry Impact</span>
        </div>
        <div class="gauge">
          <svg viewBox="0 0 120 70"><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#2a3038" stroke-width="8"/><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#f2a93b" stroke-width="8" stroke-dasharray="157" stroke-dashoffset="12.56"/></svg>
          <span class="gauge-value mono">92</span>
          <span class="gauge-label">Reader Interest</span>
        </div>
      </div>
    </div>

    <!--
      SCORING METHODOLOGY
      Site-wide constant (not per-article) — see SCORING_METHODOLOGY.md
      for the full weighted breakdown and rationale behind each factor.
      Update this block, not per-run, if weights change.
    -->
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

  <!--
    INDUSTRY SNAPSHOT CONTRACT
    One .stat-panel per <IndustrySnapshot> child element. Ranked lists
    use .rank-list (name + proportional bar + mention count); free-form
    groupings (trending topics, emerging tech) use .tagcloud instead.
  -->
  <section class="dashboard reveal" id="snapshot">
    <h2 class="section-title">Industry Snapshot <span class="count">Past 48 hours</span></h2>
    <div class="dash-grid">
      <div class="stat-panel">
        <h4>Top Manufacturers</h4>
        <ul class="rank-list">
          <li><span>Tesla</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:100%"></span></span><span class="rank-count">14</span></li>
          <li><span>BYD</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:82%"></span></span><span class="rank-count">12</span></li>
          <li><span>Mercedes‑Benz</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:68%"></span></span><span class="rank-count">10</span></li>
          <li><span>BMW</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:53%"></span></span><span class="rank-count">8</span></li>
          <li><span>Hyundai/Kia</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:53%"></span></span><span class="rank-count">8</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4>Top Suppliers & Networks</h4>
        <ul class="rank-list">
          <li><span>EVgo</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:100%"></span></span><span class="rank-count">5</span></li>
          <li><span>Allego</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:90%"></span></span><span class="rank-count">4</span></li>
          <li><span>Beam Global</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:70%"></span></span><span class="rank-count">3</span></li>
          <li><span>char.gy</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:55%"></span></span><span class="rank-count">2</span></li>
          <li><span>Wenea/Brixmor</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:55%"></span></span><span class="rank-count">2</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4>Most Mentioned Executives</h4>
        <ul class="rank-list">
          <li><span>Elon Musk (Tesla)</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:100%"></span></span><span class="rank-count">7</span></li>
          <li><span>Ola Källenius (Mercedes‑Benz)</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:71%"></span></span><span class="rank-count">5</span></li>
          <li><span>Milan Nedeljković (BMW)</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:57%"></span></span><span class="rank-count">4</span></li>
          <li><span>RJ Scaringe (Rivian)</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:43%"></span></span><span class="rank-count">3</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4>Trending Topics</h4>
        <div class="tagcloud">
          <span class="chip lg">Safety</span>
          <span class="chip lg">Hybrids</span>
          <span class="chip">Charging build‑out</span>
          <span class="chip">Solid‑state batteries</span>
          <span class="chip">AI & ADAS</span>
          <span class="chip">Sales & Earnings</span>
          <span class="chip">Recalls/Probes</span>
          <span class="chip">Range records</span>
        </div>
      </div>

      <div class="stat-panel">
        <h4>Emerging Technologies</h4>
        <ul class="rank-list">
          <li><span>Solid‑state cells</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:100%"></span></span><span class="rank-count">5</span></li>
          <li><span>Iron‑air LDES</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:80%"></span></span><span class="rank-count">4</span></li>
          <li><span>High‑power DC networks</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:80%"></span></span><span class="rank-count">4</span></li>
          <li><span>Cab‑less autonomy (mining)</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:60%"></span></span><span class="rank-count">3</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4>Government & Safety Activity</h4>
        <ul class="rank-list">
          <li><span>NHTSA (US)</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:100%"></span></span><span class="rank-count">3</span></li>
          <li><span>IIHS (US)</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:83%"></span></span><span class="rank-count">2</span></li>
          <li><span>UK SMMT/Grants</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:67%"></span></span><span class="rank-count">2</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4>Financial & Market Moves</h4>
        <ul class="rank-list">
          <li><span>Rivian Q2 beat; gross profit record</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:100%"></span></span><span class="rank-count">3</span></li>
          <li><span>BYD July sales +22%</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:83%"></span></span><span class="rank-count">2</span></li>
          <li><span>Tesla margin pressure</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:67%"></span></span><span class="rank-count">2</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4>Global Regions in Focus</h4>
        <ul class="rank-list">
          <li><span>United States</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:100%"></span></span><span class="rank-count">15</span></li>
          <li><span>China</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:87%"></span></span><span class="rank-count">13</span></li>
          <li><span>UK & Europe</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:73%"></span></span><span class="rank-count">11</span></li>
          <li><span>Nordics</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:47%"></span></span><span class="rank-count">7</span></li>
        </ul>
      </div>
    </div>
  </section>

  <!--
    FEATURE PANELS CONTRACT
    Five larger drill-down panels, one per named Homepage panel:
    Manufacturers, Technology, Government, Supplier, TrendingTopics.
    Each holds 3-5 .fp-row items (headline + one-line takeaway + score/date meta).
  -->
  <section class="feature-panels reveal">
    <div class="feature-panel">
      <h3>Manufacturers</h3>
      <div class="fp-row">
        <a href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">BMW pauses G‑Class rival as China headwinds bite</a>
        <div class="fp-meta"><span>Score 84</span><span>•</span><span>Autocar</span><span>•</span><span>Aug 4, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/new-mercedes-gla-ev-bigger-400-miles-range/" target="_blank" rel="noopener">Mercedes unveils new GLA EV with up to 408‑mile range</a>
        <div class="fp-meta"><span>Score 79</span><span>•</span><span>Electrek</span><span>•</span><span>Jul 29, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/28/bmw-ramps-up-ix3-output-orders-near-100000/" target="_blank" rel="noopener">BMW ramps iX3 output as orders near 100k</a>
        <div class="fp-meta"><span>Score 76</span><span>•</span><span>Electrek</span><span>•</span><span>Jul 28, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/08/04/subarus-new-trailseeker-ev-outselling-other-electric-vehicles/" target="_blank" rel="noopener">Subaru’s Trailseeker quickly tops brand’s EV sales</a>
        <div class="fp-meta"><span>Score 68</span><span>•</span><span>Electrek</span><span>•</span><span>Aug 4, 2026</span></div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Technology</h3>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">SK On and Factorial form solid‑state scaling alliance</a>
        <div class="fp-meta"><span>Score 81</span><span>•</span><span>Electrek</span><span>•</span><span>Jul 29, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/08/04/waymo-co-ceo-camera-only-self-driving-tesla/" target="_blank" rel="noopener">Waymo CEO: camera‑only autonomy hits safety ceiling</a>
        <div class="fp-meta"><span>Score 77</span><span>•</span><span>Electrek</span><span>•</span><span>Aug 4, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.greencarreports.com/news/1146043_sulfur-crystal-battery-could-triple-ev-range-without-cobalt-or-nickel" target="_blank" rel="noopener">Startup touts sulfur‑crystal cells to triple EV range</a>
        <div class="fp-meta"><span>Score 73</span><span>•</span><span>Green Car Reports</span><span>•</span><span>Aug 4, 2026</span></div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Government & Safety</h3>
      <div class="fp-row">
        <a href="https://www.electrive.com/2026/08/03/nhtsa-opens-probe-into-1-2-million-teslas/" target="_blank" rel="noopener">NHTSA opens probe into 1.2M Teslas for suspension faults</a>
        <div class="fp-meta"><span>Score 94</span><span>•</span><span>electrive</span><span>•</span><span>Aug 3, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.iihs.org/news/detail/driver-death-rates-remain-high-for-small-cars-models-with-powerful-engines" target="_blank" rel="noopener">IIHS: small cars, sports/muscle cars top death‑rate list</a>
        <div class="fp-meta"><span>Score 78</span><span>•</span><span>IIHS</span><span>•</span><span>Jul 30, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.autocar.co.uk/car-news/new-cars/mercedes-big-screens-stay-we-went-too-far-removing-buttons" target="_blank" rel="noopener">Mercedes chief: brand to reintroduce “sensible buttons”</a>
        <div class="fp-meta"><span>Score 64</span><span>•</span><span>Autocar</span><span>•</span><span>Aug 5, 2026</span></div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Suppliers & Infrastructure</h3>
      <div class="fp-row">
        <a href="https://electrek.co/2026/08/04/evgo-is-putting-500-fast-chargers-where-americans-shop/" target="_blank" rel="noopener">EVgo to add 500+ DC fast stalls at shopping centers</a>
        <div class="fp-meta"><span>Score 80</span><span>•</span><span>Electrek</span><span>•</span><span>Aug 4, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.electrive.com/2026/08/05/uk-volkswagen-gives-id-buzz-cargo-a-58-kwh-battery-and-v2l/" target="_blank" rel="noopener">VW adds 58‑kWh pack & V2L to ID. Buzz Cargo (UK)</a>
        <div class="fp-meta"><span>Score 66</span><span>•</span><span>electrive</span><span>•</span><span>Aug 5, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://chargedevs.com/newswire/beam-global-supplies-ev-arc-off-grid-charging-systems-for-dallas-municipal-fleet-and-massachusetts-carshare-pilot/" target="_blank" rel="noopener">Beam Global wins Dallas & MA off‑grid charging orders</a>
        <div class="fp-meta"><span>Score 62</span><span>•</span><span>Charged EVs</span><span>•</span><span>Aug 2, 2026</span></div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Trending Topics</h3>
      <div class="fp-row">
        <a href="https://electrek.co/2026/08/04/subarus-new-trailseeker-ev-outselling-other-electric-vehicles/" target="_blank" rel="noopener">Affordable EVs gain: Subaru’s new Trailseeker jumps early</a>
        <div class="fp-meta"><span>Score 65</span><span>•</span><span>Electrek</span><span>•</span><span>Aug 4, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.autocar.co.uk/car-news/electric-cars/evs-and-hybrids-drive-uk-car-market-best-july-covid" target="_blank" rel="noopener">EVs & hybrids power UK to best July since 2019</a>
        <div class="fp-meta"><span>Score 72</span><span>•</span><span>Autocar</span><span>•</span><span>Aug 5, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/08/04/audis-cheapest-ev-also-most-efficient-car-all-time/" target="_blank" rel="noopener">Audi A2 e‑tron teased as brand’s most efficient car</a>
        <div class="fp-meta"><span>Score 69</span><span>•</span><span>Electrek</span><span>•</span><span>Aug 4, 2026</span></div>
      </div>
    </div>
  </section>

  <!--
    LATEST ARTICLES CONTRACT
    Every .article-row = one analyzed article. score-chip shows
    ImportanceScore (0-100); add class "high" when score >= 85.
    article-take is a ONE-LINE original takeaway, never a paraphrase
    of source-article sentences. article-tags holds Entity + Topic
    chips. article-source always carries Publisher, Published date,
    and a "Read original →" link to OriginalURL.
  -->
  <section class="latest reveal" id="latest-articles">
    <h2 class="section-title">Latest Articles <span class="count">22 analyzed today</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip high">94</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/03/nhtsa-opens-probe-into-1-2-million-teslas/" target="_blank" rel="noopener">NHTSA opens probe into 1.2 million Teslas over suspension components</a>
          <div class="article-take">A US safety review puts Tesla’s largest US cohorts under scrutiny and could trigger hardware fixes or a recall.</div>
          <div class="article-tags">
            <span class="chip">Tesla</span><span class="chip">NHTSA</span><span class="chip">Safety</span><span class="chip">Recall/Investigation</span><span class="chip">United States</span>
          </div>
        </div>
        <div class="article-source">
          <span>electrive — Aug 3, 2026</span>
          <a href="https://www.electrive.com/2026/08/03/nhtsa-opens-probe-into-1-2-million-teslas/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip high">89</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">US examines Model 3/Y front suspension failures after 156 complaints</a>
          <div class="article-take">Complaint volume and part commonality across model years elevate regulatory pressure on Tesla’s core lineup.</div>
          <div class="article-tags">
            <span class="chip">Tesla</span><span class="chip">NHTSA</span><span class="chip">Safety</span><span class="chip">United States</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 31, 2026</span>
          <a href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">80</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/04/evgo-is-putting-500-fast-chargers-where-americans-shop/" target="_blank" rel="noopener">EVgo to deploy 500+ fast chargers at US shopping centers</a>
          <div class="article-take">Retail‑adjacent charging tightens convenience gaps and boosts utilization versus highway‑only hubs.</div>
          <div class="article-tags">
            <span class="chip">EVgo</span><span class="chip">Charging</span><span class="chip">Retail</span><span class="chip">United States</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 4, 2026</span>
          <a href="https://electrek.co/2026/08/04/evgo-is-putting-500-fast-chargers-where-americans-shop/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">76</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">SK On and Factorial team up to scale solid‑state batteries</a>
          <div class="article-take">A cell‑maker/OEM alliance targets manufacturability as the gating factor for next‑gen chemistries.</div>
          <div class="article-tags">
            <span class="chip">SK On</span><span class="chip">Factorial</span><span class="chip">Battery</span><span class="chip">Solid‑state</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">79</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/new-mercedes-gla-ev-bigger-400-miles-range/" target="_blank" rel="noopener">Mercedes debuts GLA EV with 800V charging, 408‑mile spec</a>
          <div class="article-take">MMA architecture pushes compact luxury crossovers toward long‑range, high‑speed charging baselines.</div>
          <div class="article-tags">
            <span class="chip">Mercedes‑Benz</span><span class="chip">EV</span><span class="chip">Charging</span><span class="chip">Manufacturing</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/new-mercedes-gla-ev-bigger-400-miles-range/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">72</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/electric-cars/evs-and-hybrids-drive-uk-car-market-best-july-covid" target="_blank" rel="noopener">EVs, PHEVs lift UK market to strongest July since 2019</a>
          <div class="article-take">Discounting and grants accelerate ZEV mandate progress even as petrol share slides.</div>
          <div class="article-tags">
            <span class="chip">UK</span><span class="chip">EV</span><span class="chip">Hybrid</span><span class="chip">Sales</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 5, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/electric-cars/evs-and-hybrids-drive-uk-car-market-best-july-covid" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip high">86</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/30/rivian-rivn-q2-2026-earnings-r2-deliveries-revenue-up-27/" target="_blank" rel="noopener">Rivian Q2: revenue +27%, record gross profit as R2 deliveries start</a>
          <div class="article-take">Improving unit economics and a sub‑$50k model move Rivian toward scale‑positive quarters.</div>
          <div class="article-tags">
            <span class="chip">Rivian</span><span class="chip">Finance</span><span class="chip">EV</span><span class="chip">Production</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 30, 2026</span>
          <a href="https://electrek.co/2026/07/30/rivian-rivn-q2-2026-earnings-r2-deliveries-revenue-up-27/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">70</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/04/audis-cheapest-ev-also-most-efficient-car-all-time/" target="_blank" rel="noopener">Audi readies A2 e‑tron as its most efficient model</a>
          <div class="article-take">VW Group’s compact EV play leans on aero and new LFP/NMC options to stretch range per kWh.</div>
          <div class="article-tags">
            <span class="chip">Audi</span><span class="chip">EV</span><span class="chip">Efficiency</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 4, 2026</span>
          <a href="https://electrek.co/2026/08/04/audis-cheapest-ev-also-most-efficient-car-all-time/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">69</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/mercedes-big-screens-stay-we-went-too-far-removing-buttons" target="_blank" rel="noopener">Mercedes: “We went too far” removing buttons; some return</a>
          <div class="article-take">User‑interface strategy shifts back toward physical controls while keeping panoramic screens.</div>
          <div class="article-tags">
            <span class="chip">Mercedes‑Benz</span><span class="chip">Software</span><span class="chip">UX</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 5, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/mercedes-big-screens-stay-we-went-too-far-removing-buttons" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">66</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/05/uk-volkswagen-gives-id-buzz-cargo-a-58-kwh-battery-and-v2l/" target="_blank" rel="noopener">VW adds 58‑kWh battery and V2L to ID. Buzz Cargo in UK</a>
          <div class="article-take">Lower‑capacity pack widens price ladder while bidirectional features suit fleet power tools.</div>
          <div class="article-tags">
            <span class="chip">Volkswagen</span><span class="chip">Commercial EV</span><span class="chip">V2L</span><span class="chip">UK</span>
          </div>
        </div>
        <div class="article-source">
          <span>electrive — Aug 5, 2026</span>
          <a href="https://www.electrive.com/2026/08/05/uk-volkswagen-gives-id-buzz-cargo-a-58-kwh-battery-and-v2l/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">71</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/04/subarus-new-trailseeker-ev-outselling-other-electric-vehicles/" target="_blank" rel="noopener">Subaru’s new Trailseeker already outsells brand’s other EVs</a>
          <div class="article-take">Adventure packaging and pricing traction suggest a clearer lane for Subaru’s electrification push.</div>
          <div class="article-tags">
            <span class="chip">Subaru</span><span class="chip">EV</span><span class="chip">Sales</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 4, 2026</span>
          <a href="https://electrek.co/2026/08/04/subarus-new-trailseeker-ev-outselling-other-electric-vehicles/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">74</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/denmark-evs-account-for-almost-all-new-car-registrations-in-july/" target="_blank" rel="noopener">Denmark: EVs hit 97% of private new‑car registrations in July</a>
          <div class="article-take">A Norway‑like milestone signals rapid Nordic adoption beyond early leaders.</div>
          <div class="article-tags">
            <span class="chip">Denmark</span><span class="chip">EV</span><span class="chip">Policy</span><span class="chip">Sales</span>
          </div>
        </div>
        <div class="article-source">
          <span>electrive — Aug 4, 2026</span>
          <a href="https://www.electrive.com/2026/08/04/denmark-evs-account-for-almost-all-new-car-registrations-in-july/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">68</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/byd-goes-after-defender-boxy-%C2%A348k-402bhp-hybrid-suv" target="_blank" rel="noopener">BYD launches Ti7 hybrid SUV in UK from £47,995</a>
          <div class="article-take">The boxy seven‑seater undercuts premium rivals and debuts BYD’s DM‑p PHEV setup in Britain.</div>
          <div class="article-tags">
            <span class="chip">BYD</span><span class="chip">Hybrid</span><span class="chip">UK</span><span class="chip">SUV</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 5, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/byd-goes-after-defender-boxy-%C2%A348k-402bhp-hybrid-suv" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">67</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/new-models-vital-ds-survival-uk-sales-hit-record-low" target="_blank" rel="noopener">DS UK sales slump; new N°3/N°7 models critical to rebound</a>
          <div class="article-take">Brand consolidation and product cadence will determine DS’s survival in a shrinking premium niche.</div>
          <div class="article-tags">
            <span class="chip">DS Automobiles</span><span class="chip">Sales</span><span class="chip">Strategy</span><span class="chip">UK</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 5, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/new-models-vital-ds-survival-uk-sales-hit-record-low" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </section>

  <!--
    NEWS SECTIONS CONTRACT
    One <div class="sec-group" id="{slug}"> per <Sections> child,
    slug matching the nav anchors above. Same .article-row markup
    as Latest Articles, filtered to that section's classification.
  -->
  <div class="sec-group reveal" id="industry-news">
    <h2 class="section-title">Industry News <span class="count">5 items</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip high">89</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">US investigates Tesla Model 3/Y suspension complaints</a>
          <div class="article-take">Large‑scale probe raises potential warranty and recall exposure.</div>
          <div class="article-tags"><span class="chip">Industry</span><span class="chip">Safety</span><span class="chip">Tesla</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 31, 2026</span>
          <a href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">72</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/electric-cars/evs-and-hybrids-drive-uk-car-market-best-july-covid" target="_blank" rel="noopener">UK: EVs & hybrids drive best July since pre‑pandemic</a>
          <div class="article-take">Mandates, grants and discounts are resetting buyer mix toward electrified models.</div>
          <div class="article-tags"><span class="chip">UK</span><span class="chip">Sales</span><span class="chip">EV</span><span class="chip">Hybrid</span></div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 5, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/electric-cars/evs-and-hybrids-drive-uk-car-market-best-july-covid" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">66</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/denmark-evs-account-for-almost-all-new-car-registrations-in-july/" target="_blank" rel="noopener">Denmark hits 97% EV share for private registrations</a>
          <div class="article-take">Nordic demand compresses ICE residuals and speeds infrastructure ROI cycles.</div>
          <div class="article-tags"><span class="chip">Denmark</span><span class="chip">EV</span><span class="chip">Policy</span></div>
        </div>
        <div class="article-source">
          <span>electrive — Aug 4, 2026</span>
          <a href="https://www.electrive.com/2026/08/04/denmark-evs-account-for-almost-all-new-car-registrations-in-july/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">67</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/new-models-vital-ds-survival-uk-sales-hit-record-low" target="_blank" rel="noopener">DS sales slide; turnaround hinges on new models</a>
          <div class="article-take">Portfolio rationalization stresses the need for volume entries in Europe.</div>
          <div class="article-tags"><span class="chip">DS</span><span class="chip">Strategy</span><span class="chip">Europe</span></div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 5, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/new-models-vital-ds-survival-uk-sales-hit-record-low" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">64</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/03/hyundai-kias-record-us-sales-run/" target="_blank" rel="noopener">Hyundai & Kia extend US record streak on hybrid strength</a>
          <div class="article-take">Electrified mix offsets softer pure‑EV pockets while capacity scales in NA.</div>
          <div class="article-tags"><span class="chip">Hyundai</span><span class="chip">Kia</span><span class="chip">Sales</span><span class="chip">Hybrid</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 3, 2026</span>
          <a href="https://electrek.co/2026/08/03/hyundai-kias-record-us-sales-run/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="electric-vehicles">
    <h2 class="section-title">Electric Vehicles <span class="count">5 items</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip">79</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/new-mercedes-gla-ev-bigger-400-miles-range/" target="_blank" rel="noopener">New Mercedes GLA EV targets 408‑mile range and 320 kW charging</a>
          <div class="article-take">Compact luxury EVs move upmarket on both efficiency and charge speed.</div>
          <div class="article-tags"><span class="chip">Mercedes‑Benz</span><span class="chip">EV</span><span class="chip">Charging</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/new-mercedes-gla-ev-bigger-400-miles-range/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">70</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/04/audis-cheapest-ev-also-most-efficient-car-all-time/" target="_blank" rel="noopener">Audi A2 e‑tron previewed as brand’s most efficient car</a>
          <div class="article-take">Aero‑first design and updated MEB tech underpin range gains.</div>
          <div class="article-tags"><span class="chip">Audi</span><span class="chip">Efficiency</span><span class="chip">EV</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 4, 2026</span>
          <a href="https://electrek.co/2026/08/04/audis-cheapest-ev-also-most-efficient-car-all-time/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">71</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/04/subarus-new-trailseeker-ev-outselling-other-electric-vehicles/" target="_blank" rel="noopener">Subaru’s Trailseeker outpaces brand’s other EVs</a>
          <div class="article-take">Adventure branding resonates as the market leans toward practical EVs.</div>
          <div class="article-tags"><span class="chip">Subaru</span><span class="chip">EV</span><span class="chip">Sales</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 4, 2026</span>
          <a href="https://electrek.co/2026/08/04/subarus-new-trailseeker-ev-outselling-other-electric-vehicles/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">66</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/05/uk-volkswagen-gives-id-buzz-cargo-a-58-kwh-battery-and-v2l/" target="_blank" rel="noopener">ID. Buzz Cargo gets smaller pack and V2L in UK</a>
          <div class="article-take">Spec diversification addresses total cost of ownership for fleets.</div>
          <div class="article-tags"><span class="chip">Volkswagen</span><span class="chip">Commercial EV</span><span class="chip">V2L</span></div>
        </div>
        <div class="article-source">
          <span>electrive — Aug 5, 2026</span>
          <a href="https://www.electrive.com/2026/08/05/uk-volkswagen-gives-id-buzz-cargo-a-58-kwh-battery-and-v2l/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">65</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/30/tesla-10-millionth-vehicle-ev-growth-stalled/" target="_blank" rel="noopener">Tesla hits 10M vehicles as EV growth plateaus</a>
          <div class="article-take">Scale milestone arrives amid slower output versus installed capacity.</div>
          <div class="article-tags"><span class="chip">Tesla</span><span class="chip">Production</span><span class="chip">EV</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 30, 2026</span>
          <a href="https://electrek.co/2026/07/30/tesla-10-millionth-vehicle-ev-growth-stalled/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="manufacturers">
    <h2 class="section-title">Manufacturers <span class="count">4 items</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip">84</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">BMW shelves hardcore off‑roader amid China shift</a>
          <div class="article-take">Portfolio review prioritizes demand certainty and capital efficiency.</div>
          <div class="article-tags"><span class="chip">BMW</span><span class="chip">Strategy</span><span class="chip">China</span></div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 5, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">68</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/byd-goes-after-defender-boxy-%C2%A348k-402bhp-hybrid-suv" target="_blank" rel="noopener">BYD’s Ti7 PHEV undercuts premium 4x4s in UK</a>
          <div class="article-take">Aggressive pricing and DM‑p tech broaden BYD’s European reach.</div>
          <div class="article-tags"><span class="chip">BYD</span><span class="chip">Hybrid</span><span class="chip">UK</span></div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 5, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/byd-goes-after-defender-boxy-%C2%A348k-402bhp-hybrid-suv" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">71</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/04/subarus-new-trailseeker-ev-outselling-other-electric-vehicles/" target="_blank" rel="noopener">Subaru’s Trailseeker tops brand EV sales mix</a>
          <div class="article-take">Early traction validates adventurous positioning for mainstream electrics.</div>
          <div class="article-tags"><span class="chip">Subaru</span><span class="chip">EV</span><span class="chip">Sales</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 4, 2026</span>
          <a href="https://electrek.co/2026/08/04/subarus-new-trailseeker-ev-outselling-other-electric-vehicles/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">64</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/03/hyundai-kias-record-us-sales-run/" target="_blank" rel="noopener">Hyundai/Kia extend US record run led by hybrids</a>
          <div class="article-take">Hybrid volume cushions cyclicality in EV adoption curves.</div>
          <div class="article-tags"><span class="chip">Hyundai</span><span class="chip">Kia</span><span class="chip">Hybrid</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 3, 2026</span>
          <a href="https://electrek.co/2026/08/03/hyundai-kias-record-us-sales-run/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="dealers">
    <h2 class="section-title">Dealers <span class="count">1 item</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip">60</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/company-cars/used-ev-repair-scheme-looks-tackle-cliff-edge-residual-drops" target="_blank" rel="noopener">BCA opens HV repair facility to support used‑EV values</a>
          <div class="article-take">Battery repair and health certificates aim to stabilize residuals and speed turnover.</div>
          <div class="article-tags"><span class="chip">Dealers</span><span class="chip">Used EVs</span><span class="chip">Battery</span></div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 5, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/company-cars/used-ev-repair-scheme-looks-tackle-cliff-edge-residual-drops" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="suppliers">
    <h2 class="section-title">Suppliers <span class="count">3 items</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip">80</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/04/evgo-is-putting-500-fast-chargers-where-americans-shop/" target="_blank" rel="noopener">EVgo to add 500+ fast chargers across US retail sites</a>
          <div class="article-take">Retail partnerships shift fast‑charge dwell into daily errands.</div>
          <div class="article-tags"><span class="chip">EVgo</span><span class="chip">Charging</span><span class="chip">Retail</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 4, 2026</span>
          <a href="https://electrek.co/2026/08/04/evgo-is-putting-500-fast-chargers-where-americans-shop/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">62</div>
        <div class="article-main">
          <a class="headline" href="https://chargedevs.com/newswire/beam-global-supplies-ev-arc-off-grid-charging-systems-for-dallas-municipal-fleet-and-massachusetts-carshare-pilot/" target="_blank" rel="noopener">Beam Global ships off‑grid chargers to Dallas & MA pilot</a>
          <div class="article-take">Solar + storage avoids trenching delays for municipal deployments.</div>
          <div class="article-tags"><span class="chip">Beam Global</span><span class="chip">Infrastructure</span></div>
        </div>
        <div class="article-source">
          <span>Charged EVs — Aug 2, 2026</span>
          <a href="https://chargedevs.com/newswire/beam-global-supplies-ev-arc-off-grid-charging-systems-for-dallas-municipal-fleet-and-massachusetts-carshare-pilot/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">58</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/03/devon-and-torbay-commission-nearly-3000-public-ev-charging-points/" target="_blank" rel="noopener">UK councils commission ~3,000 kerbside chargers</a>
          <div class="article-take">Believ, char.gy and Wenea split rollout to expand on‑street access.</div>
          <div class="article-tags"><span class="chip">UK</span><span class="chip">char.gy</span><span class="chip">Believ</span><span class="chip">Wenea</span></div>
        </div>
        <div class="article-source">
          <span>electrive — Aug 3, 2026</span>
          <a href="https://www.electrive.com/2026/08/03/devon-and-torbay-commission-nearly-3000-public-ev-charging-points/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="government">
    <h2 class="section-title">Government <span class="count">3 items</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip high">94</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/03/nhtsa-opens-probe-into-1-2-million-teslas/" target="_blank" rel="noopener">NHTSA opens suspension probe into 1.2M Teslas</a>
          <div class="article-take">Regulatory scrutiny intensifies on core Tesla models after defect reports.</div>
          <div class="article-tags"><span class="chip">NHTSA</span><span class="chip">Safety</span><span class="chip">Tesla</span></div>
        </div>
        <div class="article-source">
          <span>electrive — Aug 3, 2026</span>
          <a href="https://www.electrive.com/2026/08/03/nhtsa-opens-probe-into-1-2-million-teslas/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">78</div>
        <div class="article-main">
          <a class="headline" href="https://www.iihs.org/news/detail/driver-death-rates-remain-high-for-small-cars-models-with-powerful-engines" target="_blank" rel="noopener">IIHS: small cars, powerful models lead driver death rates</a>
          <div class="article-take">Risk profiles diverge sharply by vehicle class and performance tier.</div>
          <div class="article-tags"><span class="chip">IIHS</span><span class="chip">Safety</span><span class="chip">Analysis</span></div>
        </div>
        <div class="article-source">
          <span>IIHS — Jul 30, 2026</span>
          <a href="https://www.iihs.org/news/detail/driver-death-rates-remain-high-for-small-cars-models-with-powerful-engines" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">66</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/denmark-evs-account-for-almost-all-new-car-registrations-in-july/" target="_blank" rel="noopener">Denmark posts 97% EV share for private buyers in July</a>
          <div class="article-take">Policy and price realignment fuel rapid private‑market electrification.</div>
          <div class="article-tags"><span class="chip">Denmark</span><span class="chip">Policy</span><span class="chip">EV</span></div>
        </div>
        <div class="article-source">
          <span>electrive — Aug 4, 2026</span>
          <a href="https://www.electrive.com/2026/08/04/denmark-evs-account-for-almost-all-new-car-registrations-in-july/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="technology">
    <h2 class="section-title">Technology <span class="count">4 items</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip">77</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/04/waymo-co-ceo-camera-only-self-driving-tesla/" target="_blank" rel="noopener">Waymo: camera‑only self‑driving won’t reach superhuman safety</a>
          <div class="article-take">Sensor‑stack choices remain a core strategic split in autonomy.</div>
          <div class="article-tags"><span class="chip">Autonomous</span><span class="chip">ADAS</span><span class="chip">Waymo</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 4, 2026</span>
          <a href="https://electrek.co/2026/08/04/waymo-co-ceo-camera-only-self-driving-tesla/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">76</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">SK On + Factorial align to industrialize solid‑state</a>
          <div class="article-take">Partnership targets scale, not just lab wins, in next‑gen cells.</div>
          <div class="article-tags"><span class="chip">Battery</span><span class="chip">Solid‑state</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">73</div>
        <div class="article-main">
          <a class="headline" href="https://www.greencarreports.com/news/1146043_sulfur-crystal-battery-could-triple-ev-range-without-cobalt-or-nickel" target="_blank" rel="noopener">Sulfur‑crystal battery claims 3× range without cobalt/nickel</a>
          <div class="article-take">If validated at scale, new chemistry could cut costs and supply risk.</div>
          <div class="article-tags"><span class="chip">Battery</span><span class="chip">Materials</span></div>
        </div>
        <div class="article-source">
          <span>Green Car Reports — Aug 4, 2026</span>
          <a href="https://www.greencarreports.com/news/1146043_sulfur-crystal-battery-could-triple-ev-range-without-cobalt-or-nickel" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">69</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/mercedes-big-screens-stay-we-went-too-far-removing-buttons" target="_blank" rel="noopener">Mercedes to reintroduce physical controls in UI refresh</a>
          <div class="article-take">HMI strategy balances large screens with tactile shortcuts.</div>
          <div class="article-tags"><span class="chip">Software</span><span class="chip">UX</span><span class="chip">Mercedes‑Benz</span></div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 5, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/mercedes-big-screens-stay-we-went-too-far-removing-buttons" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="finance">
    <h2 class="section-title">Finance <span class="count">3 items</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip high">86</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/30/rivian-rivn-q2-2026-earnings-r2-deliveries-revenue-up-27/" target="_blank" rel="noopener">Rivian revenue +27% with record gross profit</a>
          <div class="article-take">Scaling plus lower BOM costs show a credible path toward profitability.</div>
          <div class="article-tags"><span class="chip">Earnings</span><span class="chip">Rivian</span><span class="chip">EV</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 30, 2026</span>
          <a href="https://electrek.co/2026/07/30/rivian-rivn-q2-2026-earnings-r2-deliveries-revenue-up-27/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">74</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/business-corporate/cheap-cars-hit-tesla-profits-tech-pivot-stalls" target="_blank" rel="noopener">Tesla margins slump despite higher deliveries</a>
          <div class="article-take">Price cuts and cheaper trims weigh on ASPs as robotaxi timelines slip.</div>
          <div class="article-tags"><span class="chip">Tesla</span><span class="chip">Margins</span><span class="chip">Strategy</span></div>
        </div>
        <div class="article-source">
          <span>Autocar — Jul 31, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/business-corporate/cheap-cars-hit-tesla-profits-tech-pivot-stalls" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">72</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/03/byd-boosts-sales-by-22-in-july/" target="_blank" rel="noopener">BYD July sales +22% with export share at record 43%</a>
          <div class="article-take">Overseas growth offsets softer China demand as competition intensifies.</div>
          <div class="article-tags"><span class="chip">BYD</span><span class="chip">Sales</span><span class="chip">Exports</span></div>
        </div>
        <div class="article-source">
          <span>electrive — Aug 3, 2026</span>
          <a href="https://www.electrive.com/2026/08/03/byd-boosts-sales-by-22-in-july/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="international">
    <h2 class="section-title">International <span class="count">3 items</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip">74</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/denmark-evs-account-for-almost-all-new-car-registrations-in-july/" target="_blank" rel="noopener">Denmark nears universal private EV adoption in July</a>
          <div class="article-take">Another Nordic market crosses a symbolic EV threshold.</div>
          <div class="article-tags"><span class="chip">Denmark</span><span class="chip">EV</span><span class="chip">Market</span></div>
        </div>
        <div class="article-source">
          <span>electrive — Aug 4, 2026</span>
          <a href="https://www.electrive.com/2026/08/04/denmark-evs-account-for-almost-all-new-car-registrations-in-july/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">68</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/electric-cars/evs-and-hybrids-drive-uk-car-market-best-july-covid" target="_blank" rel="noopener">UK car market posts best July since 2019 on EV/hybrid lift</a>
          <div class="article-take">Policy, pricing and fuel costs shift buyer behavior.</div>
          <div class="article-tags"><span class="chip">UK</span><span class="chip">Sales</span><span class="chip">EV</span></div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 5, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/electric-cars/evs-and-hybrids-drive-uk-car-market-best-july-covid" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">63</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/philippines-launches-e850m-incentive-programme-for-ev-manufacturing/" target="_blank" rel="noopener">Philippines launches €850m EV manufacturing incentives</a>
          <div class="article-take">Production subsidies expand Southeast Asia’s supply‑chain footprint.</div>
          <div class="article-tags"><span class="chip">Philippines</span><span class="chip">Policy</span><span class="chip">Manufacturing</span></div>
        </div>
        <div class="article-source">
          <span>electrive — Aug 4, 2026</span>
          <a href="https://www.electrive.com/2026/08/04/philippines-launches-e850m-incentive-programme-for-ev-manufacturing/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="opinion">
    <h2 class="section-title">Opinion <span class="count">2 items</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip">58</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/mercedes-big-screens-stay-we-went-too-far-removing-buttons" target="_blank" rel="noopener">Opinion: Big screens stay, but buttons matter again</a>
          <div class="article-take">Carmakers are rediscovering ergonomics as a competitive edge in software‑defined cars.</div>
          <div class="article-tags"><span class="chip">UX</span><span class="chip">Design</span><span class="chip">Mercedes‑Benz</span></div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 5, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/mercedes-big-screens-stay-we-went-too-far-removing-buttons" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">55</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/04/waymo-co-ceo-camera-only-self-driving-tesla/" target="_blank" rel="noopener">Analysis: Why sensor choices still split AV strategies</a>
          <div class="article-take">Diverse safety cases keep lidar vs. camera debates very much alive.</div>
          <div class="article-tags"><span class="chip">Autonomous</span><span class="chip">Lidar</span><span class="chip">Safety</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 4, 2026</span>
          <a href="https://electrek.co/2026/08/04/waymo-co-ceo-camera-only-self-driving-tesla/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

</main>

<footer>
  <p class="legal-note mono" style="font-family:'IBM Plex Sans',sans-serif;">
    AutoIntel Intelligence analyzes and scores publicly reported automotive industry news.
    Headlines, executive summaries, takeaways and scores on this page are original editorial
    analysis produced by AutoIntel — we do not reproduce source-article text. Every item links
    to its original publisher; please read the full story there for complete reporting and context.
  </p>
</footer>

<script>
document.getElementById('publishDate').textContent = new Date().toLocaleDateString('en-US',{weekday:'long',year:'numeric',month:'long',day:'numeric'}).toUpperCase();

(function(){
  var toggle = document.getElementById('sectionNavToggle');
  var nav = document.getElementById('sectionNav');
  if (!toggle || !nav) return;
  toggle.addEventListener('click', function(){
    var open = nav.classList.toggle('is-open');
    toggle.setAttribute('aria-expanded', open ? 'true' : 'false');
  });
  nav.addEventListener('click', function(e){
    if (e.target.tagName === 'A') {
      nav.classList.remove('is-open');
      toggle.setAttribute('aria-expanded', 'false');
    }
  });
})();

(function(){
  var track = document.getElementById('tickerTrack');
  if (track) track.innerHTML += track.innerHTML; // seamless loop
})();

(function(){
  var reveals = Array.prototype.slice.call(document.querySelectorAll('.reveal'));
  if (!reveals.length || !('IntersectionObserver' in window)) {
    reveals.forEach(function(el){ el.classList.add('is-visible'); });
    return;
  }
  var observer = new IntersectionObserver(function(entries){
    entries.forEach(function(entry){
      if (entry.isIntersecting) {
        entry.target.classList.add('is-visible');
        observer.unobserve(entry.target);
      }
    });
  }, { threshold: 0.1, rootMargin: '0px 0px -40px 0px' });
  reveals.forEach(function(el){ observer.observe(el); });
})();
</script>

</body>
</html>