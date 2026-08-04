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
        <h1>NHTSA opens probe into 1.2 million Tesla Model 3 and Model Y over suspension failures</h1>
        <p class="exec-summary">US safety regulators launched a sweeping investigation into front-suspension link separations on high‑volume Tesla models sold between 2018 and 2023. The probe puts fresh scrutiny on Tesla’s design robustness and service practices, raises potential recall exposure, and signals more assertive oversight as the EV fleet ages and failure modes surface at scale.</p>

        <div class="takeaways">
          <h3>Key Takeaways</h3>
          <ul>
            <li>Scope covers roughly 1.2 million cars, indicating a systemic issue window rather than isolated incidents.</li>
            <li>A suspension link detachment risks loss of steering control — a high-severity safety outcome that typically triggers prompt corrective action.</li>
            <li>Investigation outcome could force design, parts and torque-spec changes, plus expanded parts inventory and retrofit capacity in service centers.</li>
            <li>Wider implication: maturing EV fleets are entering the wear‑out phase; quality and aftersales operations will increasingly define brand trust.</li>
          </ul>
        </div>

        <div class="impact-row">
          <div class="impact-block">
            <h4>Industry Impact</h4>
            <p>Should NHTSA substantiate a defect trend, the resulting recall would be one of the largest for a modern EV and could tighten validation expectations for high-load chassis components across the sector. Regulators, insurers and fleets are likely to sharpen focus on underbody durability, while suppliers see opportunity for upgraded bushings, links and corrosion protection engineered for heavier EV duty cycles.</p>
          </div>
          <div class="impact-block">
            <h4>Companies Affected</h4>
            <div class="chip-row">
              <span class="chip entity-mfr">Tesla</span>
              <span class="chip">NHTSA</span>
              <span class="chip">Model 3</span>
              <span class="chip">Model Y</span>
            </div>
          </div>
        </div>

        <div class="source-strip">
          <span>Source: <b>Electrek</b></span>
          <span>July 31, 2026</span>
          <a href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">Read original →</a>
        </div>

        <div class="related">
          <h4>Related Coverage</h4>
          <ul>
            <li><a href="https://electrek.co/2026/08/03/tesla-fsd-v14-lite-hw3-computer-failures/" target="_blank" rel="noopener">Tesla FSD v14 Lite tied to rising HW3 computer failures, owners report</a></li>
            <li><a href="https://electrek.co/2026/08/04/tesla-china-sales-crash-exports-surge-h1-2026/" target="_blank" rel="noopener">Tesla China sales are crashing as exports surge</a></li>
            <li><a href="https://electrek.co/2026/07/30/tesla-10-millionth-vehicle-ev-growth-stalled/" target="_blank" rel="noopener">Tesla hits 10 million vehicles — but its EV growth has stalled</a></li>
            <li><a href="https://electrek.co/2026/07/28/tesla-sues-cybertruck-supplier-angstrom-tooling/" target="_blank" rel="noopener">Tesla sues Cybertruck supplier amid standoff keeping production hostage</a></li>
          </ul>
        </div>
      </div>

      <div class="hero-gauges">
        <div class="gauge">
          <svg viewBox="0 0 120 70"><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#2a3038" stroke-width="8"/><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#f2a93b" stroke-width="8" stroke-dasharray="157" stroke-dashoffset="7.85"/></svg>
          <span class="gauge-value mono">95</span>
          <span class="gauge-label">Importance</span>
        </div>
        <div class="gauge">
          <svg viewBox="0 0 120 70"><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#2a3038" stroke-width="8"/><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#3ecf8e" stroke-width="8" stroke-dasharray="157" stroke-dashoffset="18.84"/></svg>
          <span class="gauge-value mono">88</span>
          <span class="gauge-label">Editorial Quality</span>
        </div>
        <div class="gauge">
          <svg viewBox="0 0 120 70"><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#2a3038" stroke-width="8"/><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#e2604f" stroke-width="8" stroke-dasharray="157" stroke-dashoffset="10.99"/></svg>
          <span class="gauge-value mono">93</span>
          <span class="gauge-label">Industry Impact</span>
        </div>
        <div class="gauge">
          <svg viewBox="0 0 120 70"><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#2a3038" stroke-width="8"/><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#f2a93b" stroke-width="8" stroke-dasharray="157" stroke-dashoffset="15.70"/></svg>
          <span class="gauge-value mono">90</span>
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
    <h2 class="section-title">Industry Snapshot <span class="count">Past 48 hours</span></h2>
    <div class="dash-grid">
      <div class="stat-panel">
        <h4>Top Manufacturers</h4>
        <ul class="rank-list">
          <li><span>BYD</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:100%"></div></div><span class="rank-count">12</span></li>
          <li><span>Tesla</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:88%"></div></div><span class="rank-count">11</span></li>
          <li><span>Hyundai/Kia</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:80%"></div></div><span class="rank-count">10</span></li>
          <li><span>BMW</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:67%"></div></div><span class="rank-count">8</span></li>
          <li><span>Audi</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:58%"></div></div><span class="rank-count">7</span></li>
        </ul>
      </div>
      <div class="stat-panel">
        <h4>Top Brands</h4>
        <ul class="rank-list">
          <li><span>Genesis</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:75%"></div></div><span class="rank-count">9</span></li>
          <li><span>Volvo</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:67%"></div></div><span class="rank-count">8</span></li>
          <li><span>Mercedes-Benz</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:58%"></div></div><span class="rank-count">7</span></li>
          <li><span>Volkswagen</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:42%"></div></div><span class="rank-count">5</span></li>
          <li><span>Rivian</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:42%"></div></div><span class="rank-count">5</span></li>
        </ul>
      </div>
      <div class="stat-panel">
        <h4>Top Suppliers / Networks</h4>
        <ul class="rank-list">
          <li><span>EVgo / Brixmor</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:100%"></div></div><span class="rank-count">6</span></li>
          <li><span>Beam Global</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:83%"></div></div><span class="rank-count">5</span></li>
          <li><span>MAHLE</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:67%"></div></div><span class="rank-count">4</span></li>
          <li><span>Blue Solutions / AVL</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:50%"></div></div><span class="rank-count">3</span></li>
          <li><span>Automat Solutions</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:33%"></div></div><span class="rank-count">2</span></li>
        </ul>
      </div>
      <div class="stat-panel">
        <h4>Most Mentioned Executives</h4>
        <ul class="rank-list">
          <li><span>Elon Musk (Tesla)</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:100%"></div></div><span class="rank-count">7</span></li>
          <li><span>Gernot Döllner (Audi)</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:71%"></div></div><span class="rank-count">5</span></li>
          <li><span>Michael Leiters (Porsche)</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:57%"></div></div><span class="rank-count">4</span></li>
          <li><span>RJ Scaringe (Rivian)</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:43%"></div></div><span class="rank-count">3</span></li>
          <li><span>Ola Källenius (Mercedes)</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:29%"></div></div><span class="rank-count">2</span></li>
        </ul>
      </div>
      <div class="stat-panel">
        <h4>Trending Topics</h4>
        <div class="tagcloud">
          <span class="chip lg">Safety probes</span>
          <span class="chip">EV efficiency</span>
          <span class="chip">Solid-state batteries</span>
          <span class="chip">Robotaxi UX</span>
          <span class="chip">Charging build‑out</span>
          <span class="chip">Hybrids surge</span>
          <span class="chip">China exports</span>
          <span class="chip">Software-defined vehicle</span>
          <span class="chip">Recalls</span>
        </div>
      </div>
      <div class="stat-panel">
        <h4>Emerging Technologies</h4>
        <div class="tagcloud">
          <span class="chip lg">Solid-state (SK On/Factorial)</span>
          <span class="chip">Iron‑air LDES</span>
          <span class="chip">800V platforms</span>
          <span class="chip">AI copilots in AVs</span>
          <span class="chip">V2L / off‑grid charging</span>
          <span class="chip">Sensor fusion post‑lidar</span>
        </div>
      </div>
      <div class="stat-panel">
        <h4>Government & Policy</h4>
        <ul class="rank-list">
          <li><span>NHTSA Tesla probe</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:100%"></div></div><span class="rank-count">1</span></li>
          <li><span>Philippines EV incentives</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:80%"></div></div><span class="rank-count">1</span></li>
          <li><span>Denmark EV grant uplift</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:80%"></div></div><span class="rank-count">1</span></li>
          <li><span>China ADAS light ban</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:60%"></div></div><span class="rank-count">1</span></li>
        </ul>
      </div>
      <div class="stat-panel">
        <h4>Financial & Capital</h4>
        <ul class="rank-list">
          <li><span>Rivian Q2 beat</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:100%"></div></div><span class="rank-count">1</span></li>
          <li><span>Base Power $1B raise</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:88%"></div></div><span class="rank-count">1</span></li>
          <li><span>Drivalia EIB loan</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:75%"></div></div><span class="rank-count">1</span></li>
          <li><span>BYD July sales +22%</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:63%"></div></div><span class="rank-count">1</span></li>
        </ul>
      </div>
      <div class="stat-panel">
        <h4>Global Regions</h4>
        <div class="tagcloud">
          <span class="chip lg">United States</span>
          <span class="chip lg">China</span>
          <span class="chip">United Kingdom</span>
          <span class="chip">European Union</span>
          <span class="chip">Nordics</span>
          <span class="chip">Mexico</span>
          <span class="chip">Philippines</span>
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
        <a href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">BMW puts G‑Class rival on hold as China headwinds bite</a>
        <div class="fp-meta"><span>Score 82</span><span>•</span><span>Autocar</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.autocar.co.uk/car-news/new-cars/audi-q9-suv-revealed-huge-%C2%A3100k-a8-successor" target="_blank" rel="noopener">Audi reveals Q9 flagship SUV aimed at US and Middle East</a>
        <div class="fp-meta"><span>Score 78</span><span>•</span><span>Autocar</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/hyundai-reveals-ioniq-3-prices-start-30000-interest-surges/" target="_blank" rel="noopener">Hyundai’s IONIQ 3 debuts at ~$30k with strong demand</a>
        <div class="fp-meta"><span>Score 80</span><span>•</span><span>Electrek</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/31/byd-undercuts-defender-first-7-seat-suv-uk/" target="_blank" rel="noopener">BYD launches Ti 7 seven‑seat SUV, undercutting Defender</a>
        <div class="fp-meta"><span>Score 77</span><span>•</span><span>Electrek</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/08/04/new-porsche-boss-says-electric-718-is-still-coming-taycan-isnt-going-anywhere/" target="_blank" rel="noopener">Porsche’s new CEO reaffirms electric 718 and Taycan</a>
        <div class="fp-meta"><span>Score 73</span><span>•</span><span>Electrek</span></div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Technology</h3>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/waymo-gemini-ai-ojai-robotaxi-redesigned-interface/" target="_blank" rel="noopener">Waymo adds Google Gemini assistant and new rider UI</a>
        <div class="fp-meta"><span>Score 76</span><span>•</span><span>Electrek</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">SK On and Factorial expand solid‑state alliance</a>
        <div class="fp-meta"><span>Score 79</span><span>•</span><span>Electrek</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Volvo exits lidar on EX90/ES90, compensates owners</a>
        <div class="fp-meta"><span>Score 81</span><span>•</span><span>Electrek</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/08/04/waymo-co-ceo-camera-only-self-driving-tesla/" target="_blank" rel="noopener">Waymo CEO: camera‑only autonomy hits a safety ceiling</a>
        <div class="fp-meta"><span>Score 75</span><span>•</span><span>Electrek</span></div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Government</h3>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">NHTSA opens Tesla suspension probe (1.2M vehicles)</a>
        <div class="fp-meta"><span>Score 95</span><span>•</span><span>Electrek</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.electrive.com/2026/08/04/philippines-launches-e850m-incentive-programme-for-ev-manufacturing/" target="_blank" rel="noopener">Philippines launches €850m EV manufacturing incentives</a>
        <div class="fp-meta"><span>Score 72</span><span>•</span><span>electrive</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.carscoops.com/2026/08/china-autonomous-light-ban/" target="_blank" rel="noopener">China bans turquoise self‑driving lights</a>
        <div class="fp-meta"><span>Score 68</span><span>•</span><span>Carscoops</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.roadandtrack.com/news/a73278061/california-tire-efficiency-program-niche-exemptions-for-enthusiasts/" target="_blank" rel="noopener">California tire efficiency plan carves niche exemptions</a>
        <div class="fp-meta"><span>Score 61</span><span>•</span><span>Road & Track</span></div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Suppliers & Infrastructure</h3>
      <div class="fp-row">
        <a href="https://www.electrive.com/2026/08/04/evgo-and-brixmor-to-add-more-than-500-fast-charging-stalls-in-the-us/" target="_blank" rel="noopener">EVgo & Brixmor to add 500+ US fast‑charging stalls</a>
        <div class="fp-meta"><span>Score 78</span><span>•</span><span>electrive</span></div>
      </div>
      <div class="fp-row">
        <a href="https://chargedevs.com/newswire/beam-global-supplies-ev-arc-off-grid-charging-systems-for-dallas-municipal-fleet-and-massachusetts-carshare-pilot/" target="_blank" rel="noopener">Beam Global wins Dallas and MA off‑grid charging deals</a>
        <div class="fp-meta"><span>Score 70</span><span>•</span><span>Charged EVs</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/08/03/base-power-raises-1b-to-roll-out-its-giant-new-home-battery/" target="_blank" rel="noopener">Base Power raises $1B for large home battery rollout</a>
        <div class="fp-meta"><span>Score 66</span><span>•</span><span>Electrek</span></div>
      </div>
      <div class="fp-row">
        <a href="https://chargedevs.com/newswire/mahle-introduces-a-new-range-extender-engine-and-a-rare-earth-free-electric-motor/" target="_blank" rel="noopener">MAHLE shows HD range‑extender & rare‑earth‑free motor</a>
        <div class="fp-meta"><span>Score 64</span><span>•</span><span>Charged EVs</span></div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Trending Topics</h3>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/477795/" target="_blank" rel="noopener">IEA: Global EV sales rebound 35% in Q2; 50 countries set records</a>
        <div class="fp-meta"><span>Score 80</span><span>•</span><span>Electrek</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.greencarreports.com/news/1146051_gm-pilot-ev-charging-network-now-spans-over-25-states" target="_blank" rel="noopener">GM‑Pilot EV charging network now in 25+ states</a>
        <div class="fp-meta"><span>Score 69</span><span>•</span><span>Green Car Reports</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/08/04/audis-cheapest-ev-also-most-efficient-car-all-time/" target="_blank" rel="noopener">Audi A2 e‑tron teased as brand’s most efficient car</a>
        <div class="fp-meta"><span>Score 67</span><span>•</span><span>Electrek</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.electrive.com/2026/08/04/denmark-evs-account-for-almost-all-new-car-registrations-in-july/" target="_blank" rel="noopener">Denmark: EVs hit 97% of private registrations in July</a>
        <div class="fp-meta"><span>Score 72</span><span>•</span><span>electrive</span></div>
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
        <div class="score-chip high">95</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">NHTSA opens probe into 1.2M Tesla Model 3/Y over suspension</a>
          <div class="article-take">A potential steering-control failure on high‑volume EVs could trigger one of the sector’s largest recalls.</div>
          <div class="article-tags">
            <span class="chip">Tesla</span><span class="chip">NHTSA</span><span class="chip">Safety</span><span class="chip">Recall</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 31, 2026</span>
          <a href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">81</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Volvo drops lidar on EX90/ES90, pays owners compensation</a>
          <div class="article-take">Strategic U‑turn trims BOM costs and resets Volvo’s ADAS roadmap post‑Luminar.</div>
          <div class="article-tags">
            <span class="chip">Volvo</span><span class="chip">ADAS</span><span class="chip">Suppliers</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">79</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">SK On and Factorial deepen solid‑state battery alliance</a>
          <div class="article-take">Partnership aims to accelerate manufacturability, not just lab breakthroughs, for next‑gen cells.</div>
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
        <div class="score-chip">80</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/hyundai-reveals-ioniq-3-prices-start-30000-interest-surges/" target="_blank" rel="noopener">Hyundai IONIQ 3 launches around $30k; interest surges</a>
          <div class="article-take">Aggressive pricing and >300‑mile range push mass‑market EV adoption beyond early adopters.</div>
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
        <div class="score-chip">78</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/audi-q9-suv-revealed-huge-%C2%A3100k-a8-successor" target="_blank" rel="noopener">Audi reveals Q9, a huge flagship SUV and A8 successor</a>
          <div class="article-take">Audi pivots luxury toward full‑size SUVs with tech‑heavy cabins and high-margin trims.</div>
          <div class="article-tags">
            <span class="chip">Audi</span><span class="chip">SUV</span><span class="chip">Manufacturing</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar — Jul 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/audi-q9-suv-revealed-huge-%C2%A3100k-a8-successor" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">72</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/evgo-and-brixmor-to-add-more-than-500-fast-charging-stalls-in-the-us/" target="_blank" rel="noopener">EVgo and Brixmor to add 500+ US fast‑charging stalls</a>
          <div class="article-take">Retail‑site deployments keep charging close to shopping journeys to lift utilization.</div>
          <div class="article-tags">
            <span class="chip">EVgo</span><span class="chip">Charging</span><span class="chip">Retail</span>
          </div>
        </div>
        <div class="article-source">
          <span>electrive — Aug 4, 2026</span>
          <a href="https://www.electrive.com/2026/08/04/evgo-and-brixmor-to-add-more-than-500-fast-charging-stalls-in-the-us/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">76</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/waymo-gemini-ai-ojai-robotaxi-redesigned-interface/" target="_blank" rel="noopener">Waymo integrates Gemini AI and debuts new rider interface</a>
          <div class="article-take">Conversational guidance meets AV UX — a preview of human‑machine interaction in driverless rides.</div>
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
        <div class="score-chip">73</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/04/new-porsche-boss-says-electric-718-is-still-coming-taycan-isnt-going-anywhere/" target="_blank" rel="noopener">Porsche’s new boss: electric 718 still coming; Taycan stays</a>
          <div class="article-take">Stability message calms dealers amid segment noise and evolving BEV targets.</div>
          <div class="article-tags">
            <span class="chip">Porsche</span><span class="chip">EV</span><span class="chip">Strategy</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 4, 2026</span>
          <a href="https://electrek.co/2026/08/04/new-porsche-boss-says-electric-718-is-still-coming-taycan-isnt-going-anywhere/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">72</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">BMW pauses hardcore off‑roader as it revisits product mix</a>
          <div class="article-take">Demand divergence and China exposure push BMW toward flexible, region‑led portfolios.</div>
          <div class="article-tags">
            <span class="chip">BMW</span><span class="chip">Product</span><span class="chip">China</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">70</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/30/tesla-10-millionth-vehicle-ev-growth-stalled/" target="_blank" rel="noopener">Tesla hits 10M vehicles — growth lags capacity</a>
          <div class="article-take">Production milestones matter less than demand pacing and product cadence into 2027.</div>
          <div class="article-tags">
            <span class="chip">Tesla</span><span class="chip">Production</span><span class="chip">Demand</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 30, 2026</span>
          <a href="https://electrek.co/2026/07/30/tesla-10-millionth-vehicle-ev-growth-stalled/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">69</div>
        <div class="article-main">
          <a class="headline" href="https://www.greencarreports.com/news/1146051_gm-pilot-ev-charging-network-now-spans-over-25-states" target="_blank" rel="noopener">GM‑Pilot EV fast‑charging network covers 25+ states</a>
          <div class="article-take">Legacy OEMs leverage travel centers to close interstate DCFC gaps rapidly.</div>
          <div class="article-tags">
            <span class="chip">GM</span><span class="chip">EVgo</span><span class="chip">Charging</span>
          </div>
        </div>
        <div class="article-source">
          <span>Green Car Reports — Aug 4, 2026</span>
          <a href="https://www.greencarreports.com/news/1146051_gm-pilot-ev-charging-network-now-spans-over-25-states" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">67</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/04/audis-cheapest-ev-also-most-efficient-car-all-time/" target="_blank" rel="noopener">Audi says revived A2 e‑tron will be its most efficient car</a>
          <div class="article-take">Efficiency‑first packaging returns as a competitive edge in small‑EV economics.</div>
          <div class="article-tags">
            <span class="chip">Audi</span><span class="chip">Efficiency</span><span class="chip">EV</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 4, 2026</span>
          <a href="https://electrek.co/2026/08/04/audis-cheapest-ev-also-most-efficient-car-all-time/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">72</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/denmark-evs-account-for-almost-all-new-car-registrations-in-july/" target="_blank" rel="noopener">Denmark: EVs reach 97% of private registrations in July</a>
          <div class="article-take">Nordic policy alignment continues to showcase what rapid electrification can look like.</div>
          <div class="article-tags">
            <span class="chip">Denmark</span><span class="chip">EV adoption</span><span class="chip">Policy</span>
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
          <a class="headline" href="https://www.carscoops.com/2026/08/china-autonomous-light-ban/" target="_blank" rel="noopener">China bans turquoise autonomous driving lights</a>
          <div class="article-take">Standardized signaling in AVs inches forward while retrofits face regulatory gray areas.</div>
          <div class="article-tags">
            <span class="chip">China</span><span class="chip">AV</span><span class="chip">Regulation</span>
          </div>
        </div>
        <div class="article-source">
          <span>Carscoops — Aug 4, 2026</span>
          <a href="https://www.carscoops.com/2026/08/china-autonomous-light-ban/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">66</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/03/base-power-raises-1b-to-roll-out-its-giant-new-home-battery/" target="_blank" rel="noopener">Base Power raises $1B to deploy 39.2‑kWh home battery</a>
          <div class="article-take">Bigger residential storage targets resilience and load‑shifting for EV households.</div>
          <div class="article-tags">
            <span class="chip">Energy storage</span><span class="chip">Home</span><span class="chip">Grid</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 3, 2026</span>
          <a href="https://electrek.co/2026/08/03/base-power-raises-1b-to-roll-out-its-giant-new-home-battery/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">70</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/30/rivian-rivn-q2-2026-earnings-r2-deliveries-revenue-up-27/" target="_blank" rel="noopener">Rivian Q2: revenue +27% YoY, record gross profit</a>
          <div class="article-take">R2 deliveries give Rivian leverage to scale while improving unit economics.</div>
          <div class="article-tags">
            <span class="chip">Rivian</span><span class="chip">Earnings</span><span class="chip">EV</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 30, 2026</span>
          <a href="https://electrek.co/2026/07/30/rivian-rivn-q2-2026-earnings-r2-deliveries-revenue-up-27/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">65</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/philippines-launches-e850m-incentive-programme-for-ev-manufacturing/" target="_blank" rel="noopener">Philippines unveils €850m EV manufacturing incentives</a>
          <div class="article-take">Southeast Asia intensifies competition for capex with targeted EV packages.</div>
          <div class="article-tags">
            <span class="chip">Philippines</span><span class="chip">Investment</span><span class="chip">Manufacturing</span>
          </div>
        </div>
        <div class="article-source">
          <span>electrive — Aug 4, 2026</span>
          <a href="https://www.electrive.com/2026/08/04/philippines-launches-e850m-incentive-programme-for-ev-manufacturing/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">63</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/31/byd-undercuts-defender-first-7-seat-suv-uk/" target="_blank" rel="noopener">BYD brings boxy, seven‑seat Ti 7 SUV to the UK</a>
          <div class="article-take">Value‑priced family hauler expands BYD’s European footprint with rugged styling.</div>
          <div class="article-tags">
            <span class="chip">BYD</span><span class="chip">SUV</span><span class="chip">UK market</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 31, 2026</span>
          <a href="https://electrek.co/2026/07/31/byd-undercuts-defender-first-7-seat-suv-uk/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">61</div>
        <div class="article-main">
          <a class="headline" href="https://www.roadandtrack.com/news/a73278061/california-tire-efficiency-program-niche-exemptions-for-enthusiasts/" target="_blank" rel="noopener">California tire efficiency plan adds enthusiast exemptions</a>
          <div class="article-take">Regulators balance efficiency targets with motorsport and off‑road niches.</div>
          <div class="article-tags">
            <span class="chip">California</span><span class="chip">Policy</span><span class="chip">Tires</span>
          </div>
        </div>
        <div class="article-source">
          <span>Road & Track — Jul 2026</span>
          <a href="https://www.roadandtrack.com/news/a73278061/california-tire-efficiency-program-niche-exemptions-for-enthusiasts/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">62</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/waymo-gemini-ai-ojai-robotaxi-redesigned-interface/" target="_blank" rel="noopener">Waymo Ojai robotaxi readies for broader public access</a>
          <div class="article-take">New UX aims to reduce rider friction as service scales beyond early pilots.</div>
          <div class="article-tags">
            <span class="chip">Waymo</span><span class="chip">Mobility</span><span class="chip">AV</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/waymo-gemini-ai-ojai-robotaxi-redesigned-interface/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">60</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/blue-solutions-and-avl-test-solid-state-battery-safety/" target="_blank" rel="noopener">Blue Solutions & AVL validate solid‑state safety behaviors</a>
          <div class="article-take">Thermal propagation management advances move solid‑state closer to series readiness.</div>
          <div class="article-tags">
            <span class="chip">Blue Solutions</span><span class="chip">AVL</span><span class="chip">Battery safety</span>
          </div>
        </div>
        <div class="article-source">
          <span>electrive — Aug 4, 2026</span>
          <a href="https://www.electrive.com/2026/08/04/blue-solutions-and-avl-test-solid-state-battery-safety/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">64</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/mercedes-big-screens-stay-we-went-too-far-removing-buttons" target="_blank" rel="noopener">Mercedes: screens stay, but buttons return where sensible</a>
          <div class="article-take">Tactile controls creep back as OEMs recalibrate in‑car UX for safety and ease.</div>
          <div class="article-tags">
            <span class="chip">Mercedes-Benz</span><span class="chip">UX</span><span class="chip">HMI</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/mercedes-big-screens-stay-we-went-too-far-removing-buttons" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">63</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/04/hyundai-confirms-ioniq-6-n-on-track-launch-us/" target="_blank" rel="noopener">Hyundai confirms IONIQ 6 N is still US‑bound this year</a>
          <div class="article-take">Performance halo bolsters brand credibility as affordable EVs expand.</div>
          <div class="article-tags">
            <span class="chip">Hyundai</span><span class="chip">Performance</span><span class="chip">EV</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 4, 2026</span>
          <a href="https://electrek.co/2026/08/04/hyundai-confirms-ioniq-6-n-on-track-launch-us/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">62</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/03/nice-opens-former-mobilize-share-charging-network-to-public/" target="_blank" rel="noopener">Nice reopens former Mobilize Share chargers to the public</a>
          <div class="article-take">Repurposing legacy car‑share bays adds near‑term kerbside charge access.</div>
          <div class="article-tags">
            <span class="chip">Charging</span><span class="chip">France</span><span class="chip">Infrastructure</span>
          </div>
        </div>
        <div class="article-source">
          <span>electrive — Aug 3, 2026</span>
          <a href="https://www.electrive.com/2026/08/03/nice-opens-former-mobilize-share-charging-network-to-public/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">61</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/30/a-new-zipcar-pilot-pairs-shared-evs-with-off-grid-solar-charging/" target="_blank" rel="noopener">Zipcar pilots shared EVs with off‑grid solar chargers</a>
          <div class="article-take">Pairing car‑share with standalone charging unlocks underserved neighborhoods.</div>
          <div class="article-tags">
            <span class="chip">Mobility</span><span class="chip">Charging</span><span class="chip">Solar</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 30, 2026</span>
          <a href="https://electrek.co/2026/07/30/a-new-zipcar-pilot-pairs-shared-evs-with-off-grid-solar-charging/" target="_blank" rel="noopener">Read original →</a>
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
    <h2 class="section-title">Industry News <span class="count">Curated highlights</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip high">95</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">NHTSA opens probe into 1.2M Teslas for suspension failures</a>
          <div class="article-take">Large‑scale safety review could reshape EV chassis validation norms.</div>
          <div class="article-tags">
            <span class="chip">Safety</span><span class="chip">Regulation</span><span class="chip">Tesla</span>
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
          <a class="headline" href="https://electrek.co/2026/07/29/477795/" target="_blank" rel="noopener">IEA: Global EV sales jump 35% in Q2, 50 countries set records</a>
          <div class="article-take">Momentum resumed after a soft start to the year, led by value EVs and hybrids.</div>
          <div class="article-tags">
            <span class="chip">Sales</span><span class="chip">IEA</span><span class="chip">EV adoption</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/477795/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">72</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/mercedes-big-screens-stay-we-went-too-far-removing-buttons" target="_blank" rel="noopener">Mercedes to reintroduce key physical buttons alongside big screens</a>
          <div class="article-take">Automakers recalibrate UX to cut distraction while keeping software features front‑and‑center.</div>
          <div class="article-tags">
            <span class="chip">UX</span><span class="chip">HMI</span><span class="chip">Mercedes-Benz</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/mercedes-big-screens-stay-we-went-too-far-removing-buttons" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="electric-vehicles">
    <h2 class="section-title">Electric Vehicles <span class="count">Market & models</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip">80</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/hyundai-reveals-ioniq-3-prices-start-30000-interest-surges/" target="_blank" rel="noopener">Hyundai’s $30k IONIQ 3 looks like a mass‑market hit</a>
          <div class="article-take">Value plus range expands EV addressable market beyond early adopters.</div>
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
        <div class="score-chip">73</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/04/new-porsche-boss-says-electric-718-is-still-coming-taycan-isnt-going-anywhere/" target="_blank" rel="noopener">Porsche reaffirms electric 718 program</a>
          <div class="article-take">Performance EV roadmap stays intact despite segment volatility.</div>
          <div class="article-tags">
            <span class="chip">Porsche</span><span class="chip">Sports EV</span><span class="chip">Strategy</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 4, 2026</span>
          <a href="https://electrek.co/2026/08/04/new-porsche-boss-says-electric-718-is-still-coming-taycan-isnt-going-anywhere/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">67</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/04/audis-cheapest-ev-also-most-efficient-car-all-time/" target="_blank" rel="noopener">Audi A2 e‑tron targets best‑ever efficiency</a>
          <div class="article-take">Efficiency arms race heats up as small EVs chase profitability.</div>
          <div class="article-tags">
            <span class="chip">Audi</span><span class="chip">Efficiency</span><span class="chip">EV Tech</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 4, 2026</span>
          <a href="https://electrek.co/2026/08/04/audis-cheapest-ev-also-most-efficient-car-all-time/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="manufacturers">
    <h2 class="section-title">Manufacturers <span class="count">Strategy & product</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip">78</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/audi-q9-suv-revealed-huge-%C2%A3100k-a8-successor" target="_blank" rel="noopener">Audi debuts Q9 flagship SUV</a>
          <div class="article-take">Upsizing luxury portfolio to meet US and Gulf demand where margins are highest.</div>
          <div class="article-tags">
            <span class="chip">Audi</span><span class="chip">SUV</span><span class="chip">Luxury</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar — Jul 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/audi-q9-suv-revealed-huge-%C2%A3100k-a8-successor" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">72</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">BMW rethinks product slate amid China slowdown</a>
          <div class="article-take">Portfolio flexibility beats one‑size‑fits‑all in diverging global markets.</div>
          <div class="article-tags">
            <span class="chip">BMW</span><span class="chip">China</span><span class="chip">Planning</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">63</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/31/byd-undercuts-defender-first-7-seat-suv-uk/" target="_blank" rel="noopener">BYD’s seven‑seat Ti 7 expands UK lineup</a>
          <div class="article-take">Aggressive pricing pressures incumbents in family SUV segments.</div>
          <div class="article-tags">
            <span class="chip">BYD</span><span class="chip">UK</span><span class="chip">Competition</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 31, 2026</span>
          <a href="https://electrek.co/2026/07/31/byd-undercuts-defender-first-7-seat-suv-uk/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="dealers">
    <h2 class="section-title">Dealers <span class="count">Retail & networks</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip">62</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/30/a-new-zipcar-pilot-pairs-shared-evs-with-off-grid-solar-charging/" target="_blank" rel="noopener">Zipcar pilots EV car‑share with off‑grid chargers</a>
          <div class="article-take">Community deployments create new EV trial funnels where dealers have no presence.</div>
          <div class="article-tags">
            <span class="chip">Mobility</span><span class="chip">Retail</span><span class="chip">Charging</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 30, 2026</span>
          <a href="https://electrek.co/2026/07/30/a-new-zipcar-pilot-pairs-shared-evs-with-off-grid-solar-charging/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">69</div>
        <div class="article-main">
          <a class="headline" href="https://www.greencarreports.com/news/1146051_gm-pilot-ev-charging-network-now-spans-over-25-states" target="_blank" rel="noopener">GM‑Pilot’s charging footprint boosts road‑trip confidence</a>
          <div class="article-take">More highway DCFC reduces buyer objections dealers face at point of sale.</div>
          <div class="article-tags">
            <span class="chip">Charging</span><span class="chip">GM</span><span class="chip">Retail</span>
          </div>
        </div>
        <div class="article-source">
          <span>Green Car Reports — Aug 4, 2026</span>
          <a href="https://www.greencarreports.com/news/1146051_gm-pilot-ev-charging-network-now-spans-over-25-states" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="suppliers">
    <h2 class="section-title">Suppliers <span class="count">Ecosystem moves</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip">79</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">SK On and Factorial: scaling solid‑state to mass market</a>
          <div class="article-take">Joint work concentrates on manufacturability and supply risk over lab demos.</div>
          <div class="article-tags">
            <span class="chip">Batteries</span><span class="chip">Partnership</span><span class="chip">Technology</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">70</div>
        <div class="article-main">
          <a class="headline" href="https://chargedevs.com/newswire/beam-global-supplies-ev-arc-off-grid-charging-systems-for-dallas-municipal-fleet-and-massachusetts-carshare-pilot/" target="_blank" rel="noopener">Beam Global expands off‑grid EV ARC deployments</a>
          <div class="article-take">Construction‑free chargers speed time‑to‑charge for fleets and pilots.</div>
          <div class="article-tags">
            <span class="chip">Infrastructure</span><span class="chip">Off‑grid</span><span class="chip">Municipal</span>
          </div>
        </div>
        <div class="article-source">
          <span>Charged EVs — Aug 1, 2026</span>
          <a href="https://chargedevs.com/newswire/beam-global-supplies-ev-arc-off-grid-charging-systems-for-dallas-municipal-fleet-and-massachusetts-carshare-pilot/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">64</div>
        <div class="article-main">
          <a class="headline" href="https://chargedevs.com/newswire/mahle-introduces-a-new-range-extender-engine-and-a-rare-earth-free-electric-motor/" target="_blank" rel="noopener">MAHLE unveils HD range‑extender and rare‑earth‑free motor</a>
          <div class="article-take">Hybridized heavies and motor material shifts reshape supplier roadmaps.</div>
          <div class="article-tags">
            <span class="chip">MAHLE</span><span class="chip">Powertrain</span><span class="chip">Supply chain</span>
          </div>
        </div>
        <div class="article-source">
          <span>Charged EVs — Aug 1, 2026</span>
          <a href="https://chargedevs.com/newswire/mahle-introduces-a-new-range-extender-engine-and-a-rare-earth-free-electric-motor/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="government">
    <h2 class="section-title">Government <span class="count">Regulation & policy</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip high">95</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">NHTSA opens probe into Tesla suspension failures</a>
          <div class="article-take">Large‑scale safety oversight sharpens EV scrutiny.</div>
          <div class="article-tags">
            <span class="chip">NHTSA</span><span class="chip">Safety</span><span class="chip">Tesla</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 31, 2026</span>
          <a href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">65</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/philippines-launches-e850m-incentive-programme-for-ev-manufacturing/" target="_blank" rel="noopener">Philippines launches major EV manufacturing incentives</a>
          <div class="article-take">New ASEAN node emerges for cost‑competitive EV production.</div>
          <div class="article-tags">
            <span class="chip">Policy</span><span class="chip">Manufacturing</span><span class="chip">ASEAN</span>
          </div>
        </div>
        <div class="article-source">
          <span>electrive — Aug 4, 2026</span>
          <a href="https://www.electrive.com/2026/08/04/philippines-launches-e850m-incentive-programme-for-ev-manufacturing/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">68</div>
        <div class="article-main">
          <a class="headline" href="https://www.carscoops.com/2026/08/china-autonomous-light-ban/" target="_blank" rel="noopener">China bans turquoise AV lights, clarifies signaling</a>
          <div class="article-take">Standardization reduces consumer confusion as AV pilots expand.</div>
          <div class="article-tags">
            <span class="chip">China</span><span class="chip">AV</span><span class="chip">Standards</span>
          </div>
        </div>
        <div class="article-source">
          <span>Carscoops — Aug 4, 2026</span>
          <a href="https://www.carscoops.com/2026/08/china-autonomous-light-ban/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="technology">
    <h2 class="section-title">Technology <span class="count">Software & hardware</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip">81</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Volvo drops lidar and compensates customers</a>
          <div class="article-take">OEMs reassess sensor stacks as cost, value and timing collide.</div>
          <div class="article-tags">
            <span class="chip">ADAS</span><span class="chip">Sensors</span><span class="chip">Volvo</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">79</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">Solid‑state battery alliance ramps up</a>
          <div class="article-take">Focus shifts from chemistry to yield, safety and supply readiness.</div>
          <div class="article-tags">
            <span class="chip">Battery</span><span class="chip">Solid‑state</span><span class="chip">Scale‑up</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">75</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/04/waymo-co-ceo-camera-only-self-driving-tesla/" target="_blank" rel="noopener">Waymo CEO outlines limits of camera‑only autonomy</a>
          <div class="article-take">Sensor redundancy and perception fidelity remain essential for higher safety bars.</div>
          <div class="article-tags">
            <span class="chip">Autonomous</span><span class="chip">Safety</span><span class="chip">Sensors</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 4, 2026</span>
          <a href="https://electrek.co/2026/08/04/waymo-co-ceo-camera-only-self-driving-tesla/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="finance">
    <h2 class="section-title">Finance <span class="count">Earnings & capital</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip">70</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/30/rivian-rivn-q2-2026-earnings-r2-deliveries-revenue-up-27/" target="_blank" rel="noopener">Rivian beats on Q2 as R2 deliveries begin</a>
          <div class="article-take">Improving gross margin suggests a credible path to scale.</div>
          <div class="article-tags">
            <span class="chip">Rivian</span><span class="chip">Earnings</span><span class="chip">Scaling</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 30, 2026</span>
          <a href="https://electrek.co/2026/07/30/rivian-rivn-q2-2026-earnings-r2-deliveries-revenue-up-27/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">66</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/03/base-power-raises-1b-to-roll-out-its-giant-new-home-battery/" target="_blank" rel="noopener">Base Power raises $1B for home energy storage</a>
          <div class="article-take">Capital flows to resilience‑oriented, EV‑adjacent home upgrades.</div>
          <div class="article-tags">
            <span class="chip">Storage</span><span class="chip">Fundraising</span><span class="chip">Home energy</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 3, 2026</span>
          <a href="https://electrek.co/2026/08/03/base-power-raises-1b-to-roll-out-its-giant-new-home-battery/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="international">
    <h2 class="section-title">International <span class="count">Global shifts</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip">72</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/denmark-evs-account-for-almost-all-new-car-registrations-in-july/" target="_blank" rel="noopener">Denmark: EVs are virtually all new private registrations</a>
          <div class="article-take">Nordic policies continue to set the global pace.</div>
          <div class="article-tags">
            <span class="chip">Denmark</span><span class="chip">EV policy</span><span class="chip">Adoption</span>
          </div>
        </div>
        <div class="article-source">
          <span>electrive — Aug 4, 2026</span>
          <a href="https://www.electrive.com/2026/08/04/denmark-evs-account-for-almost-all-new-car-registrations-in-july/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">65</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/philippines-launches-e850m-incentive-programme-for-ev-manufacturing/" target="_blank" rel="noopener">Philippines bids for EV manufacturing with €850m plan</a>
          <div class="article-take">Regional competition for EV supply chains intensifies.</div>
          <div class="article-tags">
            <span class="chip">ASEAN</span><span class="chip">Manufacturing</span><span class="chip">Incentives</span>
          </div>
        </div>
        <div class="article-source">
          <span>electrive — Aug 4, 2026</span>
          <a href="https://www.electrive.com/2026/08/04/philippines-launches-e850m-incentive-programme-for-ev-manufacturing/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="opinion">
    <h2 class="section-title">Opinion <span class="count">Analysis & columns</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip">64</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/mercedes-big-screens-stay-we-went-too-far-removing-buttons" target="_blank" rel="noopener">Mercedes: we went “too far” removing buttons</a>
          <div class="article-take">Pragmatic UI is back — and drivers will notice.</div>
          <div class="article-tags">
            <span class="chip">Opinion</span><span class="chip">UX</span><span class="chip">Safety</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/mercedes-big-screens-stay-we-went-too-far-removing-buttons" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">61</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/opinion/new-cars/ignore-jay-leno-your-dream-garage-only-needs-three-cars" target="_blank" rel="noopener">Ignore Jay Leno: you only need three cars</a>
          <div class="article-take">A minimalist take on enthusiast ownership in a software‑defined era.</div>
          <div class="article-tags">
            <span class="chip">Opinion</span><span class="chip">Culture</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 2026</span>
          <a href="https://www.autocar.co.uk/opinion/new-cars/ignore-jay-leno-your-dream-garage-only-needs-three-cars" target="_blank" rel="noopener">Read original →</a>
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