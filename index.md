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
  margin-bottom:16px;
}
.exec-summary{
  color:var(--ink-dim);
  font-size:15.5px;
  margin-bottom:22px;
}
.takeaways h3,.impact-block h4,.related h4{
  font-family:'IBM Plex Mono',monospace;
  font-size:11px;
  letter-spacing:0.1em;
  color:var(--ink-dim);
  text-transform:uppercase;
  margin-bottom:10px;
  font-weight:500;
}
.takeaways ul{margin:0 0 22px;padding-left:18px}
.takeaways li{margin-bottom:6px}
.impact-row{
  display:grid;
  grid-template-columns:1.4fr 1fr;
  gap:24px;
  margin-bottom:22px;
  padding-top:20px;
  border-top:1px solid var(--line);
}
.impact-block p{margin:0;color:var(--ink-dim);font-size:14px}
.chip-row{display:flex;flex-wrap:wrap;gap:8px}
.chip{
  font-family:'IBM Plex Mono',monospace;
  font-size:11px;
  padding:5px 10px;
  border-radius:999px;
  background:var(--panel-2);
  border:1px solid var(--line);
  color:var(--ink-dim);
}
.chip.entity-mfr{border-color:#3a4a3f;color:var(--teal)}
.source-strip{
  display:flex;
  gap:16px;
  flex-wrap:wrap;
  align-items:center;
  font-size:12.5px;
  color:var(--ink-dim);
  padding-top:16px;
  border-top:1px solid var(--line);
  margin-bottom:18px;
}
.source-strip a{
  color:var(--amber);
  font-weight:500;
}
.source-strip a:hover{text-decoration:underline}
.related ul{list-style:none;margin:0;padding:0;display:flex;flex-direction:column;gap:6px}
.related a{color:var(--ink-dim);font-size:13px}
.related a:hover{color:var(--teal)}

/* Gauge cluster */
.hero-gauges{
  display:grid;
  grid-template-columns:1fr 1fr;
  gap:18px;
  align-content:start;
}
.gauge{
  background:var(--panel-2);
  border:1px solid var(--line);
  border-radius:10px;
  padding:16px 14px 14px;
  text-align:center;
}
.gauge svg{width:100%;height:auto;display:block}
.gauge-value{
  font-family:'IBM Plex Mono',monospace;
  font-size:22px;
  font-weight:600;
  margin-top:-34px;
  display:block;
}
.gauge-label{
  font-family:'IBM Plex Mono',monospace;
  font-size:10px;
  letter-spacing:0.08em;
  color:var(--ink-dim);
  text-transform:uppercase;
  display:block;
  margin-top:2px;
}

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
@media(max-width:768px){
  .article-row{grid-template-columns:40px 1fr;grid-template-areas:"score main" ". source"}
  .score-chip{grid-area:score;width:32px;height:32px;font-size:11px}
  .article-main{grid-area:main}
  .article-source{grid-area:source;align-items:flex-start;text-align:left}
  .hero-grid{grid-template-columns:1fr}
  .hero-gauges{grid-template-columns:repeat(4,1fr)}
  .impact-row{grid-template-columns:1fr}
}

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
  <nav class="section-nav">
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
</header>

<main class="wrap">

  <!--
    FEATURED STORY CONTRACT
    Selection: highest ImportanceScore across today's analyzed articles.
    Fields below map directly to <FeaturedStory><Output> in the spec.
    Populate script replaces each {{FEATURED_*}} / {{SCORE_*}} token.
    Executive summary and takeaways are ORIGINAL analysis — never
    paraphrase or reproduce source-article sentences here.
  -->
  <section class="hero reveal" id="featured">
    <span class="eyebrow">FEATURED STORY</span>
    <div class="hero-grid">
      <div class="hero-main">
        <h1>NHTSA opens probe into 1.2 million Tesla Model 3/Y over possible suspension failures</h1>
        <p class="exec-summary">US regulators launched a sweeping investigation into Tesla’s most popular models after reports of front suspension links detaching in motion. The probe brings fresh regulatory pressure on Tesla’s quality and safety controls, with potential implications for service costs, warranty reserves, parts suppliers and—most importantly—owner confidence heading into peak replacement cycles.</p>

        <div class="takeaways">
          <h3>Key Takeaways</h3>
          <ul>
            <li>Preliminary evaluation targets 2018–2020 Model 3 and 2021–2023 Model Y over lower lateral link separations.</li>
            <li>156 complaints triggered the action; outcomes range from service campaigns to a recall depending on defect scope.</li>
            <li>Any remedy could disrupt service capacity and parts logistics amid high Tesla parc growth.</li>
            <li>Findings may ripple to global regulators, increasing compliance and documentation demands on Tesla and suppliers.</li>
            <li>Short term: PR and resale-value sensitivity; long term: design validation and supplier quality audits in focus.</li>
          </ul>
        </div>

        <div class="impact-row">
          <div class="impact-block">
            <h4>Industry Impact</h4>
            <p>High-profile safety inquiries shape consumer trust in advanced EVs and can reset the bar for validation, traceability and supplier oversight across the sector. A forced remedy would pressure Tesla’s service operations and could accelerate broader industry moves to standardize suspension-component quality controls at growing EV volumes.</p>
          </div>
          <div class="impact-block">
            <h4>Companies Affected</h4>
            <div class="chip-row">
              <span class="chip entity-mfr">Tesla</span>
              <span class="chip">NHTSA</span>
              <span class="chip">Tier-1 suspension suppliers</span>
              <span class="chip">US Tesla owners</span>
            </div>
          </div>
        </div>

        <div class="source-strip">
          <span>Source: <b>Electrek</b></span>
          <span>Aug 4, 2026</span>
          <a href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">Read original →</a>
        </div>

        <div class="related">
          <h4>Related Coverage</h4>
          <ul>
            <li><a href="https://www.electrive.com/2026/08/03/nhtsa-opens-probe-into-1-2-million-teslas/" target="_blank" rel="noopener">NHTSA opens probe into 1.2 million Teslas</a></li>
            <li><a href="https://electrek.co/2026/07/28/tesla-sues-cybertruck-supplier-angstrom-tooling/" target="_blank" rel="noopener">Tesla sues Cybertruck supplier amid standoff keeping production hostage</a></li>
            <li><a href="https://electrek.co/2026/08/03/tesla-fsd-v14-lite-hw3-computer-failures/" target="_blank" rel="noopener">Tesla FSD v14 Lite tied to rising HW3 computer failures, owners report</a></li>
          </ul>
        </div>
      </div>

      <div class="hero-gauges">
        <div class="gauge">
          <svg viewBox="0 0 120 70"><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#2a3038" stroke-width="8"/><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#f2a93b" stroke-width="8" stroke-dasharray="157" stroke-dashoffset="11"/></svg>
          <span class="gauge-value mono">93</span>
          <span class="gauge-label">Importance</span>
        </div>
        <div class="gauge">
          <svg viewBox="0 0 120 70"><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#2a3038" stroke-width="8"/><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#3ecf8e" stroke-width="8" stroke-dasharray="157" stroke-dashoffset="19"/></svg>
          <span class="gauge-value mono">88</span>
          <span class="gauge-label">Editorial Quality</span>
        </div>
        <div class="gauge">
          <svg viewBox="0 0 120 70"><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#2a3038" stroke-width="8"/><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#e2604f" stroke-width="8" stroke-dasharray="157" stroke-dashoffset="16"/></svg>
          <span class="gauge-value mono">90</span>
          <span class="gauge-label">Industry Impact</span>
        </div>
        <div class="gauge">
          <svg viewBox="0 0 120 70"><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#2a3038" stroke-width="8"/><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#f2a93b" stroke-width="8" stroke-dasharray="157" stroke-dashoffset="8"/></svg>
          <span class="gauge-value mono">95</span>
          <span class="gauge-label">Reader Interest</span>
        </div>
      </div>
    </div>
  </section>

  <!--
    INDUSTRY SNAPSHOT CONTRACT
    One .stat-panel per <IndustrySnapshot> child element. Ranked lists
    use .rank-list (name + proportional bar + mention count); free-form
    groupings (trending topics, emerging tech) use .tagcloud instead.
  -->
  <section class="dashboard reveal" id="snapshot">
    <h2 class="section-title">Industry Snapshot <span class="count">Week of Aug 4, 2026</span></h2>
    <div class="dash-grid">
      <div class="stat-panel">
        <h4>Top Manufacturers</h4>
        <ul class="rank-list">
          <li><span>Tesla</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:100%"></span></span><span class="rank-count">14</span></li>
          <li><span>BYD</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:86%"></span></span><span class="rank-count">12</span></li>
          <li><span>Hyundai/Kia</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:79%"></span></span><span class="rank-count">11</span></li>
          <li><span>BMW</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:71%"></span></span><span class="rank-count">10</span></li>
          <li><span>Mercedes-Benz</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:57%"></span></span><span class="rank-count">8</span></li>
        </ul>
      </div>
      <div class="stat-panel">
        <h4>Top Brands</h4>
        <ul class="rank-list">
          <li><span>Audi</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:78%"></span></span><span class="rank-count">11</span></li>
          <li><span>Genesis</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:50%"></span></span><span class="rank-count">7</span></li>
          <li><span>Volkswagen</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:57%"></span></span><span class="rank-count">8</span></li>
          <li><span>Volvo</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:43%"></span></span><span class="rank-count">6</span></li>
          <li><span>Ferrari</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:36%"></span></span><span class="rank-count">5</span></li>
        </ul>
      </div>
      <div class="stat-panel">
        <h4>Top Suppliers</h4>
        <ul class="rank-list">
          <li><span>SK On</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:80%"></span></span><span class="rank-count">8</span></li>
          <li><span>Factorial</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:70%"></span></span><span class="rank-count">7</span></li>
          <li><span>Beam Global</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:60%"></span></span><span class="rank-count">6</span></li>
          <li><span>MAHLE</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:50%"></span></span><span class="rank-count">5</span></li>
          <li><span>Allego</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:40%"></span></span><span class="rank-count">4</span></li>
        </ul>
      </div>
      <div class="stat-panel">
        <h4>Most Mentioned Executives</h4>
        <ul class="rank-list">
          <li><span>Elon Musk (Tesla)</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:100%"></span></span><span class="rank-count">9</span></li>
          <li><span>Ola Källenius (Mercedes)</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:56%"></span></span><span class="rank-count">5</span></li>
          <li><span>Milan Nedeljković (BMW)</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:56%"></span></span><span class="rank-count">5</span></li>
          <li><span>RJ Scaringe (Rivian)</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:44%"></span></span><span class="rank-count">4</span></li>
          <li><span>Dmitri Dolgov (Waymo)</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:33%"></span></span><span class="rank-count">3</span></li>
        </ul>
      </div>
      <div class="stat-panel">
        <h4>Trending Topics</h4>
        <div class="tagcloud">
          <span class="chip lg">Safety probes</span>
          <span class="chip lg">Affordable EVs</span>
          <span class="chip">Charging build‑out</span>
          <span class="chip">Solid‑state batteries</span>
          <span class="chip">Robotaxis</span>
          <span class="chip">Long‑range claims</span>
          <span class="chip">Supplier risk</span>
          <span class="chip">Market share shifts</span>
        </div>
      </div>
      <div class="stat-panel">
        <h4>Emerging Technologies</h4>
        <div class="tagcloud">
          <span class="chip lg">Solid‑state cells</span>
          <span class="chip">Iron‑air storage</span>
          <span class="chip">Lidar alternatives</span>
          <span class="chip">GenAI in UX</span>
          <span class="chip">SDV architectures</span>
          <span class="chip">VPPs</span>
        </div>
      </div>
      <div class="stat-panel">
        <h4>Government Activity</h4>
        <ul class="rank-list">
          <li><span>NHTSA Tesla probe</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:100%"></span></span><span class="rank-count">1</span></li>
          <li><span>Philippines EV incentives</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:70%"></span></span><span class="rank-count">1</span></li>
          <li><span>UK grant updates</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:60%"></span></span><span class="rank-count">1</span></li>
          <li><span>Nordic EV adoption</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:55%"></span></span><span class="rank-count">2</span></li>
        </ul>
      </div>
      <div class="stat-panel">
        <h4>Supplier & Charging Activity</h4>
        <ul class="rank-list">
          <li><span>EVgo/Brixmor expansion</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:95%"></span></span><span class="rank-count">500+</span></li>
          <li><span>Allego UK rollout</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:80%"></span></span><span class="rank-count">1,400</span></li>
          <li><span>GM–Pilot–EVgo sites</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:65%"></span></span><span class="rank-count">130+</span></li>
        </ul>
      </div>
      <div class="stat-panel">
        <h4>Financial & Market Signals</h4>
        <ul class="rank-list">
          <li><span>Rivian Q2 beat</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:90%"></span></span><span class="rank-count">27%</span></li>
          <li><span>BYD July sales</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:80%"></span></span><span class="rank-count">+22%</span></li>
          <li><span>Lucid stake news</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:55%"></span></span><span class="rank-count">+25%</span></li>
        </ul>
      </div>
      <div class="stat-panel">
        <h4>Global Regions in Focus</h4>
        <div class="tagcloud">
          <span class="chip lg">United States</span>
          <span class="chip lg">China</span>
          <span class="chip">United Kingdom</span>
          <span class="chip">Nordics</span>
          <span class="chip">EU</span>
          <span class="chip">Southeast Asia</span>
        </div>
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
        <a href="https://www.autocar.co.uk/car-news/new-cars/audi-q9-suv-revealed-huge-%C2%A3100k-a8-successor" target="_blank" rel="noopener">Audi unveils Q9 flagship SUV</a>
        <div class="fp-meta"><span>Score 80</span><span>•</span><span>Aug 4, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">BMW pauses G‑Class rival as strategy shifts</a>
        <div class="fp-meta"><span>Score 76</span><span>•</span><span>Aug 4, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/new-mercedes-gla-ev-bigger-400-miles-range/" target="_blank" rel="noopener">Mercedes GLA EV grows up with 400+ mile range</a>
        <div class="fp-meta"><span>Score 85</span><span>•</span><span>Jul 29, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/ferrari-luce-ev-sold-out-2026-allocation/" target="_blank" rel="noopener">Ferrari’s Luce EV sells out 2026 run</a>
        <div class="fp-meta"><span>Score 70</span><span>•</span><span>Jul 29, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.autocar.co.uk/car-news/new-cars/byd-goes-after-defender-boxy-%C2%A348k-402bhp-hybrid-suv" target="_blank" rel="noopener">BYD brings boxy Ti7 hybrid to UK</a>
        <div class="fp-meta"><span>Score 73</span><span>•</span><span>Aug 1, 2026</span></div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Technology</h3>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Volvo drops lidar, compensates owners</a>
        <div class="fp-meta"><span>Score 88</span><span>•</span><span>Jul 29, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">SK On + Factorial ally on solid‑state</a>
        <div class="fp-meta"><span>Score 75</span><span>•</span><span>Jul 29, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/waymo-gemini-ai-ojai-robotaxi-redesigned-interface/" target="_blank" rel="noopener">Waymo integrates Gemini AI in Ojai robotaxi</a>
        <div class="fp-meta"><span>Score 78</span><span>•</span><span>Jul 29, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.autocar.co.uk/car-news/new-cars/reborn-audi-a2-driven-electric-comeback-efficiency-king" target="_blank" rel="noopener">Audi A2 e‑tron targets top-tier efficiency</a>
        <div class="fp-meta"><span>Score 74</span><span>•</span><span>Aug 4, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.electrive.com/2026/08/03/blue-solutions-and-avl-test-solid-state-battery-safety/" target="_blank" rel="noopener">Solid‑state safety advanced in AVL tests</a>
        <div class="fp-meta"><span>Score 68</span><span>•</span><span>Aug 3, 2026</span></div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Government & Policy</h3>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">NHTSA probes 1.2M Teslas’ suspensions</a>
        <div class="fp-meta"><span>Score 93</span><span>•</span><span>Jul 31, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.electrive.com/2026/08/04/philippines-launches-e850m-incentive-programme-for-ev-manufacturing/" target="_blank" rel="noopener">Philippines unveils €850m EV build incentives</a>
        <div class="fp-meta"><span>Score 72</span><span>•</span><span>Aug 4, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.electrive.com/2026/08/04/hyundai-kona-electric-now-qualifies-for-full-uk-electric-car-grant/" target="_blank" rel="noopener">UK upgrades Kona Electric to full grant tier</a>
        <div class="fp-meta"><span>Score 64</span><span>•</span><span>Aug 4, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.electrive.com/2026/08/04/denmark-evs-account-for-almost-all-new-car-registrations-in-july/" target="_blank" rel="noopener">Denmark hits 97% EV share for private buyers</a>
        <div class="fp-meta"><span>Score 77</span><span>•</span><span>Aug 4, 2026</span></div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Suppliers & Infrastructure</h3>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/28/tesla-sues-cybertruck-supplier-angstrom-tooling/" target="_blank" rel="noopener">Tesla seeks emergency access to supplier tools</a>
        <div class="fp-meta"><span>Score 74</span><span>•</span><span>Jul 28, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.electrive.com/2026/08/04/evgo-and-brixmor-to-add-more-than-500-fast-charging-stalls-in-the-us/" target="_blank" rel="noopener">EVgo + Brixmor to add 500+ DCFC stalls</a>
        <div class="fp-meta"><span>Score 70</span><span>•</span><span>Aug 4, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.electrive.com/2026/08/01/allego-commits-e100-million-to-expand-uk-charging-network/" target="_blank" rel="noopener">Allego invests €100m in UK ultra-rapid hubs</a>
        <div class="fp-meta"><span>Score 66</span><span>•</span><span>Aug 1, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://chargedevs.com/newswire/beam-global-supplies-ev-arc-off-grid-charging-systems-for-dallas-municipal-fleet-and-massachusetts-carshare-pilot/" target="_blank" rel="noopener">Beam’s off‑grid chargers expand in US fleets</a>
        <div class="fp-meta"><span>Score 62</span><span>•</span><span>Aug 1, 2026</span></div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Trending Topics</h3>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/28/volkswagen-launches-cheaper-id-polo-ev-orders-25000/" target="_blank" rel="noopener">Affordable EVs surge: VW ID. Polo hits 25k orders</a>
        <div class="fp-meta"><span>Score 80</span><span>•</span><span>Jul 28, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/hyundai-reveals-ioniq-3-prices-start-30000-interest-surges/" target="_blank" rel="noopener">Hyundai IONIQ 3 targets $30k sweet spot</a>
        <div class="fp-meta"><span>Score 82</span><span>•</span><span>Jul 29, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/08/03/byd-opens-denza-z9s-pre-orders-record-1100-km-ev-range/" target="_blank" rel="noopener">Range race escalates: BYD Denza Z9S 1,100 km CLTC</a>
        <div class="fp-meta"><span>Score 73</span><span>•</span><span>Aug 3, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/477795/" target="_blank" rel="noopener">IEA: EV sales rebound 35% in Q2; 50 nations set records</a>
        <div class="fp-meta"><span>Score 72</span><span>•</span><span>Jul 29, 2026</span></div>
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
    <h2 class="section-title">Latest Articles <span class="count">15 analyzed today</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip high">93</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">NHTSA probes 1.2 million Tesla Model 3/Y over suspension failures</a>
          <div class="article-take">A large safety inquiry could reshape Tesla’s service load, supplier QA, and near‑term brand sentiment.</div>
          <div class="article-tags">
            <span class="chip">Tesla</span><span class="chip">NHTSA</span><span class="chip">Safety</span><span class="chip">Recall/Probe</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 31, 2026</span>
          <a href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip high">88</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Volvo drops lidar on EX90 & ES90; pays compensation to owners</a>
          <div class="article-take">Cutting lidar trims cost/complexity but raises questions about sensor strategy and supplier exposure.</div>
          <div class="article-tags">
            <span class="chip">Volvo</span><span class="chip">Luminar</span><span class="chip">ADAS</span><span class="chip">Suppliers</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip high">85</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/new-mercedes-gla-ev-bigger-400-miles-range/" target="_blank" rel="noopener">Mercedes GLA EV gets bigger, smarter, and 400+ miles of range</a>
          <div class="article-take">Mercedes pushes mainstream appeal with space, 800V charging, and MB.OS upgrades in its entry SUV.</div>
          <div class="article-tags">
            <span class="chip">Mercedes-Benz</span><span class="chip">EV</span><span class="chip">Charging</span><span class="chip">Software</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/new-mercedes-gla-ev-bigger-400-miles-range/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">80</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/audi-q9-suv-revealed-huge-%C2%A3100k-a8-successor" target="_blank" rel="noopener">Audi reveals Q9 SUV as its new range‑topper</a>
          <div class="article-take">Big Audi leans into in‑car experience and premium margins while filling a profitable US/Middle East niche.</div>
          <div class="article-tags">
            <span class="chip">Audi</span><span class="chip">Manufacturing</span><span class="chip">Luxury</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 4, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/audi-q9-suv-revealed-huge-%C2%A3100k-a8-successor" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">70</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/ferrari-luce-ev-sold-out-2026-allocation/" target="_blank" rel="noopener">Ferrari’s $640K Luce EV sells out 2026 allocation</a>
          <div class="article-take">Ultra‑lux demand shows room for EVs at the top—even amid design debate and sky‑high pricing.</div>
          <div class="article-tags">
            <span class="chip">Ferrari</span><span class="chip">EV</span><span class="chip">Luxury</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/ferrari-luce-ev-sold-out-2026-allocation/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">82</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/hyundai-reveals-ioniq-3-prices-start-30000-interest-surges/" target="_blank" rel="noopener">Hyundai’s IONIQ 3 starts around $30k and demand surges</a>
          <div class="article-take">Aggressive pricing + 300‑mile range positions Hyundai to capture entry EV buyers en masse.</div>
          <div class="article-tags">
            <span class="chip">Hyundai</span><span class="chip">EV</span><span class="chip">Pricing</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/hyundai-reveals-ioniq-3-prices-start-30000-interest-surges/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">80</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/28/volkswagen-launches-cheaper-id-polo-ev-orders-25000/" target="_blank" rel="noopener">VW launches cheaper ID. Polo after 25,000 orders</a>
          <div class="article-take">A sub‑$30k EV from a legacy giant intensifies the affordability race across Europe.</div>
          <div class="article-tags">
            <span class="chip">Volkswagen</span><span class="chip">EV</span><span class="chip">Retail</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 28, 2026</span>
          <a href="https://electrek.co/2026/07/28/volkswagen-launches-cheaper-id-polo-ev-orders-25000/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">78</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/waymo-gemini-ai-ojai-robotaxi-redesigned-interface/" target="_blank" rel="noopener">Waymo adds Google Gemini AI assistant and new UI</a>
          <div class="article-take">Deepening Google integration signals a software‑led arms race in autonomous ride‑hail UX.</div>
          <div class="article-tags">
            <span class="chip">Waymo</span><span class="chip">Autonomous</span><span class="chip">Software</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/waymo-gemini-ai-ojai-robotaxi-redesigned-interface/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">74</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/28/byd-launches-worlds-first-sdv-kei-ev-starting-at-13000/" target="_blank" rel="noopener">BYD launches SDV kei EV from ~$13,000</a>
          <div class="article-take">Low‑cost software‑defined kei cars preview how China could reshape urban mobility segments.</div>
          <div class="article-tags">
            <span class="chip">BYD</span><span class="chip">EV</span><span class="chip">SDV</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 28, 2026</span>
          <a href="https://electrek.co/2026/07/28/byd-launches-worlds-first-sdv-kei-ev-starting-at-13000/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">72</div>
        <div class="article-main">
          <a class="headline" href="https://www.greencarreports.com/news/1146051_gm-pilot-ev-charging-network-now-spans-over-25-states" target="_blank" rel="noopener">GM–Pilot EV charging network spans 25+ states</a>
          <div class="article-take">OEM‑backed corridors strengthen highway coverage and brand‑owned energy ecosystems.</div>
          <div class="article-tags">
            <span class="chip">GM</span><span class="chip">Charging</span><span class="chip">Infrastructure</span>
          </div>
        </div>
        <div class="article-source">
          <span>Green Car Reports — Aug 3, 2026</span>
          <a href="https://www.greencarreports.com/news/1146051_gm-pilot-ev-charging-network-now-spans-over-25-states" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">78</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/30/rivian-rivn-q2-2026-earnings-r2-deliveries-revenue-up-27/" target="_blank" rel="noopener">Rivian Q2: revenue up 27%, record gross profit</a>
          <div class="article-take">R2 deliveries begin to translate hype into healthier unit economics and cash trajectory.</div>
          <div class="article-tags">
            <span class="chip">Rivian</span><span class="chip">Finance</span><span class="chip">Production</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 30, 2026</span>
          <a href="https://electrek.co/2026/07/30/rivian-rivn-q2-2026-earnings-r2-deliveries-revenue-up-27/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">77</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/denmark-evs-account-for-almost-all-new-car-registrations-in-july/" target="_blank" rel="noopener">Denmark: EVs make up 97% of private new car sales in July</a>
          <div class="article-take">Nordic momentum underscores policy + product alignment driving rapid ICE displacement.</div>
          <div class="article-tags">
            <span class="chip">Denmark</span><span class="chip">EV Adoption</span><span class="chip">Government</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrive — Aug 4, 2026</span>
          <a href="https://www.electrive.com/2026/08/04/denmark-evs-account-for-almost-all-new-car-registrations-in-july/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">76</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">BMW puts G‑Class rival on hold amid China headwinds</a>
          <div class="article-take">Macro shifts push BMW toward sharper portfolio discipline and regionalized demand planning.</div>
          <div class="article-tags">
            <span class="chip">BMW</span><span class="chip">Strategy</span><span class="chip">Manufacturing</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 4, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">73</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/03/byd-opens-denza-z9s-pre-orders-record-1100-km-ev-range/" target="_blank" rel="noopener">BYD’s Denza Z9S opens orders with 1,100 km CLTC</a>
          <div class="article-take">If verified in mixed cycles, extreme range could pressure premium rivals on spec sheets.</div>
          <div class="article-tags">
            <span class="chip">BYD</span><span class="chip">Range</span><span class="chip">Premium EV</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 3, 2026</span>
          <a href="https://electrek.co/2026/08/03/byd-opens-denza-z9s-pre-orders-record-1100-km-ev-range/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">75</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">SK On and Factorial team up to scale solid‑state batteries</a>
          <div class="article-take">Partnerships signal a shift from lab wins to pilot‑line manufacturability in next‑gen cells.</div>
          <div class="article-tags">
            <span class="chip">SK On</span><span class="chip">Factorial</span><span class="chip">Battery</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">Read original →</a>
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
    <h2 class="section-title">Industry News <span class="count">4 highlights</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip high">93</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">NHTSA opens probe into 1.2M Tesla vehicles</a>
          <div class="article-take">A potential suspension defect draws fresh regulatory heat to the US EV leader.</div>
          <div class="article-tags"><span class="chip">Safety</span><span class="chip">Regulation</span><span class="chip">Tesla</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 31, 2026</span>
          <a href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">76</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">BMW pauses hardcore SUV as market shifts</a>
          <div class="article-take">Softening China demand forces tighter capital allocation and model scrutiny.</div>
          <div class="article-tags"><span class="chip">BMW</span><span class="chip">Strategy</span></div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 4, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">72</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/477795/" target="_blank" rel="noopener">IEA: Global EV sales jump 35% in Q2; 50 nations set records</a>
          <div class="article-take">Momentum rebounds alongside greater model variety and improving infrastructure.</div>
          <div class="article-tags"><span class="chip">EV Adoption</span><span class="chip">Markets</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/477795/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">64</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/opinion/business-corporate/roof-boxes-top-car-accessory-market-defies-auto-downturn" target="_blank" rel="noopener">Accessory makers defy auto downturn</a>
          <div class="article-take">Premium lifestyle add‑ons keep margins healthy even as vehicle sales wobble.</div>
          <div class="article-tags"><span class="chip">Aftermarket</span><span class="chip">Profitability</span></div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 4, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/opinion/business-corporate/roof-boxes-top-car-accessory-market-defies-auto-downturn" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="electric-vehicles">
    <h2 class="section-title">Electric Vehicles <span class="count">5 highlights</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip high">85</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/new-mercedes-gla-ev-bigger-400-miles-range/" target="_blank" rel="noopener">Mercedes GLA EV debuts with 400+ mile range</a>
          <div class="article-take">A mass‑market spec sheet aimed squarely at EV skeptics.</div>
          <div class="article-tags"><span class="chip">Mercedes-Benz</span><span class="chip">EV</span><span class="chip">Range</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/new-mercedes-gla-ev-bigger-400-miles-range/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">82</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/hyundai-reveals-ioniq-3-prices-start-30000-interest-surges/" target="_blank" rel="noopener">Hyundai IONIQ 3 to start around $30k</a>
          <div class="article-take">Value leadership becomes a core Hyundai EV play.</div>
          <div class="article-tags"><span class="chip">Hyundai</span><span class="chip">Pricing</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/hyundai-reveals-ioniq-3-prices-start-30000-interest-surges/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">80</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/28/volkswagen-launches-cheaper-id-polo-ev-orders-25000/" target="_blank" rel="noopener">VW opens pre‑orders for cheaper ID. Polo</a>
          <div class="article-take">Compact EVs gather real order momentum at sub‑€30k prices.</div>
          <div class="article-tags"><span class="chip">Volkswagen</span><span class="chip">Retail</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 28, 2026</span>
          <a href="https://electrek.co/2026/07/28/volkswagen-launches-cheaper-id-polo-ev-orders-25000/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">74</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/reborn-audi-a2-driven-electric-comeback-efficiency-king" target="_blank" rel="noopener">Reborn Audi A2 targets efficiency leadership</a>
          <div class="article-take">Aerodynamics + updated MEB tech aim to stretch miles per kWh.</div>
          <div class="article-tags"><span class="chip">Audi</span><span class="chip">Efficiency</span></div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 4, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/reborn-audi-a2-driven-electric-comeback-efficiency-king" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">73</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/03/byd-opens-denza-z9s-pre-orders-record-1100-km-ev-range/" target="_blank" rel="noopener">BYD Denza Z9S claims 1,100 km CLTC range</a>
          <div class="article-take">Specmanship intensifies in premium long‑range battles.</div>
          <div class="article-tags"><span class="chip">BYD</span><span class="chip">Premium</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 3, 2026</span>
          <a href="https://electrek.co/2026/08/03/byd-opens-denza-z9s-pre-orders-record-1100-km-ev-range/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="manufacturers">
    <h2 class="section-title">Manufacturers <span class="count">5 highlights</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip">80</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/audi-q9-suv-revealed-huge-%C2%A3100k-a8-successor" target="_blank" rel="noopener">Audi Q9 debuts as luxury SUV flagship</a>
          <div class="article-take">Signals Audi’s upmarket pivot with experience‑led interiors.</div>
          <div class="article-tags"><span class="chip">Audi</span><span class="chip">Strategy</span></div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 4, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/audi-q9-suv-revealed-huge-%C2%A3100k-a8-successor" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">76</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">BMW trims future model slate amid China slowdown</a>
          <div class="article-take">Portfolio realism beats trophy projects in a tougher macro.</div>
          <div class="article-tags"><span class="chip">BMW</span><span class="chip">China</span></div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 4, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">70</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/ferrari-luce-ev-sold-out-2026-allocation/" target="_blank" rel="noopener">Ferrari’s first EV sells out its first year</a>
          <div class="article-take">Limited volume + brand gravity = fast sell‑through.</div>
          <div class="article-tags"><span class="chip">Ferrari</span><span class="chip">EV</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/ferrari-luce-ev-sold-out-2026-allocation/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">71</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/30/genesis-gv60-magma-costs-10k-more-than-hyundai-ioniq-5-n/" target="_blank" rel="noopener">Genesis GV60 Magma priced above IONIQ 5 N</a>
          <div class="article-take">Premium halo EVs test buyers’ appetite for brand elevation.</div>
          <div class="article-tags"><span class="chip">Genesis</span><span class="chip">Performance EV</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 30, 2026</span>
          <a href="https://electrek.co/2026/07/30/genesis-gv60-magma-costs-10k-more-than-hyundai-ioniq-5-n/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">73</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/byd-goes-after-defender-boxy-%C2%A348k-402bhp-hybrid-suv" target="_blank" rel="noopener">BYD Ti7 hybrid undercuts Defender in UK</a>
          <div class="article-take">Aggressive pricing meets rugged styling to woo family SUV buyers.</div>
          <div class="article-tags"><span class="chip">BYD</span><span class="chip">Hybrid</span></div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 1, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/byd-goes-after-defender-boxy-%C2%A348k-402bhp-hybrid-suv" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="dealers">
    <h2 class="section-title">Dealers <span class="count">3 highlights</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip">60</div>
        <div class="article-main">
          <a class="headline" href="https://www.carscoops.com/2026/08/servicemember-repossession-settlement/" target="_blank" rel="noopener">US DOJ settles with dealer over servicemember repossession case</a>
          <div class="article-take">Compliance lapses can carry steep reputational and legal costs for retailers.</div>
          <div class="article-tags"><span class="chip">Dealers</span><span class="chip">Legal</span></div>
        </div>
        <div class="article-source">
          <span>Carscoops — Aug 4, 2026</span>
          <a href="https://www.carscoops.com/2026/08/servicemember-repossession-settlement/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">58</div>
        <div class="article-main">
          <a class="headline" href="https://www.motor1.com/news/803722/costco-infiniti-discount/" target="_blank" rel="noopener">Costco offers big discounts on new Infiniti SUVs</a>
          <div class="article-take">Warehouse partnerships keep traffic flowing amid deal‑driven markets.</div>
          <div class="article-tags"><span class="chip">Retail</span><span class="chip">Incentives</span></div>
        </div>
        <div class="article-source">
          <span>Motor1 — Aug 4, 2026</span>
          <a href="https://www.motor1.com/news/803722/costco-infiniti-discount/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">55</div>
        <div class="article-main">
          <a class="headline" href="https://www.carscoops.com/2026/08/costco-infiniti-discount/" target="_blank" rel="noopener">Infiniti’s new QX65 already has a Costco deal</a>
          <div class="article-take">Early promo pricing aims to speed showroom turns on fresh sheetmetal.</div>
          <div class="article-tags"><span class="chip">Infiniti</span><span class="chip">Sales</span></div>
        </div>
        <div class="article-source">
          <span>Carscoops — Aug 3, 2026</span>
          <a href="https://www.carscoops.com/2026/08/costco-infiniti-discount/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="suppliers">
    <h2 class="section-title">Suppliers <span class="count">5 highlights</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip">74</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/28/tesla-sues-cybertruck-supplier-angstrom-tooling/" target="_blank" rel="noopener">Tesla sues supplier to retrieve Cybertruck tooling</a>
          <div class="article-take">A rare public dispute spotlights program risk when single‑source tools get stranded.</div>
          <div class="article-tags"><span class="chip">Suppliers</span><span class="chip">Production</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 28, 2026</span>
          <a href="https://electrek.co/2026/07/28/tesla-sues-cybertruck-supplier-angstrom-tooling/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">75</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">SK On and Factorial join forces on solid‑state</a>
          <div class="article-take">Alliances aim to de‑risk scale‑up from pilot to pack.</div>
          <div class="article-tags"><span class="chip">Battery</span><span class="chip">Partnerships</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">63</div>
        <div class="article-main">
          <a class="headline" href="https://chargedevs.com/newswire/mahle-introduces-a-new-range-extender-engine-and-a-rare-earth-free-electric-motor/" target="_blank" rel="noopener">MAHLE unveils HD range extender and rare‑earth‑free motor</a>
          <div class="article-take">Component innovation targets cost, packaging and supply security.</div>
          <div class="article-tags"><span class="chip">MAHLE</span><span class="chip">Powertrain</span></div>
        </div>
        <div class="article-source">
          <span>Charged EVs — Jul 31, 2026</span>
          <a href="https://chargedevs.com/newswire/mahle-introduces-a-new-range-extender-engine-and-a-rare-earth-free-electric-motor/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">60</div>
        <div class="article-main">
          <a class="headline" href="https://chargedevs.com/newswire/automat-solutions-new-lytematch-and-lyteguide-software-platforms-facilitate-battery-electrolyte-development/" target="_blank" rel="noopener">Tools emerge to accelerate electrolyte development</a>
          <div class="article-take">Software enters the lab to compress materials discovery timelines.</div>
          <div class="article-tags"><span class="chip">Software</span><span class="chip">Battery R&D</span></div>
        </div>
        <div class="article-source">
          <span>Charged EVs — Aug 1, 2026</span>
          <a href="https://chargedevs.com/newswire/automat-solutions-new-lytematch-and-lyteguide-software-platforms-facilitate-battery-electrolyte-development/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">58</div>
        <div class="article-main">
          <a class="headline" href="https://chargedevs.com/newswire/danisenses-new-current-transducer-measures-isolated-dc-and-ac-current-in-power-electronics/" target="_blank" rel="noopener">Danisense introduces precision current transducer</a>
          <div class="article-take">Measurement accuracy improvements feed inverter and charger design.</div>
          <div class="article-tags"><span class="chip">Power Electronics</span><span class="chip">Suppliers</span></div>
        </div>
        <div class="article-source">
          <span>Charged EVs — Aug 2, 2026</span>
          <a href="https://chargedevs.com/newswire/danisenses-new-current-transducer-measures-isolated-dc-and-ac-current-in-power-electronics/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="government">
    <h2 class="section-title">Government <span class="count">5 highlights</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip high">93</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">NHTSA investigates Tesla suspension complaints</a>
          <div class="article-take">Outcome could trigger a major service action across a large US EV fleet.</div>
          <div class="article-tags"><span class="chip">NHTSA</span><span class="chip">Safety</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 31, 2026</span>
          <a href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      
      <div class="article-row">
        <div class="score-chip">72</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/philippines-launches-e850m-incentive-programme-for-ev-manufacturing/" target="_blank" rel="noopener">Philippines launches major EV manufacturing incentives</a>
          <div class="article-take">Southeast Asia sharpens its bid to capture EV supply chains.</div>
          <div class="article-tags"><span class="chip">Policy</span><span class="chip">Manufacturing</span></div>
        </div>
        <div class="article-source">
          <span>Electrive — Aug 4, 2026</span>
          <a href="https://www.electrive.com/2026/08/04/philippines-launches-e850m-incentive-programme-for-ev-manufacturing/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      
      <div class="article-row">
        <div class="score-chip">64</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/hyundai-kona-electric-now-qualifies-for-full-uk-electric-car-grant/" target="_blank" rel="noopener">Kona Electric now qualifies for full UK grant</a>
          <div class="article-take">Eligibility shift sweetens the TCO case for company‑car drivers.</div>
          <div class="article-tags"><span class="chip">UK</span><span class="chip">Incentives</span></div>
        </div>
        <div class="article-source">
          <span>Electrive — Aug 4, 2026</span>
          <a href="https://www.electrive.com/2026/08/04/hyundai-kona-electric-now-qualifies-for-full-uk-electric-car-grant/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      
      <div class="article-row">
        <div class="score-chip">77</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/denmark-evs-account-for-almost-all-new-car-registrations-in-july/" target="_blank" rel="noopener">Denmark’s near‑100% EV share for private buyers</a>
          <div class="article-take">Policy clarity + product depth drive rapid ICE phase‑down.</div>
          <div class="article-tags"><span class="chip">Denmark</span><span class="chip">EV Adoption</span></div>
        </div>
        <div class="article-source">
          <span>Electrive — Aug 4, 2026</span>
          <a href="https://www.electrive.com/2026/08/04/denmark-evs-account-for-almost-all-new-car-registrations-in-july/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      
      <div class="article-row">
        <div class="score-chip">69</div>
        <div class="article-main">
          <a class="headline" href="https://www.greencarreports.com/news/1146045_california-has-nearly-50-more-public-ev-chargers-than-gas-nozzles" target="_blank" rel="noopener">California now has far more public EV plugs than gas nozzles</a>
          <div class="article-take">Network scale is reaching parity—and surpassing—legacy fueling in key markets.</div>
          <div class="article-tags"><span class="chip">California</span><span class="chip">Charging</span></div>
        </div>
        <div class="article-source">
          <span>Green Car Reports — Aug 2, 2026</span>
          <a href="https://www.greencarreports.com/news/1146045_california-has-nearly-50-more-public-ev-chargers-than-gas-nozzles" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      
    </div>
  </div>

  <div class="sec-group reveal" id="technology">
    <h2 class="section-title">Technology <span class="count">5 highlights</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip high">88</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Volvo walks away from lidar on key models</a>
          <div class="article-take">Sensor stack choices are narrowing as OEMs seek cost and integration wins.</div>
          <div class="article-tags"><span class="chip">ADAS</span><span class="chip">Sensors</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      
      <div class="article-row">
        <div class="score-chip">78</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/waymo-gemini-ai-ojai-robotaxi-redesigned-interface/" target="_blank" rel="noopener">Waymo integrates Gemini AI into robotaxi UX</a>
          <div class="article-take">Conversational interfaces are becoming table‑stakes for AV passenger experience.</div>
          <div class="article-tags"><span class="chip">Autonomous</span><span class="chip">AI</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/waymo-gemini-ai-ojai-robotaxi-redesigned-interface/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      
      <div class="article-row">
        <div class="score-chip">75</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">Solid‑state battery partnership advances scale</a>
          <div class="article-take">Partnerships can bridge chemistry wins to manufacturable products.</div>
          <div class="article-tags"><span class="chip">Battery</span><span class="chip">Manufacturing</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      
      <div class="article-row">
        <div class="score-chip">68</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/03/blue-solutions-and-avl-test-solid-state-battery-safety/" target="_blank" rel="noopener">AVL tests show steps toward safer solid‑state cells</a>
          <div class="article-take">Thermal propagation control remains the gating factor for SSB adoption.</div>
          <div class="article-tags"><span class="chip">Safety</span><span class="chip">Battery</span></div>
        </div>
        <div class="article-source">
          <span>Electrive — Aug 3, 2026</span>
          <a href="https://www.electrive.com/2026/08/03/blue-solutions-and-avl-test-solid-state-battery-safety/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      
      <div class="article-row">
        <div class="score-chip">67</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/04/waymo-co-ceo-camera-only-self-driving-tesla/" target="_blank" rel="noopener">Waymo CEO critiques camera‑only autonomy</a>
          <div class="article-take">Strong sensing stacks are argued as essential to surpass human safety baselines.</div>
          <div class="article-tags"><span class="chip">Autonomy</span><span class="chip">Sensors</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 4, 2026</span>
          <a href="https://electrek.co/2026/08/04/waymo-co-ceo-camera-only-self-driving-tesla/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      
    </div>
  </div>

  <div class="sec-group reveal" id="finance">
    <h2 class="section-title">Finance <span class="count">5 highlights</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip">78</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/30/rivian-rivn-q2-2026-earnings-r2-deliveries-revenue-up-27/" target="_blank" rel="noopener">Rivian Q2 beats with improving margins</a>
          <div class="article-take">Scaling a lower‑cost model starts to bend the cost curve.</div>
          <div class="article-tags"><span class="chip">Earnings</span><span class="chip">Rivian</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 30, 2026</span>
          <a href="https://electrek.co/2026/07/30/rivian-rivn-q2-2026-earnings-r2-deliveries-revenue-up-27/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      
      <div class="article-row">
        <div class="score-chip">72</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/03/byd-boosts-sales-by-22-in-july/" target="_blank" rel="noopener">BYD July sales climb 22% with record exports</a>
          <div class="article-take">Exports offset softer home market and diversify revenue mix.</div>
          <div class="article-tags"><span class="chip">BYD</span><span class="chip">Sales</span></div>
        </div>
        <div class="article-source">
          <span>Electrive — Aug 3, 2026</span>
          <a href="https://www.electrive.com/2026/08/03/byd-boosts-sales-by-22-in-july/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      
      <div class="article-row">
        <div class="score-chip">69</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/06/tesla-10-millionth-vehicle-ev-growth-stalled/" target="_blank" rel="noopener">Tesla hits 10M vehicles as growth cools</a>
          <div class="article-take">Scale milestone meets under‑utilized capacity—efficiency becomes key.</div>
          <div class="article-tags"><span class="chip">Tesla</span><span class="chip">Production</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 30, 2026</span>
          <a href="https://electrek.co/2026/06/tesla-10-millionth-vehicle-ev-growth-stalled/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      
      <div class="article-row">
        <div class="score-chip">65</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/28/saudi-prince-alwaleed-5-percent-lucid-stake-lcid/" target="_blank" rel="noopener">Prince Alwaleed discloses 5% Lucid stake; stock jumps</a>
          <div class="article-take">A confidence signal from a key backer buys time for execution.</div>
          <div class="article-tags"><span class="chip">Lucid</span><span class="chip">Capital</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 28, 2026</span>
          <a href="https://electrek.co/2026/07/28/saudi-prince-alwaleed-5-percent-lucid-stake-lcid/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      
      <div class="article-row">
        <div class="score-chip">63</div>
        <div class="article-main">
          <a class="headline" href="https://www.roadandtrack.com/news/a73307948/bmw-job-cuts-following-profit-drop-reevaluate-future-car-plans/" target="_blank" rel="noopener">BMW mulls job cuts after profit drop</a>
          <div class="article-take">Cost discipline meets portfolio pruning as profits compress.</div>
          <div class="article-tags"><span class="chip">BMW</span><span class="chip">Restructuring</span></div>
        </div>
        <div class="article-source">
          <span>Road & Track — Jul 31, 2026</span>
          <a href="https://www.roadandtrack.com/news/a73307948/bmw-job-cuts-following-profit-drop-reevaluate-future-car-plans/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      
    </div>
  </div>

  <div class="sec-group reveal" id="international">
    <h2 class="section-title">International <span class="count">4 highlights</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip">71</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/28/baidu-apollo-go-london-robotaxi-testing-uber-lyft/" target="_blank" rel="noopener">Baidu’s Apollo Go begins robotaxi testing in London</a>
          <div class="article-take">Chinese AV players expand with Western ride‑hail partners.</div>
          <div class="article-tags"><span class="chip">Baidu</span><span class="chip">AV</span><span class="chip">UK</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 28, 2026</span>
          <a href="https://electrek.co/2026/07/28/baidu-apollo-go-london-robotaxi-testing-uber-lyft/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      
      <div class="article-row">
        <div class="score-chip">73</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/03/norways-ev-share-rises-to-97-6-in-july/" target="_blank" rel="noopener">Norway’s EV share rises to 97.6% in July</a>
          <div class="article-take">Long‑standing EV leader holds course on ICE‑free trajectory.</div>
          <div class="article-tags"><span class="chip">Norway</span><span class="chip">EV Adoption</span></div>
        </div>
        <div class="article-source">
          <span>Electrive — Aug 3, 2026</span>
          <a href="https://www.electrive.com/2026/08/03/norways-ev-share-rises-to-97-6-in-july/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      
      <div class="article-row">
        <div class="score-chip">68</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/01/xpeng-announces-major-expansion-plans-for-australia-and-new-zealand/" target="_blank" rel="noopener">XPeng outlines expansion in Australia & New Zealand</a>
          <div class="article-take">Chinese brands continue their global march with broader retail footprints.</div>
          <div class="article-tags"><span class="chip">XPeng</span><span class="chip">Expansion</span></div>
        </div>
        <div class="article-source">
          <span>Electrive — Aug 1, 2026</span>
          <a href="https://www.electrive.com/2026/08/01/xpeng-announces-major-expansion-plans-for-australia-and-new-zealand/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      
      <div class="article-row">
        <div class="score-chip">66</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/30/kia-ev3-production-mexico-us/" target="_blank" rel="noopener">Kia EV3 to be built in Mexico for North America</a>
          <div class="article-take">Local sourcing sets up competitive pricing and logistics to the US market.</div>
          <div class="article-tags"><span class="chip">Kia</span><span class="chip">Manufacturing</span><span class="chip">Mexico</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 30, 2026</span>
          <a href="https://electrek.co/2026/07/30/kia-ev3-production-mexico-us/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      
    </div>
  </div>

  <div class="sec-group reveal" id="opinion">
    <h2 class="section-title">Opinion <span class="count">3 reads</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip">58</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/opinion/new-cars/ignore-jay-leno-your-dream-garage-only-needs-three-cars" target="_blank" rel="noopener">Your dream garage probably only needs three cars</a>
          <div class="article-take">A case for quality over quantity—and why you should drive what you own.</div>
          <div class="article-tags"><span class="chip">Opinion</span><span class="chip">Culture</span></div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 4, 2026</span>
          <a href="https://www.autocar.co.uk/opinion/new-cars/ignore-jay-leno-your-dream-garage-only-needs-three-cars" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      
      <div class="article-row">
        <div class="score-chip">60</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/opinion/business-manufacturing/chinese-car-makers-all-share-parts-will-world-follow" target="_blank" rel="noopener">China’s shared‑parts playbook: will the world follow?</a>
          <div class="article-take">Standardization trims cost and time—but can brands still stand out?</div>
          <div class="article-tags"><span class="chip">China</span><span class="chip">Supply Chain</span></div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 4, 2026</span>
          <a href="https://www.autocar.co.uk/opinion/business-manufacturing/chinese-car-makers-all-share-parts-will-world-follow" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      
      <div class="article-row">
        <div class="score-chip">59</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/opinion/new-cars/will-ferraris-synthesised-gearbox-really-delight-drivers" target="_blank" rel="noopener">Will Ferrari’s synthesised manual really delight?</a>
          <div class="article-take">If the feel is faithful, does the missing mechanical link matter?</div>
          <div class="article-tags"><span class="chip">Ferrari</span><span class="chip">Experience</span></div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 4, 2026</span>
          <a href="https://www.autocar.co.uk/opinion/new-cars/will-ferraris-synthesised-gearbox-really-delight-drivers" target="_blank" rel="noopener">Read original →</a>
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