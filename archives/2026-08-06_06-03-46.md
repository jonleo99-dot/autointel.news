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
    <span class="ticker-item"><b>Volvo</b> drops lidar on EX90/ES90 <span class="ticker-up">▲</span></span>
    <span class="ticker-item"><b>Tesla</b> Q2 margins under pressure <span class="ticker-down">▼</span></span>
    <span class="ticker-item"><b>BMW</b> iX3 orders surge to ~100k <span class="ticker-up">▲</span></span>
    <span class="ticker-item"><b>Lucid</b> delays Cosmos to 2027 <span class="ticker-down">▼</span></span>
    <span class="ticker-item"><b>UK EV Market</b> best July since 2019 <span class="ticker-up">▲</span></span>
    <span class="ticker-item"><b>Solid‑state batteries</b> SK On + Factorial alliance <span class="ticker-up">▲</span></span>
    <span class="ticker-item"><b>Robotaxi</b> Waymo UI refresh & Gemini <span class="ticker-up">▲</span></span>
    <span class="ticker-item"><b>Charging</b> EVgo adds 500+ retail fast stalls <span class="ticker-up">▲</span></span>
    <span class="ticker-item"><b>Recalls</b> Ram 1500 seat belt anchors <span class="ticker-down">▼</span></span>
    <span class="ticker-item"><b>BYD</b> Denza D9 launches in UK <span class="ticker-up">▲</span></span>
    <!-- repeat: <span class="ticker-item">{{TICKER_ICON}}<b>{{NAME}}</b> {{LABEL}} <span class="ticker-up|ticker-down|ticker-flat">▲|▼|■</span></span> -->
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
    <!-- {{FEATURED_IMAGE}}: 800x450 hero image URL. Omit the whole
         .hero-media block (not just the img) if no image was generated
         for this article, so hero-grid's own rounded corners apply. -->
    <div class="hero-media">
      <img src="https://electrek.co/wp-content/uploads/sites/3/2026/07/Volvo-Lidar.webp?w=1600" alt="Volvo drops lidar for good on EX90 and ES90, pays owner compensation" width="800" height="450" loading="lazy">
    </div>
    <div class="hero-grid">
      <div class="hero-main">
        <h1>Volvo drops lidar for good on EX90 and ES90, pays owner compensation</h1>
        <p class="dek">Volvo confirmed it will remove lidar hardware from the EX90 and ES90 and compensate owners in markets like Norway after ending its supplier relationship with Luminar.</p>

        <div class="source-strip">
          <span>Source: <b>Electrek</b></span>
          <span>Aug 5, 2026</span>
          <a href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Read original →</a>
        </div>

        <div class="entity-grid">
          <div class="entity-field">
            <span class="ef-label">Manufacturers</span>
            <div class="chip-row">
              <span class="chip entity-mfr">Volvo Cars</span>
            </div>
          </div>
          <div class="entity-field">
            <span class="ef-label">Suppliers</span>
            <!-- repeat: <span class="chip">{{ENTITY_ICON}}{{NAME}}</span> -->
            <div class="chip-row"><span class="chip">Luminar Technologies</span></div>
          </div>
          <div class="entity-field">
            <span class="ef-label">Countries</span>
            <!-- repeat: <span class="chip">{{ENTITY_ICON}}{{NAME}}</span> (flag glyph) -->
            <div class="chip-row"><span class="chip">Norway</span><span class="chip">Sweden</span></div>
          </div>
          <div class="entity-field">
            <span class="ef-label">Government Agencies</span>
            <div class="chip-row">
              
              <!-- repeat: <span class="chip entity-gov">{{ENTITY_ICON}}{{NAME}}</span> -->
            </div>
          </div>
          <div class="entity-field">
            <span class="ef-label">Public Companies</span>
            <div class="chip-row">
              <span class="chip stock down"><span class="tk">VOLCAR-B.ST</span><span class="chg">■</span></span>
              <span class="chip stock down"><span class="tk">LAZR</span><span class="chg">▼</span></span>
              <!-- repeat: <span class="chip stock up|down">{{ENTITY_ICON}}<span class="tk">{{TICKER}}</span><span class="chg">{{CHANGE}}</span></span> -->
            </div>
          </div>
          <div class="entity-field">
            <span class="ef-label">Topics</span>
            <!-- repeat: <span class="chip">{{TOPIC_ICON}}{{NAME}}</span> -->
            <!-- {{TOPIC_ICON}}: complete pre-classed 16x16 icon element
                 (class="chip-icon") for this topic — same convention and
                 drop-entirely-if-missing rule as {{ENTITY_ICON}}. -->
            <div class="chip-row"><span class="chip">ADAS</span><span class="chip">Lidar</span><span class="chip">Safety</span><span class="chip">Autonomous</span><span class="chip">Software</span></div>
          </div>
          <div class="entity-field wide">
            <span class="ef-label">Related Stories</span>
            <ul class="data-list">
              <li><a href="https://electrek.co/2026/08/04/waymo-co-ceo-camera-only-self-driving-tesla/" target="_blank" rel="noopener">Waymo CEO explains why camera‑only self‑driving falls short</a></li>
              <li><a href="https://electrek.co/2026/07/29/waymo-gemini-ai-ojai-robotaxi-redesigned-interface/" target="_blank" rel="noopener">Waymo adds Gemini AI assistant and new UI to Ojai robotaxi</a></li>
              <li><a href="https://electrek.co/2026/08/05/evgo-is-putting-500-fast-chargers-where-americans-shop/" target="_blank" rel="noopener">EVgo is putting 500+ fast chargers where Americans shop</a></li>
              <li><a href="https://electrek.co/2026/08/05/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Volvo confirms lidar removal and compensation details</a></li>
            </ul>
          </div>
          <div class="entity-field wide">
            <span class="ef-label">Timeline</span>
            <ul class="timeline-list">
              <li><span class="t-date mono">Aug 2026</span><span>Volvo confirms EX90/ES90 will not ship with lidar; owners in Norway receive NOK 18,000 compensation.</span></li>
              <li><span class="t-date mono">Early 2026</span><span>Volvo ends lidar supplier relationship with Luminar.</span></li>
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
    <h2 class="section-title">Industry Snapshot <span class="count">Week of Aug 5, 2026</span></h2>
    <div class="dash-grid">
      <div class="stat-panel">
        <h4>Top Manufacturers (by mention)</h4>
        <ul class="rank-list">
          <li><span>Tesla</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:100%"></span></span><span class="rank-count">28</span></li>
          <li><span>BYD</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:82%"></span></span><span class="rank-count">23</span></li>
          <li><span>BMW</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:70%"></span></span><span class="rank-count">20</span></li>
          <li><span>Hyundai/Kia</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:68%"></span></span><span class="rank-count">19</span></li>
          <li><span>Volvo</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:61%"></span></span><span class="rank-count">17</span></li>
        </ul>
      </div>
      <div class="stat-panel">
        <h4>Top Suppliers & Tech Firms</h4>
        <ul class="rank-list">
          <li><span>EVgo</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:100%"></span></span><span class="rank-count">12</span></li>
          <li><span>Luminar</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:83%"></span></span><span class="rank-count">10</span></li>
          <li><span>SK On</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:58%"></span></span><span class="rank-count">7</span></li>
          <li><span>Factorial</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:50%"></span></span><span class="rank-count">6</span></li>
          <li><span>Ørsted</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:42%"></span></span><span class="rank-count">5</span></li>
        </ul>
      </div>
      <div class="stat-panel">
        <h4>Trending Topics</h4>
        <div class="tagcloud">
          <span class="chip lg">Lidar</span>
          <span class="chip lg">Robotaxis</span>
          <span class="chip">Solid‑state batteries</span>
          <span class="chip">EV Charging</span>
          <span class="chip">ZEV Mandate</span>
          <span class="chip">Recalls</span>
          <span class="chip">LFP Chemistry</span>
          <span class="chip">Tariffs & Trade</span>
        </div>
      </div>
      <div class="stat-panel">
        <h4>Government & Policy</h4>
        <ul class="rank-list">
          <li><span>UK ZEV targets</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:100%"></span></span><span class="rank-count">8</span></li>
          <li><span>FCC inverter rules</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:75%"></span></span><span class="rank-count">6</span></li>
          <li><span>EU battery standards</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:50%"></span></span><span class="rank-count">4</span></li>
        </ul>
      </div>
      <div class="stat-panel">
        <h4>Financial Moves</h4>
        <ul class="rank-list">
          <li><span>Tesla profits/margins</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:100%"></span></span><span class="rank-count">9</span></li>
          <li><span>Lucid delay/reset</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:78%"></span></span><span class="rank-count">7</span></li>
          <li><span>BMW product review</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:67%"></span></span><span class="rank-count">6</span></li>
          <li><span>GM–SAIC JV extension</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:56%"></span></span><span class="rank-count">5</span></li>
        </ul>
      </div>
      <div class="stat-panel">
        <h4>Global Regions</h4>
        <ul class="rank-list">
          <li><span>Europe (UK, Nordics)</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:100%"></span></span><span class="rank-count">24</span></li>
          <li><span>China</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:79%"></span></span><span class="rank-count">19</span></li>
          <li><span>North America</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:75%"></span></span><span class="rank-count">18</span></li>
          <li><span>UK & Ireland</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:67%"></span></span><span class="rank-count">16</span></li>
        </ul>
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
        <a href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Volvo abandons lidar on EX90/ES90</a>
        <div class="fp-meta"><span>Impact: High</span><span>Aug 5, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/08/05/uk-records-strongest-ev-july-to-date/" target="_blank" rel="noopener">UK EV share sets July record</a>
        <div class="fp-meta"><span>Impact: Medium</span><span>Aug 5, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/30/bmw-puts-g-class-rival-hold-china-headwinds-hit-home/" target="_blank" rel="noopener">BMW puts G‑Class rival on hold amid China headwinds</a>
        <div class="fp-meta"><span>Impact: Medium</span><span>Jul 30, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/28/bmw-ramps-up-ix3-output-orders-near-100000/" target="_blank" rel="noopener">BMW ramps up iX3 output as orders near 100k</a>
        <div class="fp-meta"><span>Impact: Medium</span><span>Jul 28, 2026</span></div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Technology</h3>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">SK On & Factorial ally on solid‑state batteries</a>
        <div class="fp-meta"><span>Impact: High</span><span>Jul 29, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/waymo-gemini-ai-ojai-robotaxi-redesigned-interface/" target="_blank" rel="noopener">Waymo integrates Gemini AI, new rider UI</a>
        <div class="fp-meta"><span>Impact: Medium</span><span>Jul 29, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/08/05/evgo-is-putting-500-fast-chargers-where-americans-shop/" target="_blank" rel="noopener">EVgo to add 500+ fast chargers at shopping centers</a>
        <div class="fp-meta"><span>Impact: Medium</span><span>Aug 4, 2026</span></div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Government & Policy</h3>
      <div class="fp-row">
        <a href="https://www.autocar.co.uk/car-news/electric-cars/evs-and-hybrids-drive-uk-car-market-best-july-covid" target="_blank" rel="noopener">UK EV/hybrid surge lifts best July since Covid</a>
        <div class="fp-meta"><span>Impact: High</span><span>Aug 5, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/08/05/fcc-bans-foreign-made-connected-solar-inverters/" target="_blank" rel="noopener">FCC moves against foreign connected inverters</a>
        <div class="fp-meta"><span>Impact: Medium</span><span>Aug 5, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/08/05/new-york-city-to-install-600-additional-curbside-charging-points/" target="_blank" rel="noopener">NYC to install 600 curbside charging points</a>
        <div class="fp-meta"><span>Impact: Medium</span><span>Aug 5, 2026</span></div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Suppliers & Energy</h3>
      <div class="fp-row">
        <a href="https://electrek.co/2026/08/05/tesla-megapack-power-orsted-big-new-texas-grid-battery/" target="_blank" rel="noopener">Tesla Megapacks power new 500 MWh Texas BESS</a>
        <div class="fp-meta"><span>Impact: Medium</span><span>Aug 5, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/28/tesla-buys-texas-solar-farm-output-zelestra/" target="_blank" rel="noopener">Tesla signs PPA for entire 140 MW Texas solar farm</a>
        <div class="fp-meta"><span>Impact: Medium</span><span>Jul 28, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://chargedevs.com/newswire/beam-global-supplies-ev-arc-off-grid-charging-systems-for-dallas-municipal-fleet-and-massachusetts-carshare-pilot/" target="_blank" rel="noopener">Beam Global deploys off‑grid chargers in Dallas & MA</a>
        <div class="fp-meta"><span>Impact: Low</span><span>Aug 1, 2026</span></div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Trending Topics</h3>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Lidar strategy pivots</a>
        <div class="fp-meta"><span>Heat: High</span><span>Aug 5, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/waymo-gemini-ai-ojai-robotaxi-redesigned-interface/" target="_blank" rel="noopener">Robotaxi UX & AI copilots</a>
        <div class="fp-meta"><span>Heat: Medium</span><span>Jul 29, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/08/05/evgo-is-putting-500-fast-chargers-where-americans-shop/" target="_blank" rel="noopener">Retail‑anchored fast charging</a>
        <div class="fp-meta"><span>Heat: Medium</span><span>Aug 4, 2026</span></div>
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
    <h2 class="section-title">Latest Articles <span class="count">16 analyzed today</span></h2>
    <div class="article-table">
      
      <div class="article-row">
        <div class="score-chip high">90</div>
        <div class="article-thumb"><img src="https://electrek.co/wp-content/uploads/sites/3/2026/07/Volvo-Lidar.webp?w=1600" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Volvo drops lidar for good on EX90 and ES90, pays compensation</a>
          <div class="article-take">A high‑profile OEM abandoning lidar signals a sharper focus on cost, software sensing, and market‑by‑market product consistency.</div>
          <div class="article-tags"><span class="chip">Volvo</span><span class="chip">Luminar</span><span class="chip">ADAS</span><span class="chip">Lidar</span><span class="chip">Safety</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 5, 2026</span>
          <a href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip high">88</div>
        <div class="article-thumb"><img src="https://images.cdn.autocar.co.uk/sites/autocar.co.uk/files/images/car-reviews/first-drives/legacy/wc-small-electric-triple-2025-me-70.jpg?itok=ejWOQ2GL" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/electric-cars/evs-and-hybrids-drive-uk-car-market-best-july-covid" target="_blank" rel="noopener">EVs and hybrids drive UK car market to best July since Covid</a>
          <div class="article-take">Electrified models lifted UK registrations as OEMs discount to hit ZEV targets, reshaping the fuel mix faster than expected.</div>
          <div class="article-tags"><span class="chip">UK</span><span class="chip">ZEV mandate</span><span class="chip">EV Sales</span><span class="chip">Hybrids</span></div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 5, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/electric-cars/evs-and-hybrids-drive-uk-car-market-best-july-covid" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">82</div>
        <div class="article-thumb"><img src="https://electrek.co/wp-content/uploads/sites/3/2026/08/wynwood-village-station-press-release-2.jpg?quality=82&strip=all&w=1200" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/04/evgo-is-putting-500-fast-chargers-where-americans-shop/" target="_blank" rel="noopener">EVgo is putting 500+ fast chargers where Americans shop</a>
          <div class="article-take">Retail‑anchored fast charging tightens the link between dwell time and spend while filling critical urban charging gaps.</div>
          <div class="article-tags"><span class="chip">EVgo</span><span class="chip">Charging</span><span class="chip">Retail</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 4, 2026</span>
          <a href="https://electrek.co/2026/08/04/evgo-is-putting-500-fast-chargers-where-americans-shop/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">80</div>
        <div class="article-thumb"><img src="https://electrek.co/wp-content/uploads/sites/3/2026/08/OLD-300-COD.jpg?quality=82&strip=all&w=1440" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/05/tesla-megapack-power-orsted-big-new-texas-grid-battery/" target="_blank" rel="noopener">Tesla Megapacks power Ørsted’s big new Texas grid battery</a>
          <div class="article-take">Another 250 MW/500 MWh of BESS in ERCOT highlights storage’s role in firming renewables and serving peak demand.</div>
          <div class="article-tags"><span class="chip">Tesla Energy</span><span class="chip">Ørsted</span><span class="chip">Grid Storage</span><span class="chip">Texas</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 5, 2026</span>
          <a href="https://electrek.co/2026/08/05/tesla-megapack-power-orsted-big-new-texas-grid-battery/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">79</div>
        <div class="article-thumb"><img src="https://images.cdn.autocar.co.uk/sites/autocar.co.uk/files/images/car-reviews/first-drives/legacy/denza-d9-002.jpg?itok=bz88ErQs" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/new-denza-d9-%C2%A375k-luxury-mpv-plug-hybrid-power" target="_blank" rel="noopener">New Denza D9 is a £75k luxury MPV with plug‑in hybrid power</a>
          <div class="article-take">BYD’s premium arm brings a high‑spec seven‑seater to the UK, undercutting established luxo‑MPVs while touting 130‑mile EV range.</div>
          <div class="article-tags"><span class="chip">BYD</span><span class="chip">Denza</span><span class="chip">PHEV</span><span class="chip">UK Launch</span></div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 5, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/new-denza-d9-%C2%A375k-luxury-mpv-plug-hybrid-power" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">78</div>
        <div class="article-thumb"><img src="https://electrek.co/wp-content/uploads/sites/3/2026/07/BMW-iX3-orders.jpeg?quality=82&strip=all&w=1400" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/28/bmw-ramps-up-ix3-output-orders-near-100000/" target="_blank" rel="noopener">BMW ramps up iX3 output as orders near 100,000</a>
          <div class="article-take">Demand is pulling Debrecen’s EV ramp ahead of plan, signaling traction for BMW’s Neue Klasse rollout.</div>
          <div class="article-tags"><span class="chip">BMW</span><span class="chip">iX3</span><span class="chip">Production</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 28, 2026</span>
          <a href="https://electrek.co/2026/07/28/bmw-ramps-up-ix3-output-orders-near-100000/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">77</div>
        <div class="article-thumb"><img src="https://electrek.co/wp-content/uploads/sites/3/2026/08/evgo-tesla-partnership-1920x1080-1.jpg?quality=82&strip=all&w=1600" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/05/evgo-branded-tesla-superchargers-are-coming/" target="_blank" rel="noopener">EVgo‑branded Superchargers are coming</a>
          <div class="article-take">Third‑party deployment of Tesla’s latest hardware accelerates NACS build‑out and vendor convergence.</div>
          <div class="article-tags"><span class="chip">EVgo</span><span class="chip">Tesla</span><span class="chip">NACS</span><span class="chip">Charging</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 5, 2026</span>
          <a href="https://electrek.co/2026/08/05/evgo-branded-tesla-superchargers-are-coming/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">76</div>
        <div class="article-thumb"><img src="https://electrek.co/wp-content/uploads/sites/3/2026/03/Lucid-first-midsize-EV-Cosmos.jpeg?quality=82&strip=all&w=1400" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/04/lucids-smaller-cosmos-suv-slated-for-2026-has-been-pushed-back-to-2027/" target="_blank" rel="noopener">Lucid’s mid‑size Cosmos delayed to 2027</a>
          <div class="article-take">The reset trades time for execution as Lucid seeks sustainable margins beyond halo models.</div>
          <div class="article-tags"><span class="chip">Lucid</span><span class="chip">Product Delay</span><span class="chip">SUV</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 4, 2026</span>
          <a href="https://electrek.co/2026/08/04/lucids-smaller-cosmos-suv-slated-for-2026-has-been-pushed-back-to-2027/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">74</div>
        <div class="article-thumb"><img src="https://electrek.co/wp-content/uploads/sites/3/2026/08/EV-market-share.jpeg?quality=82&strip=all&w=1400" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/477795/" target="_blank" rel="noopener">IEA: Global EV sales jump 35% in Q2; 50 countries set records</a>
          <div class="article-take">Q2 snapped a slow Q1 as incentives, new models and price cuts reignited demand worldwide.</div>
          <div class="article-tags"><span class="chip">IEA</span><span class="chip">EV Sales</span><span class="chip">Global</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/477795/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">72</div>
        <div class="article-thumb"><img src="https://electrek.co/wp-content/uploads/sites/3/2026/07/Hyundai-IONIQ-3-prices-Europe-1.jpeg?quality=82&strip=all&w=1400" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/hyundai-reveals-ioniq-3-prices-start-30000-interest-surges/" target="_blank" rel="noopener">Hyundai reveals IONIQ 3 around $30k; interest surges</a>
          <div class="article-take">A value‑priced hatch with >300 miles range could reset entry EV expectations in 2027.</div>
          <div class="article-tags"><span class="chip">Hyundai</span><span class="chip">IONIQ 3</span><span class="chip">Pricing</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/hyundai-reveals-ioniq-3-prices-start-30000-interest-surges/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">71</div>
        <div class="article-thumb"><img src="https://images.cdn.autocar.co.uk/sites/autocar.co.uk/files/images/car-reviews/first-drives/legacy/bmw-ix3-2026-mg-131.jpg?itok=3ft8M8or" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">BMW puts G‑Class rival on ice amid shifting demand</a>
          <div class="article-take">Munich re‑prioritizes capital as China softens, tariffs rise and market needs diverge by region.</div>
          <div class="article-tags"><span class="chip">BMW</span><span class="chip">Strategy</span><span class="chip">SUV</span></div>
        </div>
        <div class="article-source">
          <span>Autocar — Jul 30, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">69</div>
        <div class="article-thumb"><img src="https://electrek.co/wp-content/uploads/sites/3/2026/08/GM-Buick-NEVs-China.jpeg?quality=82&strip=all&w=1400" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/05/gm-buick-evs-china-overseas-suv/" target="_blank" rel="noopener">GM will export China‑built electric Buicks overseas</a>
          <div class="article-take">SAIC‑GM extends a 20‑year JV as it taps China capacity to seed Buick EVs in new markets.</div>
          <div class="article-tags"><span class="chip">GM</span><span class="chip">Buick</span><span class="chip">China</span><span class="chip">Exports</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 5, 2026</span>
          <a href="https://electrek.co/2026/08/05/gm-buick-evs-china-overseas-suv/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">67</div>
        <div class="article-thumb"><img src="https://electrek.co/wp-content/uploads/sites/3/2026/08/wc-small-electric-triple-2025-me-70.jpg?quality=82&strip=all&w=1400" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/05/uk-records-strongest-ev-july-to-date/" target="_blank" rel="noopener">UK records strongest EV July to date</a>
          <div class="article-take">Battery‑electric share hit fresh highs across cars and vans, but SMMT warns target slope remains steep.</div>
          <div class="article-tags"><span class="chip">UK</span><span class="chip">EV Share</span><span class="chip">SMMT</span></div>
        </div>
        <div class="article-source">
          <span>Electrive — Aug 5, 2026</span>
          <a href="https://www.electrive.com/2026/08/05/uk-records-strongest-ev-july-to-date/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">66</div>
        <div class="article-thumb"><img src="https://electrek.co/wp-content/uploads/sites/3/2026/08/Hyundai-vehicles-upgrade-Pleos.jpeg?quality=82&strip=all&w=1400" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/28/kias-vehicles-smart-upgrade-2027/" target="_blank" rel="noopener">Kia vehicles to gain new high‑tech infotainment from 2027</a>
          <div class="article-take">Hyundai’s new software stack rolls across the brand family, standardizing UX and connected features.</div>
          <div class="article-tags"><span class="chip">Kia</span><span class="chip">Infotainment</span><span class="chip">Software‑defined</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 28, 2026</span>
          <a href="https://electrek.co/2026/07/28/kias-vehicles-smart-upgrade-2027/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">64</div>
        <div class="article-thumb"><img src="https://electrek.co/wp-content/uploads/sites/3/2026/08/IMG_4135_00-e1785447573347.jpeg?quality=82&strip=all&w=1600" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/03/2026-tesla-model-y-rwd-review/" target="_blank" rel="noopener">2026 Tesla Model Y RWD review: entry trim, flagship software</a>
          <div class="article-take">Tesla’s base Model Y leans hard on UI, charging and ecosystem strengths over dynamic thrills.</div>
          <div class="article-tags"><span class="chip">Tesla</span><span class="chip">Model Y</span><span class="chip">Review</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 3, 2026</span>
          <a href="https://electrek.co/2026/08/03/2026-tesla-model-y-rwd-review/" target="_blank" rel="noopener">Read original →</a>
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
    <h2 class="section-title">Industry News <span class="count">Macro, policy and market moves</span></h2>
    <div class="article-table">
      
      <div class="article-row">
        <div class="score-chip high">88</div>
        <div class="article-thumb"><img src="https://images.cdn.autocar.co.uk/sites/autocar.co.uk/files/images/car-reviews/first-drives/legacy/wc-small-electric-triple-2025-me-70.jpg?itok=ejWOQ2GL" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/electric-cars/evs-and-hybrids-drive-uk-car-market-best-july-covid" target="_blank" rel="noopener">EVs and hybrids drive UK car market to best July since Covid</a>
          <div class="article-take">Electrified share jumps as incentives and pricing push buyers toward plug‑in options.</div>
          <div class="article-tags"><span class="chip">UK</span><span class="chip">EV Sales</span><span class="chip">Hybrids</span></div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 5, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/electric-cars/evs-and-hybrids-drive-uk-car-market-best-july-covid" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">74</div>
        <div class="article-thumb"><img src="https://electrek.co/wp-content/uploads/sites/3/2026/04/BYD-EVs-5-min-charging.jpeg?quality=82&strip=all&w=1400" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/477795/" target="_blank" rel="noopener">IEA: Global EV sales jump 35% in Q2; 50 countries set records</a>
          <div class="article-take">Momentum returns as markets normalize and model availability broadens.</div>
          <div class="article-tags"><span class="chip">IEA</span><span class="chip">Global EVs</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/477795/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

    </div>
  </div>

  <div class="sec-group reveal" id="electric-vehicles">
    <h2 class="section-title">Electric Vehicles <span class="count">Product and demand</span></h2>
    <div class="article-table">

      <div class="article-row">
        <div class="score-chip">78</div>
        <div class="article-thumb"><img src="https://electrek.co/wp-content/uploads/sites/3/2026/07/BMW-iX3-orders.jpeg?quality=82&strip=all&w=1400" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/28/bmw-ramps-up-ix3-output-orders-near-100000/" target="_blank" rel="noopener">BMW ramps up iX3 output as orders near 100,000</a>
          <div class="article-take">Scale builds confidence for Neue Klasse cadence across segments.</div>
          <div class="article-tags"><span class="chip">BMW</span><span class="chip">iX3</span><span class="chip">Production</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 28, 2026</span>
          <a href="https://electrek.co/2026/07/28/bmw-ramps-up-ix3-output-orders-near-100000/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      
      <div class="article-row">
        <div class="score-chip">72</div>
        <div class="article-thumb"><img src="https://electrek.co/wp-content/uploads/sites/3/2026/07/Hyundai-IONIQ-3-prices-Europe-1.jpeg?quality=82&strip=all&w=1400" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/hyundai-reveals-ioniq-3-prices-start-30000-interest-surges/" target="_blank" rel="noopener">Hyundai IONIQ 3 priced around $30k with long range</a>
          <div class="article-take">Affordable specs target the heart of mass EV adoption.</div>
          <div class="article-tags"><span class="chip">Hyundai</span><span class="chip">IONIQ 3</span><span class="chip">Value EVs</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/hyundai-reveals-ioniq-3-prices-start-30000-interest-surges/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">76</div>
        <div class="article-thumb"><img src="https://electrek.co/wp-content/uploads/sites/3/2026/03/Lucid-first-midsize-EV-Cosmos.jpeg?quality=82&strip=all&w=1400" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/04/lucids-smaller-cosmos-suv-slated-for-2026-has-been-pushed-back-to-2027/" target="_blank" rel="noopener">Lucid delays Cosmos mid‑size SUV to 2027</a>
          <div class="article-take">Execution and cost focus take precedence over speed to market.</div>
          <div class="article-tags"><span class="chip">Lucid</span><span class="chip">Mid‑size SUV</span><span class="chip">Delay</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 4, 2026</span>
          <a href="https://electrek.co/2026/08/04/lucids-smaller-cosmos-suv-slated-for-2026-has-been-pushed-back-to-2027/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

    </div>
  </div>

  <div class="sec-group reveal" id="manufacturers">
    <h2 class="section-title">Manufacturers <span class="count">Strategy and launches</span></h2>
    <div class="article-table">

      <div class="article-row">
        <div class="score-chip high">90</div>
        <div class="article-thumb"><img src="https://electrek.co/wp-content/uploads/sites/3/2026/07/Volvo-Lidar.webp?w=1600" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Volvo axes lidar on EX90/ES90</a>
          <div class="article-take">Hardware de‑contenting pairs with owner compensation to streamline trims.</div>
          <div class="article-tags"><span class="chip">Volvo</span><span class="chip">ADAS</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 5, 2026</span>
          <a href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      
      <div class="article-row">
        <div class="score-chip">71</div>
        <div class="article-thumb"><img src="https://images.cdn.autocar.co.uk/sites/autocar.co.uk/files/images/car-reviews/first-drives/legacy/bmw-ix3-2026-mg-131.jpg?itok=3ft8M8or" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">BMW pauses hardcore off‑roader plan</a>
          <div class="article-take">Capital shifts toward programs with clearer regional fit and faster ROI.</div>
          <div class="article-tags"><span class="chip">BMW</span><span class="chip">Portfolio</span></div>
        </div>
        <div class="article-source">
          <span>Autocar — Jul 30, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

    </div>
  </div>

  <div class="sec-group reveal" id="dealers">
    <h2 class="section-title">Dealers <span class="count">Retail operations</span></h2>
    <div class="article-table">

      <div class="article-row">
        <div class="score-chip">60</div>
        <div class="article-thumb"><img src="https://electrek.co/wp-content/uploads/sites/3/2026/08/28days_later.jpg?quality=82&strip=all&w=1600" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/05/a-month-after-congress-killed-the-solar-tax-credit-the-industry-is-anything-but-dead/" target="_blank" rel="noopener">After U.S. solar credit sunset, installs keep climbing</a>
          <div class="article-take">Energy retail adapts quickly—an indicator for dealer‑adjacent home charging offers.</div>
          <div class="article-tags"><span class="chip">Retail</span><span class="chip">Energy</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 5, 2026</span>
          <a href="https://electrek.co/2026/08/05/a-month-after-congress-killed-the-solar-tax-credit-the-industry-is-anything-but-dead/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

    </div>
  </div>

  <div class="sec-group reveal" id="suppliers">
    <h2 class="section-title">Suppliers <span class="count">Tier‑1 to infrastructure</span></h2>
    <div class="article-table">

      <div class="article-row">
        <div class="score-chip">82</div>
        <div class="article-thumb"><img src="https://electrek.co/wp-content/uploads/sites/3/2026/08/wynwood-village-station-press-release-2.jpg?quality=82&strip=all&w=1200" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/04/evgo-is-putting-500-fast-chargers-where-americans-shop/" target="_blank" rel="noopener">EVgo adds 500+ DCFC stalls at shopping centers</a>
          <div class="article-take">Portfolio shift toward convenient, high‑traffic locations.</div>
          <div class="article-tags"><span class="chip">EVgo</span><span class="chip">Charging</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 4, 2026</span>
          <a href="https://electrek.co/2026/08/04/evgo-is-putting-500-fast-chargers-where-americans-shop/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      
      <div class="article-row">
        <div class="score-chip">70</div>
        <div class="article-thumb"><img src="https://electrek.co/wp-content/uploads/sites/3/2026/07/Flint-Battery-storage-screenshot.jpg?quality=82&strip=all&w=1200" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/30/pjm-grid-largest-battery-is-now-under-construction-in-ohio/" target="_blank" rel="noopener">1 GWh battery under construction in Ohio (PJM)</a>
          <div class="article-take">Massive storage projects will buffer data‑center‑driven load growth.</div>
          <div class="article-tags"><span class="chip">Energy Storage</span><span class="chip">PJM</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 30, 2026</span>
          <a href="https://electrek.co/2026/07/30/pjm-grid-largest-battery-is-now-under-construction-in-ohio/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

    </div>
  </div>

  <div class="sec-group reveal" id="government">
    <h2 class="section-title">Government <span class="count">Policy & regulation</span></h2>
    <div class="article-table">

      <div class="article-row">
        <div class="score-chip">67</div>
        <div class="article-thumb"><img src="https://electrek.co/wp-content/uploads/sites/3/2026/08/wc-small-electric-triple-2025-me-70.jpg?quality=82&strip=all&w=1400" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/05/uk-records-strongest-ev-july-to-date/" target="_blank" rel="noopener">UK BEV share hits record in July</a>
          <div class="article-take">Progress toward ZEV mandates continues but needs acceleration.</div>
          <div class="article-tags"><span class="chip">UK</span><span class="chip">Policy</span></div>
        </div>
        <div class="article-source">
          <span>Electrive — Aug 5, 2026</span>
          <a href="https://www.electrive.com/2026/08/05/uk-records-strongest-ev-july-to-date/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      
      <div class="article-row">
        <div class="score-chip">65</div>
        <div class="article-thumb"><img src="https://electrek.co/wp-content/uploads/sites/3/2021/01/Tesla-Solar-Inverter-hero.jpg?quality=82&strip=all&w=1600" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/05/fcc-bans-foreign-made-connected-solar-inverters/" target="_blank" rel="noopener">FCC bans new foreign‑made connected inverters</a>
          <div class="article-take">Telecom oversight reaches into power electronics, tightening certification paths.</div>
          <div class="article-tags"><span class="chip">FCC</span><span class="chip">Inverters</span><span class="chip">Compliance</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 5, 2026</span>
          <a href="https://electrek.co/2026/08/05/fcc-bans-foreign-made-connected-solar-inverters/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

    </div>
  </div>

  <div class="sec-group reveal" id="technology">
    <h2 class="section-title">Technology <span class="count">Batteries, software & autonomy</span></h2>
    <div class="article-table">

      <div class="article-row">
        <div class="score-chip">84</div>
        <div class="article-thumb"><img src="https://electrek.co/wp-content/uploads/sites/3/2025/09/Mercedes-solid-state-EV-batteries-1.jpeg?quality=82&strip=all&w=1400" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">SK On and Factorial team up on solid‑state EV batteries</a>
          <div class="article-take">Partnerships multiply as OEMs seek credible scale paths for next‑gen cells.</div>
          <div class="article-tags"><span class="chip">Solid‑state</span><span class="chip">Batteries</span><span class="chip">Partnerships</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      
      <div class="article-row">
        <div class="score-chip">79</div>
        <div class="article-thumb"><img src="https://electrek.co/wp-content/uploads/sites/3/2026/07/Waymo-Gemini-integration-ojai.jpeg?quality=82&strip=all&w=1580" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/waymo-gemini-ai-ojai-robotaxi-redesigned-interface/" target="_blank" rel="noopener">Waymo adds Gemini AI and redesigned rider interface</a>
          <div class="article-take">A more conversational AV UX aims to reduce friction for first‑time robotaxi riders.</div>
          <div class="article-tags"><span class="chip">Waymo</span><span class="chip">Robotaxi</span><span class="chip">AI</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/waymo-gemini-ai-ojai-robotaxi-redesigned-interface/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

    </div>
  </div>

  <div class="sec-group reveal" id="finance">
    <h2 class="section-title">Finance <span class="count">Earnings & deals</span></h2>
    <div class="article-table">
      
      <div class="article-row">
        <div class="score-chip">73</div>
        <div class="article-thumb"><img src="https://images.cdn.autocar.co.uk/sites/autocar.co.uk/files/images/car-reviews/first-drives/legacy/robotaxi_87_0.jpg?itok=nITjPgOL" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/business-corporate/cheap-cars-hit-tesla-profits-tech-pivot-stalls" target="_blank" rel="noopener">Cheap cars hit Tesla profits as tech pivot stalls</a>
          <div class="article-take">Price‑driven volume is squeezing margins while autonomy timelines slip.</div>
          <div class="article-tags"><span class="chip">Tesla</span><span class="chip">Earnings</span><span class="chip">Pricing</span></div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 1, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/business-corporate/cheap-cars-hit-tesla-profits-tech-pivot-stalls" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">69</div>
        <div class="article-thumb"><img src="https://www.carscoops.com/wp-content/uploads/2026/08/GM-SAIC-1024x576.jpg" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://www.carscoops.com/2026/08/gm-saic-extension/" target="_blank" rel="noopener">GM extends 20‑year deal with SAIC</a>
          <div class="article-take">The JV will launch dozens of models as GM leans into China capacity and exports.</div>
          <div class="article-tags"><span class="chip">GM</span><span class="chip">SAIC</span><span class="chip">JV</span></div>
        </div>
        <div class="article-source">
          <span>Carscoops — Aug 5, 2026</span>
          <a href="https://www.carscoops.com/2026/08/gm-saic-extension/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

    </div>
  </div>

  <div class="sec-group reveal" id="international">
    <h2 class="section-title">International <span class="count">Cross‑border activity</span></h2>
    <div class="article-table">
      
      <div class="article-row">
        <div class="score-chip">69</div>
        <div class="article-thumb"><img src="https://electrek.co/wp-content/uploads/sites/3/2026/08/GM-Buick-NEVs-China.jpeg?quality=82&strip=all&w=1400" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/05/gm-buick-evs-china-overseas-suv/" target="_blank" rel="noopener">GM to ship China‑built Buick EVs overseas</a>
          <div class="article-take">Capacity redeployment positions GM for faster global EV rollout.</div>
          <div class="article-tags"><span class="chip">Exports</span><span class="chip">China</span><span class="chip">GM</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 5, 2026</span>
          <a href="https://electrek.co/2026/08/05/gm-buick-evs-china-overseas-suv/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      
      <div class="article-row">
        <div class="score-chip">67</div>
        <div class="article-thumb"><img src="https://www.electrive.com/media/2026/08/weride-robotaxi-gxr-greenmobility-kopenhagen-daenemark-400x267.jpeg" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/greenmobility-to-bring-weride-robotaxis-to-denmark/" target="_blank" rel="noopener">WeRide robotaxis to launch in Denmark with GreenMobility</a>
          <div class="article-take">Chinese AV tech expands into EU via car‑sharing partnerships.</div>
          <div class="article-tags"><span class="chip">WeRide</span><span class="chip">Denmark</span><span class="chip">Robotaxi</span></div>
        </div>
        <div class="article-source">
          <span>Electrive — Aug 4, 2026</span>
          <a href="https://www.electrive.com/2026/08/04/greenmobility-to-bring-weride-robotaxis-to-denmark/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

    </div>
  </div>

  <div class="sec-group reveal" id="opinion">
    <h2 class="section-title">Opinion <span class="count">Analysis & commentary</span></h2>
    <div class="article-table">
      
      <div class="article-row">
        <div class="score-chip">58</div>
        <div class="article-thumb"><img src="https://images.cdn.autocar.co.uk/sites/autocar.co.uk/files/images/car-reviews/first-drives/legacy/50555-26c0044-020.jpg?itok=RbUt5jP3" alt="" loading="lazy"></div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/mercedes-big-screens-stay-we-went-too-far-removing-buttons" target="_blank" rel="noopener">Mercedes: Big screens stay, but we went “too far” removing buttons</a>
          <div class="article-take">UX rethink brings back key physical controls without ditching screen real estate.</div>
          <div class="article-tags"><span class="chip">Mercedes</span><span class="chip">HMI</span><span class="chip">UX</span></div>
        </div>
        <div class="article-source">
          <span>Autocar — Jul 31, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/mercedes-big-screens-stay-we-went-too-far-removing-buttons" target="_blank" rel="noopener">Read original →</a>
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