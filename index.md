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
.section-title .count{
  font-family:'IBM Plex Mono',monospace;
  font-size:11px;
  color:var(--ink-dim);
  font-weight:400;
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

<!--
  TICKER CONTRACT
  One .ticker-item per trending entity/topic. {{TICKER_ICON}} is a
  complete pre-classed 14x14 icon element (class="ticker-icon"; entity
  logo or topic glyph) placed before the label — same convention as
  {{PANEL_ICON}} above. Omit it entirely if no icon is available for
  that item rather than leaving an empty box.
-->
<div class="ticker" aria-label="Trending entities and topics">
  <div class="ticker-track" id="tickerTrack">
    <span class="ticker-item"><b>Tesla</b> NHTSA opens 1.2M-vehicle suspension probe <span class="ticker-down">▼</span></span>
    <span class="ticker-item"><b>Mercedes-Benz</b> New GLA EV rated up to 408 miles <span class="ticker-up">▲</span></span>
    <span class="ticker-item"><b>UK Market</b> EVs/hybrids lift best July since 2019 <span class="ticker-up">▲</span></span>
    <span class="ticker-item"><b>Volvo</b> Drops lidar on EX90/ES90, compensates owners <span class="ticker-flat">■</span></span>
    <span class="ticker-item"><b>Ram</b> Recalls 1.5M 1500 trucks over rear seat belts <span class="ticker-down">▼</span></span>
    <span class="ticker-item"><b>Kia PV5</b> Captures 37% of small EV van market in EU/UK <span class="ticker-up">▲</span></span>
    <span class="ticker-item"><b>BYD Denza Z9S</b> 1,100 km EV opens pre-orders <span class="ticker-up">▲</span></span>
    <span class="ticker-item"><b>Hyundai &amp; Kia</b> Record US sales as hybrids surge <span class="ticker-up">▲</span></span>
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
        <h1>NHTSA opens investigation into 1.2 million Tesla Model 3 and Model Y vehicles over front suspension failures</h1>
        <p class="dek">US auto-safety regulator NHTSA launched a defect probe focused on front lower lateral links detaching on certain 2018–2023 Teslas.</p>

        <div class="source-strip">
          <span>Source: <b>Electrek</b></span>
          <span>Aug 5, 2026</span>
          <a href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">Read original →</a>
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
              <span class="chip stock down"><span class="tk">TSLA</span><span class="chg">N/A</span></span>
            </div>
          </div>
          <div class="entity-field">
            <span class="ef-label">Topics</span>
            <div class="chip-row">
              <span class="chip">Safety</span>
              <span class="chip">Recall</span>
              <span class="chip">Government</span>
              <span class="chip">Suspension</span>
            </div>
          </div>
          <div class="entity-field wide">
            <span class="ef-label">Related Stories</span>
            <ul class="data-list">
              <li><a href="https://electrek.co/2026/08/04/tesla-china-sales-crash-exports-surge-h1-2026/" target="_blank" rel="noopener">Tesla China sales slump as exports surge</a></li>
              <li><a href="https://www.caranddriver.com/news/a73319471/ram-1500-seatbelt-buckle-one-million-truck-recall/" target="_blank" rel="noopener">Ram recalls ~1.3M 1500 pickups over seat-belt anchors</a></li>
              <li><a href="https://www.autocar.co.uk/car-news/business-corporate/cheap-cars-hit-tesla-profits-tech-pivot-stalls" target="_blank" rel="noopener">Tesla Q2 profits drop as pricing erodes margins</a></li>
            </ul>
          </div>
          <div class="entity-field wide">
            <span class="ef-label">Timeline</span>
            <ul class="timeline-list">
              <li><span class="t-date mono">2018–2023</span><span>Model years included in probe: Model 3 (2018–2020) and Model Y (2021–2023)</span></li>
              <li><span class="t-date mono">Jul 31, 2026</span><span>NHTSA opens preliminary evaluation into front lower lateral link separation</span></li>
              <li><span class="t-date mono">Aug 2026</span><span>Investigation active; Tesla and NHTSA collecting field data and owner complaints</span></li>
            </ul>
          </div>
        </div>
      </div>

      <div class="hero-gauges">
        <div class="gauge">
          <svg viewBox="0 0 120 70"><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#2a3038" stroke-width="8"/><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#f2a93b" stroke-width="8" stroke-dasharray="157" stroke-dashoffset="12.9"/></svg>
          <span class="gauge-value mono">92</span>
          <span class="gauge-label">Importance</span>
        </div>
        <div class="gauge">
          <svg viewBox="0 0 120 70"><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#2a3038" stroke-width="8"/><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#3ecf8e" stroke-width="8" stroke-dasharray="157" stroke-dashoffset="18.84"/></svg>
          <span class="gauge-value mono">88</span>
          <span class="gauge-label">Editorial Quality</span>
        </div>
        <div class="gauge">
          <svg viewBox="0 0 120 70"><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#2a3038" stroke-width="8"/><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#e2604f" stroke-width="8" stroke-dasharray="157" stroke-dashoffset="23.55"/></svg>
          <span class="gauge-value mono">85</span>
          <span class="gauge-label">Industry Impact</span>
        </div>
        <div class="gauge">
          <svg viewBox="0 0 120 70"><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#2a3038" stroke-width="8"/><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#f2a93b" stroke-width="8" stroke-dasharray="157" stroke-dashoffset="15.7"/></svg>
          <span class="gauge-value mono">90</span>
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
    Each panel's <h4> leads with {{PANEL_ICON}}: a complete, pre-classed
    32x32 icon element for that metric, e.g. <svg class="panel-icon"
    viewBox="...">...</svg> or <img class="panel-icon" src="...">
    (e.g. a factory glyph for "Manufacturer Mentions"). The generation
    step outputs the whole tag, class included, not just a URL/path.
    Drop it entirely for a panel with no matching icon rather than
    leaving an empty box, e.g.: <h4>{{PANEL_ICON}}Manufacturer Mentions</h4>
  -->
  <section class="dashboard reveal" id="snapshot">
    <h2 class="section-title">Industry Snapshot <span class="count">Today</span></h2>
    <div class="dash-grid">
      
      <div class="stat-panel">
        <h4>Top Manufacturers</h4>
        <ul class="rank-list">
          <li><span>Tesla</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:100%"></span></span><span class="rank-count">12</span></li>
          <li><span>Mercedes-Benz</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:78%"></span></span><span class="rank-count">9</span></li>
          <li><span>BYD</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:70%"></span></span><span class="rank-count">8</span></li>
          <li><span>BMW</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:61%"></span></span><span class="rank-count">7</span></li>
          <li><span>Hyundai / Kia</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:57%"></span></span><span class="rank-count">6</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4>Top Suppliers</h4>
        <ul class="rank-list">
          <li><span>EVgo</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:90%"></span></span><span class="rank-count">9</span></li>
          <li><span>Kempower</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:70%"></span></span><span class="rank-count">7</span></li>
          <li><span>Factorial Energy</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:60%"></span></span><span class="rank-count">6</span></li>
          <li><span>SK On</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:50%"></span></span><span class="rank-count">5</span></li>
          <li><span>Luminar</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:40%"></span></span><span class="rank-count">4</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4>Most Mentioned Executives</h4>
        <ul class="rank-list">
          <li><span>Ola Källenius (Mercedes)</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:88%"></span></span><span class="rank-count">8</span></li>
          <li><span>Elon Musk (Tesla)</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:77%"></span></span><span class="rank-count">7</span></li>
          <li><span>Milan Nedeljković (BMW)</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:55%"></span></span><span class="rank-count">5</span></li>
          <li><span>Michael Leiters (Porsche)</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:44%"></span></span><span class="rank-count">4</span></li>
          <li><span>Silvio Napoli (Lucid)</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:33%"></span></span><span class="rank-count">3</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4>Trending Topics</h4>
        <div class="tagcloud">
          <span class="chip lg">Safety &amp; Recalls</span>
          <span class="chip">EV Market Share</span>
          <span class="chip">Solid‑State Batteries</span>
          <span class="chip">Charging Networks</span>
          <span class="chip">ADAS &amp; Lidar</span>
          <span class="chip">China Strategy</span>
          <span class="chip">Hybrids</span>
        </div>
      </div>

      <div class="stat-panel">
        <h4>Emerging Technologies</h4>
        <div class="tagcloud">
          <span class="chip">Solid‑State Cells (SK On × Factorial)</span>
          <span class="chip">Sodium‑Ion Packs</span>
          <span class="chip">Iron‑Air Long‑Duration Storage</span>
          <span class="chip">Robotaxi UX</span>
        </div>
      </div>

      <div class="stat-panel">
        <h4>Government &amp; Regulation</h4>
        <ul class="rank-list">
          <li><span>NHTSA (US)</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:100%"></span></span><span class="rank-count">10</span></li>
          <li><span>UK ZEV/Grants</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:70%"></span></span><span class="rank-count">7</span></li>
          <li><span>India PM E‑DRIVE</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:50%"></span></span><span class="rank-count">5</span></li>
          <li><span>Nordic EV Policies</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:40%"></span></span><span class="rank-count">4</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4>Financial &amp; Market Activity</h4>
        <ul class="rank-list">
          <li><span>Tesla Profit &amp; Pricing</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:90%"></span></span><span class="rank-count">9</span></li>
          <li><span>Lucid Delay/Reset</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:60%"></span></span><span class="rank-count">6</span></li>
          <li><span>BMW Orders Ramp</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:55%"></span></span><span class="rank-count">5</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4>Global Regions in Focus</h4>
        <div class="tagcloud">
          <span class="chip">United States</span>
          <span class="chip">United Kingdom</span>
          <span class="chip">China</span>
          <span class="chip">Nordics</span>
          <span class="chip">EU</span>
          <span class="chip">India</span>
        </div>
      </div>

    </div>
  </section>

  <!--
    FEATURE PANELS CONTRACT
    Five larger drill-down panels, one per named Homepage panel:
    Manufacturers, Technology, Government, Supplier, TrendingTopics.
    Each holds 3-5 .fp-row items (headline + one-line takeaway + score/date meta).
    Each panel's <h3> leads with {{FEATURE_ICON}}: a complete pre-classed
    40x40 icon element (class="fp-icon") for that panel's category — a
    larger sibling of {{PANEL_ICON}}, kept as its own variable since
    feature panels are a bigger, separately-themed icon than the compact
    dashboard metrics above. Drop it entirely if no icon exists, e.g.:
    <h3>{{FEATURE_ICON}}Manufacturers</h3>
  -->
  <section class="feature-panels reveal">
    
    <div class="feature-panel">
      <h3>Manufacturers</h3>
      <div class="fp-row">
        <a href="https://www.autocar.co.uk/car-news/electric-cars/new-mercedes-gla-revealed-audi-q4-rival-408-mile-range" target="_blank" rel="noopener">Mercedes GLA EV revealed with up to 408-mile range</a>
        <div class="fp-meta"><span>Score 88</span><span>•</span><span>Aug 5, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">BMW pauses G‑Class rival as China headwinds bite</a>
        <div class="fp-meta"><span>Score 74</span><span>•</span><span>Aug 5, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/08/05/hyundai-kias-record-us-sales-run/" target="_blank" rel="noopener">Hyundai &amp; Kia notch another US sales record on hybrids</a>
        <div class="fp-meta"><span>Score 66</span><span>•</span><span>Aug 5, 2026</span></div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Technology</h3>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">SK On, Factorial align to scale solid‑state batteries</a>
        <div class="fp-meta"><span>Score 69</span><span>•</span><span>Jul 29, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Volvo drops lidar on EX90/ES90; pays owner compensation</a>
        <div class="fp-meta"><span>Score 82</span><span>•</span><span>Jul 29, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.greencarreports.com/news/1146023_study-tesla-rivian-charging-networks-have-far-fewer-problems" target="_blank" rel="noopener">Study: Tesla &amp; Rivian networks have fewer charging issues</a>
        <div class="fp-meta"><span>Score 64</span><span>•</span><span>Aug 1, 2026</span></div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Government &amp; Safety</h3>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">NHTSA opens probe into 1.2M Teslas for suspension issue</a>
        <div class="fp-meta"><span>Score 92</span><span>•</span><span>Jul 31, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.caranddriver.com/news/a73319471/ram-1500-seatbelt-buckle-one-million-truck-recall/" target="_blank" rel="noopener">Ram recalls ~1.3M 1500 trucks for second‑row belt anchors</a>
        <div class="fp-meta"><span>Score 78</span><span>•</span><span>Aug 4, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.autocar.co.uk/car-news/electric-cars/evs-and-hybrids-drive-uk-car-market-best-july-covid" target="_blank" rel="noopener">UK: EVs/hybrids power best July since Covid</a>
        <div class="fp-meta"><span>Score 80</span><span>•</span><span>Aug 5, 2026</span></div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Suppliers &amp; Infrastructure</h3>
      <div class="fp-row">
        <a href="https://electrek.co/2026/08/04/evgo-is-putting-500-fast-chargers-where-americans-shop/" target="_blank" rel="noopener">EVgo to add 500+ fast chargers at shopping centers</a>
        <div class="fp-meta"><span>Score 68</span><span>•</span><span>Aug 4, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.electrive.com/2026/08/05/kempower-launches-ev-charger-leasing-model-in-the-uk/" target="_blank" rel="noopener">Kempower launches charger leasing model in the UK</a>
        <div class="fp-meta"><span>Score 60</span><span>•</span><span>Aug 5, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.autocar.co.uk/car-news/company-cars/used-ev-repair-scheme-looks-tackle-cliff-edge-residual-drops" target="_blank" rel="noopener">BCA opens battery repair hub to bolster used‑EV values</a>
        <div class="fp-meta"><span>Score 62</span><span>•</span><span>Aug 5, 2026</span></div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Trending Topics</h3>
      <div class="fp-row">
        <a href="https://www.autocar.co.uk/car-news/business-manufacturing/chinese-car-makers-all-share-parts-will-world-follow" target="_blank" rel="noopener">China’s shared-parts playbook pressures global costs</a>
        <div class="fp-meta"><span>Score 72</span><span>•</span><span>Aug 5, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/08/05/uk-records-strongest-ev-july-to-date/" target="_blank" rel="noopener">Nordics &amp; UK post record BEV shares in July</a>
        <div class="fp-meta"><span>Score 65</span><span>•</span><span>Aug 5, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">Solid‑state alliances accelerate commercialization</a>
        <div class="fp-meta"><span>Score 69</span><span>•</span><span>Jul 29, 2026</span></div>
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

    Between score-chip and article-main sits an optional .article-thumb
    (120x68 recommended source size, displayed at 96px wide):
      <div class="article-thumb"><img src="{{ARTICLE_THUMBNAIL}}" alt="" loading="lazy"></div>
    This same .article-row / .article-thumb markup is reused verbatim
    in the News Sections groups below. .article-row's grid columns are
    fixed in CSS, so for a row with no thumbnail just omit the whole
    .article-thumb div — the column stays reserved as blank space and
    the rest of the row still lines up with its neighbors.
  -->
  <section class="latest reveal" id="latest-articles">
    <h2 class="section-title">Latest Articles <span class="count">20 analyzed today</span></h2>
    <div class="article-table">
      
      <div class="article-row">
        <div class="score-chip high">92</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">NHTSA probes 1.2M Tesla Model 3/Y over suspension failures</a>
          <div class="article-take">A US safety review of detached front links puts Tesla’s highest‑volume models under fresh regulatory scrutiny.</div>
          <div class="article-tags">
            <span class="chip">Tesla</span><span class="chip">Safety</span><span class="chip">Government</span><span class="chip">Recall</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 31, 2026</span>
          <a href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip high">88</div>
        <div class="article-thumb"><img src="https://images.cdn.autocar.co.uk/sites/autocar.co.uk/files/styles/car_review_image_190/public/images/car-reviews/first-drives/legacy/merceds-gla-2026-017.jpg?itok=IqCN5gha" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/electric-cars/new-mercedes-gla-revealed-audi-q4-rival-408-mile-range" target="_blank" rel="noopener">New Mercedes GLA EV revealed with up to 408-mile range</a>
          <div class="article-take">Mercedes’ compact MMA platform brings 800V fast charging and class‑leading efficiency to its smallest SUV.</div>
          <div class="article-tags">
            <span class="chip">Mercedes-Benz</span><span class="chip">EV</span><span class="chip">Technology</span><span class="chip">Manufacturing</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 5, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/electric-cars/new-mercedes-gla-revealed-audi-q4-rival-408-mile-range" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">80</div>
        <div class="article-thumb"><img src="https://images.cdn.autocar.co.uk/sites/autocar.co.uk/files/styles/car_review_image_190/public/images/car-reviews/first-drives/legacy/wc-small-electric-triple-2025-me-70.jpg?itok=ejWOQ2GL" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/electric-cars/evs-and-hybrids-drive-uk-car-market-best-july-covid" target="_blank" rel="noopener">EVs and hybrids power UK to best July since Covid</a>
          <div class="article-take">Electrified models top half of registrations as grant support and discounts pull buyers into plug‑ins.</div>
          <div class="article-tags">
            <span class="chip">UK</span><span class="chip">EV</span><span class="chip">Hybrid</span><span class="chip">Market</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 5, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/electric-cars/evs-and-hybrids-drive-uk-car-market-best-july-covid" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">82</div>
        <div class="article-thumb"><img src="https://electrek.co/wp-content/uploads/sites/3/2026/07/Volvo-Lidar.webp?w=1600" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Volvo drops lidar on EX90/ES90, pays owners compensation</a>
          <div class="article-take">Volvo pivots away from its planned lidar stack, signaling a recalibration of its ADAS sensor roadmap.</div>
          <div class="article-tags">
            <span class="chip">Volvo</span><span class="chip">ADAS</span><span class="chip">Lidar</span><span class="chip">Suppliers</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">78</div>
        <div class="article-thumb"><img src="https://www.caranddriver.com/_assets/design-tokens/og-image.jpg" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://www.caranddriver.com/news/a73319471/ram-1500-seatbelt-buckle-one-million-truck-recall/" target="_blank" rel="noopener">Ram recalls ~1.3M 1500 pickups for rear seat belt anchors</a>
          <div class="article-take">FCA’s latest large‑scale recall adds pressure on quality and dealer throughput during peak sales.</div>
          <div class="article-tags">
            <span class="chip">Ram</span><span class="chip">Recall</span><span class="chip">Safety</span>
          </div>
        </div>
        <div class="article-source">
          <span>Car and Driver — Aug 4, 2026</span>
          <a href="https://www.caranddriver.com/news/a73319471/ram-1500-seatbelt-buckle-one-million-truck-recall/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">75</div>
        <div class="article-thumb"><img src="https://images.cdn.autocar.co.uk/sites/autocar.co.uk/files/styles/car_review_image_190/public/images/car-reviews/first-drives/legacy/robotaxi_87_0.jpg?itok=nITjPgOL" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/business-corporate/cheap-cars-hit-tesla-profits-tech-pivot-stalls" target="_blank" rel="noopener">Cheaper models hit Tesla margins as tech pivot slows</a>
          <div class="article-take">Price cuts and lower ASPs lifted deliveries but squeezed profits, underscoring reliance on 3/Y.</div>
          <div class="article-tags">
            <span class="chip">Tesla</span><span class="chip">Finance</span><span class="chip">Strategy</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 5, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/business-corporate/cheap-cars-hit-tesla-profits-tech-pivot-stalls" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">70</div>
        <div class="article-thumb"><img src="https://electrek.co/wp-content/uploads/sites/3/2026/08/Kia-PV5-EV-van-sales.jpeg?quality=82&strip=all&w=1400" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/05/kia-pv5-captures-37-europes-small-ev-van-market/" target="_blank" rel="noopener">Kia PV5 grabs 37% share of small EV van sales in Europe/UK</a>
          <div class="article-take">Fleet‑first packaging and pricing help Kia’s first e‑LCV quickly dominate a key segment.</div>
          <div class="article-tags">
            <span class="chip">Kia</span><span class="chip">Fleet</span><span class="chip">EV</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 5, 2026</span>
          <a href="https://electrek.co/2026/08/05/kia-pv5-captures-37-europes-small-ev-van-market/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">74</div>
        <div class="article-thumb"><img src="https://images.cdn.autocar.co.uk/sites/autocar.co.uk/files/styles/car_review_image_190/public/images/car-reviews/first-drives/legacy/bmw-ix3-2026-mg-131.jpg?itok=3ft8M8or" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">BMW puts G‑Class rival on hold amid shifting demand</a>
          <div class="article-take">A fast‑evolving China market and trade barriers force BMW to reprioritize model investments.</div>
          <div class="article-tags">
            <span class="chip">BMW</span><span class="chip">Manufacturing</span><span class="chip">Strategy</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 5, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">69</div>
        <div class="article-thumb"><img src="https://electrek.co/wp-content/uploads/sites/3/2025/09/Mercedes-solid-state-EV-batteries-1.jpeg?quality=82&strip=all&w=1400" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">SK On and Factorial team up to scale solid‑state batteries</a>
          <div class="article-take">A new alliance aims to push solid‑state cells from pilot lines to mass‑market EVs.</div>
          <div class="article-tags">
            <span class="chip">Battery</span><span class="chip">Suppliers</span><span class="chip">Technology</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">68</div>
        <div class="article-thumb"><img src="https://electrek.co/wp-content/uploads/sites/3/2026/08/wynwood-village-station-press-release-2.jpg?quality=82&strip=all&w=1200" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/04/evgo-is-putting-500-fast-chargers-where-americans-shop/" target="_blank" rel="noopener">EVgo adding 500+ fast chargers at shopping centers</a>
          <div class="article-take">Retail‑adjacent DCFC expands dwell‑time monetization and improves charging convenience.</div>
          <div class="article-tags">
            <span class="chip">Charging</span><span class="chip">EVgo</span><span class="chip">Retail</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 4, 2026</span>
          <a href="https://electrek.co/2026/08/04/evgo-is-putting-500-fast-chargers-where-americans-shop/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">66</div>
        <div class="article-thumb"><img src="https://www.caranddriver.com/_assets/design-tokens/og-image.jpg" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://www.caranddriver.com/news/a73337003/hyundai-kia-genesis-record-sales-july-2026/" target="_blank" rel="noopener">Hyundai, Kia, Genesis all hit record July sales</a>
          <div class="article-take">Strong hybrid mix offset softer EV demand, keeping Korea’s majors on a growth streak.</div>
          <div class="article-tags">
            <span class="chip">Hyundai</span><span class="chip">Kia</span><span class="chip">Hybrid</span><span class="chip">Sales</span>
          </div>
        </div>
        <div class="article-source">
          <span>Car and Driver — Aug 5, 2026</span>
          <a href="https://www.caranddriver.com/news/a73337003/hyundai-kia-genesis-record-sales-july-2026/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">65</div>
        <div class="article-thumb"><img src="https://www.electrive.com/media/2025/05/volkswagen-id7-tourer-pro-s-fahrbericht-daniel-boennighausen-ladestation-charging-station-ccs-2025-01-min-400x267.jpg" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/05/norways-ev-share-rises-to-97-6-in-july/" target="_blank" rel="noopener">Norway’s BEV share hits 97.6% in July</a>
          <div class="article-take">Norway’s near‑total electrification underscores how policy and product can transform a market.</div>
          <div class="article-tags">
            <span class="chip">Norway</span><span class="chip">EV</span><span class="chip">Government</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrive — Aug 5, 2026</span>
          <a href="https://www.electrive.com/2026/08/05/norways-ev-share-rises-to-97-6-in-july/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">64</div>
        <div class="article-thumb"><img src="https://images.hgmsites.net/tmb/pilot-gm-and-evgo-build-out-ev-fast-charging-network_100964176_t.gif" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://www.greencarreports.com/news/1146051_gm-pilot-ev-charging-network-now-spans-over-25-states" target="_blank" rel="noopener">GM–Pilot EV charging network now spans 25+ states</a>
          <div class="article-take">The Pilot/Flying J build‑out extends corridor fast charging across key freight and travel routes.</div>
          <div class="article-tags">
            <span class="chip">GM</span><span class="chip">EVgo</span><span class="chip">Charging</span>
          </div>
        </div>
        <div class="article-source">
          <span>Green Car Reports — Aug 5, 2026</span>
          <a href="https://www.greencarreports.com/news/1146051_gm-pilot-ev-charging-network-now-spans-over-25-states" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">62</div>
        <div class="article-thumb"><img src="https://images.cdn.autocar.co.uk/sites/autocar.co.uk/files/styles/car_review_image_190/public/images/car-reviews/first-drives/legacy/electric-cars-005.jpg?itok=Vmki5k7J" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/company-cars/used-ev-repair-scheme-looks-tackle-cliff-edge-residual-drops" target="_blank" rel="noopener">New battery repair hub targets used‑EV value cliff</a>
          <div class="article-take">BCA’s Doncaster site offers OEM‑standard high‑voltage diagnostics and repairs to de‑risk ex‑fleet EVs.</div>
          <div class="article-tags">
            <span class="chip">Used Cars</span><span class="chip">Battery</span><span class="chip">Residuals</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 5, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/company-cars/used-ev-repair-scheme-looks-tackle-cliff-edge-residual-drops" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">61</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/05/india-approves-chargers-awaits-deployment/" target="_blank" rel="noopener">India approves 6,562 public EV chargers; deployment lags</a>
          <div class="article-take">Policy momentum is strong, but execution remains the bottleneck for India’s public charging rollout.</div>
          <div class="article-tags">
            <span class="chip">India</span><span class="chip">Charging</span><span class="chip">Government</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrive — Aug 5, 2026</span>
          <a href="https://www.electrive.com/2026/08/05/india-approves-chargers-awaits-deployment/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/business-manufacturing/chinese-car-makers-all-share-parts-will-world-follow" target="_blank" rel="noopener">How China’s shared parts cut costs—and change the game</a>
          <div class="article-take">Standardized tooling across brands accelerates launches and squeezes cost out of non‑differentiators.</div>
          <div class="article-tags">
            <span class="chip">China</span><span class="chip">Supply Chain</span><span class="chip">Manufacturing</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 5, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/business-manufacturing/chinese-car-makers-all-share-parts-will-world-follow" target="_blank" rel="noopener">Read original →</a>
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
    <h2 class="section-title">Industry News <span class="count">Top developments</span></h2>
    <div class="article-table">
      
      <div class="article-row">
        <div class="score-chip high">92</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">NHTSA probes 1.2M Tesla Model 3/Y over suspension failures</a>
          <div class="article-take">A high‑volume safety investigation could trigger repairs, costs and brand risk for Tesla.</div>
          <div class="article-tags"><span class="chip">Safety</span><span class="chip">Government</span><span class="chip">Tesla</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 31, 2026</span>
          <a href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">80</div>
        <div class="article-thumb"><img src="https://images.cdn.autocar.co.uk/sites/autocar.co.uk/files/styles/car_review_image_190/public/images/car-reviews/first-drives/legacy/wc-small-electric-triple-2025-me-70.jpg?itok=ejWOQ2GL" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/electric-cars/evs-and-hybrids-drive-uk-car-market-best-july-covid" target="_blank" rel="noopener">EVs and hybrids power UK to best July since Covid</a>
          <div class="article-take">Plug‑in demand accelerates despite ZEV target pressure and price debates.</div>
          <div class="article-tags"><span class="chip">Market</span><span class="chip">UK</span><span class="chip">EV</span></div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 5, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/electric-cars/evs-and-hybrids-drive-uk-car-market-best-july-covid" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">74</div>
        <div class="article-thumb"><img src="https://images.cdn.autocar.co.uk/sites/autocar.co.uk/files/styles/car_review_image_190/public/images/car-reviews/first-drives/legacy/bmw-ix3-2026-mg-131.jpg?itok=3ft8M8or" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">BMW pauses hardcore off‑roader as strategy shifts</a>
          <div class="article-take">Macro volatility forces tighter portfolio discipline—even for halo projects.</div>
          <div class="article-tags"><span class="chip">Strategy</span><span class="chip">BMW</span></div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 5, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

    </div>
  </div>

  <div class="sec-group reveal" id="electric-vehicles">
    <h2 class="section-title">Electric Vehicles <span class="count">Product &amp; adoption</span></h2>
    <div class="article-table">
      
      <div class="article-row">
        <div class="score-chip high">88</div>
        <div class="article-thumb"><img src="https://images.cdn.autocar.co.uk/sites/autocar.co.uk/files/styles/car_review_image_190/public/images/car-reviews/first-drives/legacy/merceds-gla-2026-017.jpg?itok=IqCN5gha" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/electric-cars/new-mercedes-gla-revealed-audi-q4-rival-408-mile-range" target="_blank" rel="noopener">Mercedes unveils long‑range GLA EV</a>
          <div class="article-take">Efficient MMA hardware and 800V charging raise the bar for compact premium EVs.</div>
          <div class="article-tags"><span class="chip">EV</span><span class="chip">Mercedes-Benz</span></div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 5, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/electric-cars/new-mercedes-gla-revealed-audi-q4-rival-408-mile-range" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">70</div>
        <div class="article-thumb"><img src="https://electrek.co/wp-content/uploads/sites/3/2026/08/Kia-PV5-EV-van-sales.jpeg?quality=82&strip=all&w=1400" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/05/kia-pv5-captures-37-europes-small-ev-van-market/" target="_blank" rel="noopener">Kia PV5 becomes Europe’s top small e‑van</a>
          <div class="article-take">Rapid fleet uptake shows where near‑term EV economics already work.</div>
          <div class="article-tags"><span class="chip">Fleet</span><span class="chip">EV</span><span class="chip">Kia</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 5, 2026</span>
          <a href="https://electrek.co/2026/08/05/kia-pv5-captures-37-europes-small-ev-van-market/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">65</div>
        <div class="article-thumb"><img src="https://www.electrive.com/media/2025/05/volkswagen-id7-tourer-pro-s-fahrbericht-daniel-boennighausen-ladestation-charging-station-ccs-2025-01-min-400x267.jpg" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/05/norways-ev-share-rises-to-97-6-in-july/" target="_blank" rel="noopener">Norway posts 97.6% BEV share</a>
          <div class="article-take">An EV‑only market is no longer theoretical—it’s playing out in real time.</div>
          <div class="article-tags"><span class="chip">Norway</span><span class="chip">EV Adoption</span></div>
        </div>
        <div class="article-source">
          <span>Electrive — Aug 5, 2026</span>
          <a href="https://www.electrive.com/2026/08/05/norways-ev-share-rises-to-97-6-in-july/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

    </div>
  </div>

  <div class="sec-group reveal" id="manufacturers">
    <h2 class="section-title">Manufacturers <span class="count">Strategy &amp; models</span></h2>
    <div class="article-table">
      
      <div class="article-row">
        <div class="score-chip">74</div>
        <div class="article-thumb"><img src="https://images.cdn.autocar.co.uk/sites/autocar.co.uk/files/styles/car_review_image_190/public/images/car-reviews/first-drives/legacy/bmw-ix3-2026-mg-131.jpg?itok=3ft8M8or" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">BMW trims future portfolio amid market shifts</a>
          <div class="article-take">Resource focus moves to high‑volume EVs and core segments.</div>
          <div class="article-tags"><span class="chip">BMW</span><span class="chip">Strategy</span></div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 5, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">66</div>
        <div class="article-main">
          <a class="headline" href="https://www.caranddriver.com/news/a73337003/hyundai-kia-genesis-record-sales-july-2026/" target="_blank" rel="noopener">Hyundai/Kia extend record run on hybrid strength</a>
          <div class="article-take">Powertrain diversity is paying off as the EV market normalizes.</div>
          <div class="article-tags"><span class="chip">Hyundai</span><span class="chip">Kia</span><span class="chip">Sales</span></div>
        </div>
        <div class="article-source">
          <span>Car and Driver — Aug 5, 2026</span>
          <a href="https://www.caranddriver.com/news/a73337003/hyundai-kia-genesis-record-sales-july-2026/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

    </div>
  </div>

  <div class="sec-group reveal" id="dealers">
    <h2 class="section-title">Dealers <span class="count">Retail &amp; distribution</span></h2>
    <div class="article-table">
      
      <div class="article-row">
        <div class="score-chip">62</div>
        <div class="article-thumb"><img src="https://images.cdn.autocar.co.uk/sites/autocar.co.uk/files/styles/car_review_image_190/public/images/car-reviews/first-drives/legacy/electric-cars-005.jpg?itok=Vmki5k7J" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/company-cars/used-ev-repair-scheme-looks-tackle-cliff-edge-residual-drops" target="_blank" rel="noopener">BCA launches used‑EV battery repair program</a>
          <div class="article-take">Certified high‑voltage repairs and battery health reports aim to restore dealer confidence.</div>
          <div class="article-tags"><span class="chip">Used EVs</span><span class="chip">Auctions</span></div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 5, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/company-cars/used-ev-repair-scheme-looks-tackle-cliff-edge-residual-drops" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">58</div>
        <div class="article-main">
          <a class="headline" href="https://www.motor1.com/news/803722/costco-infiniti-discount/" target="_blank" rel="noopener">Costco adds fresh discounts on new Infiniti SUVs</a>
          <div class="article-take">Wholesale partnerships remain an important new‑vehicle lead generator for dealers.</div>
          <div class="article-tags"><span class="chip">Retail</span><span class="chip">Incentives</span></div>
        </div>
        <div class="article-source">
          <span>Motor1 — Aug 5, 2026</span>
          <a href="https://www.motor1.com/news/803722/costco-infiniti-discount/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

    </div>
  </div>

  <div class="sec-group reveal" id="suppliers">
    <h2 class="section-title">Suppliers <span class="count">Batteries &amp; charging</span></h2>
    <div class="article-table">
      
      <div class="article-row">
        <div class="score-chip">69</div>
        <div class="article-thumb"><img src="https://electrek.co/wp-content/uploads/sites/3/2025/09/Mercedes-solid-state-EV-batteries-1.jpeg?quality=82&strip=all&w=1400" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">SK On &amp; Factorial align on solid‑state scaling</a>
          <div class="article-take">A bid to industrialize next‑gen cells beyond lab demos and pilot runs.</div>
          <div class="article-tags"><span class="chip">Battery</span><span class="chip">Suppliers</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">68</div>
        <div class="article-thumb"><img src="https://electrek.co/wp-content/uploads/sites/3/2026/08/wynwood-village-station-press-release-2.jpg?quality=82&strip=all&w=1200" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/04/evgo-is-putting-500-fast-chargers-where-americans-shop/" target="_blank" rel="noopener">EVgo to deploy 500+ DCFC at shopping centers</a>
          <div class="article-take">Retail hosts unlock scale and better charging experiences in daily life.</div>
          <div class="article-tags"><span class="chip">Charging</span><span class="chip">EVgo</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 4, 2026</span>
          <a href="https://electrek.co/2026/08/04/evgo-is-putting-500-fast-chargers-where-americans-shop/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">60</div>
        <div class="article-thumb"><img src="https://www.electrive.com/media/2026/08/kempower-dll-bedfordshire-charging-stations-dc-hpc-uk-400x267.jpeg" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/05/kempower-launches-ev-charger-leasing-model-in-the-uk/" target="_blank" rel="noopener">Kempower launches leasing for UK HPC sites</a>
          <div class="article-take">Capex‑light models could open the door for independent CPOs.</div>
          <div class="article-tags"><span class="chip">Charging</span><span class="chip">Finance</span></div>
        </div>
        <div class="article-source">
          <span>Electrive — Aug 5, 2026</span>
          <a href="https://www.electrive.com/2026/08/05/kempower-launches-ev-charger-leasing-model-in-the-uk/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

    </div>
  </div>

  <div class="sec-group reveal" id="government">
    <h2 class="section-title">Government <span class="count">Policy &amp; regulation</span></h2>
    <div class="article-table">
      
      <div class="article-row">
        <div class="score-chip high">92</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">US launches Tesla suspension probe</a>
          <div class="article-take">The investigation could progress from evaluation to recall, depending on findings.</div>
          <div class="article-tags"><span class="chip">NHTSA</span><span class="chip">Safety</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 31, 2026</span>
          <a href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      
      <div class="article-row">
        <div class="score-chip">61</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/05/india-approves-chargers-awaits-deployment/" target="_blank" rel="noopener">India approves 6,562 chargers; installs pending</a>
          <div class="article-take">Funding and permits are in place; execution is now the critical path.</div>
          <div class="article-tags"><span class="chip">India</span><span class="chip">Charging</span></div>
        </div>
        <div class="article-source">
          <span>Electrive — Aug 5, 2026</span>
          <a href="https://www.electrive.com/2026/08/05/india-approves-chargers-awaits-deployment/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

    </div>
  </div>

  <div class="sec-group reveal" id="technology">
    <h2 class="section-title">Technology <span class="count">Batteries &amp; software</span></h2>
    <div class="article-table">
      
      <div class="article-row">
        <div class="score-chip">82</div>
        <div class="article-thumb"><img src="https://electrek.co/wp-content/uploads/sites/3/2026/07/Volvo-Lidar.webp?w=1600" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Volvo exits lidar for EX90/ES90</a>
        <div class="article-take">A major OEM vote on sensor cost/benefit reshapes supplier dynamics.</div>
          <div class="article-tags"><span class="chip">ADAS</span><span class="chip">Sensors</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      
      <div class="article-row">
        <div class="score-chip">69</div>
        <div class="article-thumb"><img src="https://electrek.co/wp-content/uploads/sites/3/2025/09/Mercedes-solid-state-EV-batteries-1.jpeg?quality=82&strip=all&w=1400" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">Solid‑state push gains new backers</a>
          <div class="article-take">Partnerships focus on manufacturability, not just energy density milestones.</div>
          <div class="article-tags"><span class="chip">Battery</span><span class="chip">R&amp;D</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

    </div>
  </div>

  <div class="sec-group reveal" id="finance">
    <h2 class="section-title">Finance <span class="count">Earnings &amp; markets</span></h2>
    <div class="article-table">
      
      <div class="article-row">
        <div class="score-chip">75</div>
        <div class="article-thumb"><img src="https://images.cdn.autocar.co.uk/sites/autocar.co.uk/files/styles/car_review_image_190/public/images/car-reviews/first-drives/legacy/robotaxi_87_0.jpg?itok=nITjPgOL" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/business-corporate/cheap-cars-hit-tesla-profits-tech-pivot-stalls" target="_blank" rel="noopener">Tesla profits slump despite volume growth</a>
          <div class="article-take">Falling ASPs and higher incentives dent margins as competition intensifies.</div>
          <div class="article-tags"><span class="chip">Earnings</span><span class="chip">Tesla</span></div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 5, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/business-corporate/cheap-cars-hit-tesla-profits-tech-pivot-stalls" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      
      <div class="article-row">
        <div class="score-chip">58</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/05/lucid-postpones-mid-size-ev-launch-to-2027/" target="_blank" rel="noopener">Lucid delays mid‑size “Cosmos” to 2027</a>
          <div class="article-take">Cash conservation and execution reset push the mainstream entry out a year.</div>
          <div class="article-tags"><span class="chip">Lucid</span><span class="chip">Delays</span></div>
        </div>
        <div class="article-source">
          <span>Electrive — Aug 5, 2026</span>
          <a href="https://www.electrive.com/2026/08/05/lucid-postpones-mid-size-ev-launch-to-2027/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

    </div>
  </div>

  <div class="sec-group reveal" id="international">
    <h2 class="section-title">International <span class="count">Global markets</span></h2>
    <div class="article-table">
      
      <div class="article-row">
        <div class="score-chip">72</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/business-manufacturing/chinese-car-makers-all-share-parts-will-world-follow" target="_blank" rel="noopener">China’s shared‑parts model challenges incumbents</a>
          <div class="article-take">Industry‑wide commoditization of non‑visible components compresses cost and time‑to‑market.</div>
          <div class="article-tags"><span class="chip">China</span><span class="chip">Supply Chain</span></div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 5, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/business-manufacturing/chinese-car-makers-all-share-parts-will-world-follow" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      
      <div class="article-row">
        <div class="score-chip">67</div>
        <div class="article-thumb"><img src="https://electrek.co/wp-content/uploads/sites/3/2026/08/BYD-Denza-Z9S-pre-orders.jpeg?quality=82&strip=all&w=1400" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/03/byd-opens-denza-z9s-pre-orders-record-1100-km-ev-range/" target="_blank" rel="noopener">BYD’s Denza Z9S claims 1,100 km range; pre‑orders open</a>
          <div class="article-take">China’s premium EV push continues with long‑range flagships at aggressive prices.</div>
          <div class="article-tags"><span class="chip">BYD</span><span class="chip">China</span><span class="chip">EV</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 3, 2026</span>
          <a href="https://electrek.co/2026/08/03/byd-opens-denza-z9s-pre-orders-record-1100-km-ev-range/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

    </div>
  </div>

  <div class="sec-group reveal" id="opinion">
    <h2 class="section-title">Opinion <span class="count">Analysis &amp; commentary</span></h2>
    <div class="article-table">
      
      <div class="article-row">
        <div class="score-chip">60</div>
        <div class="article-thumb"><img src="https://images.cdn.autocar.co.uk/sites/autocar.co.uk/files/styles/car_review_image_190/public/images/car-reviews/first-drives/legacy/jaecoo-j7-rt-2025-review-front-corner-blur-42.jpg?itok=WnSjKcye" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/opinion/new-cars/who-china-really-stealing-sales" target="_blank" rel="noopener">Who is China really stealing sales from?</a>
          <div class="article-take">Mid‑market stalwarts, not entry‑level brands, are feeling the brunt of China’s value EV surge.</div>
          <div class="article-tags"><span class="chip">China</span><span class="chip">Competition</span></div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 5, 2026</span>
          <a href="https://www.autocar.co.uk/opinion/new-cars/who-china-really-stealing-sales" target="_blank" rel="noopener">Read original →</a>
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