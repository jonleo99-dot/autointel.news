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
        <h1>NHTSA opens probe into 1.2 million Tesla Model 3/Y over suspension failures</h1>
        <p class="exec-summary">US safety regulators launched a sweeping investigation into 2018–2023 Model 3 and Model Y front-suspension link separations after more than 150 complaints. The case puts Tesla’s quality systems and field fixes under the microscope at a time when the automaker faces rising scrutiny of Autopilot and cost-driven design changes. Outcomes could include recalls, supplier rework, and tighter validation for new platforms — with ripple effects across EV competitors benchmarking Tesla’s speed-to-market.</p>

        <div class="takeaways">
          <h3>Key Takeaways</h3>
          <ul>
            <li>Scope covers ~1.2M US vehicles; findings may trigger large-scale recall actions or repair campaigns.</li>
            <li>Focus on lateral link separations highlights fatigue and assembly-quality risks during rapid cost-down cycles.</li>
            <li>Investigation outcome could influence regulators’ posture toward emerging EV players rushing new designs.</li>
          </ul>
        </div>

        <div class="impact-row">
          <div class="impact-block">
            <h4>Industry Impact</h4>
            <p>Heightened safety scrutiny raises compliance costs across the EV sector. If NHTSA mandates redesigns or extended warranties, Tesla’s margin recovery plan will face pressure, while suppliers may shoulder rework and liability. Expect peers to recalibrate validation gates and fast-track part durability analytics to avoid similar exposure.</p>
          </div>
          <div class="impact-block">
            <h4>Companies Affected</h4>
            <div class="chip-row">
              <span class="chip entity-mfr">Tesla</span>
              <span class="chip entity-mfr">NHTSA</span>
            </div>
          </div>
        </div>

        <div class="source-strip">
          <span>Source: <b>Electrek</b></span>
          <span>Today</span>
          <a href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">Read original →</a>
        </div>

        <div class="related">
          <h4>Related Coverage</h4>
          <ul>
            <li><a href="https://www.electrive.com/2026/08/03/nhtsa-opens-probe-into-1-2-million-teslas/" target="_blank" rel="noopener">NHTSA opens probe into 1.2 million Teslas</a></li>
            <li><a href="https://electrek.co/2026/08/03/tesla-fsd-v14-lite-hw3-computer-failures/" target="_blank" rel="noopener">Tesla FSD v14 Lite tied to rising HW3 computer failures, owners report</a></li>
            <li><a href="https://electrek.co/2026/07/28/tesla-sues-cybertruck-supplier-angstrom-tooling/" target="_blank" rel="noopener">Tesla sues Cybertruck supplier amid standoff keeping production hostage</a></li>
          </ul>
        </div>
      </div>

      <div class="hero-gauges">
        <div class="gauge">
          <svg viewBox="0 0 120 70"><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#2a3038" stroke-width="8"/><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#f2a93b" stroke-width="8" stroke-dasharray="157" stroke-dashoffset="12.6"/></svg>
          <span class="gauge-value mono">92</span>
          <span class="gauge-label">Importance</span>
        </div>
        <div class="gauge">
          <svg viewBox="0 0 120 70"><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#2a3038" stroke-width="8"/><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#3ecf8e" stroke-width="8" stroke-dasharray="157" stroke-dashoffset="18.84"/></svg>
          <span class="gauge-value mono">88</span>
          <span class="gauge-label">Editorial Quality</span>
        </div>
        <div class="gauge">
          <svg viewBox="0 0 120 70"><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#2a3038" stroke-width="8"/><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#e2604f" stroke-width="8" stroke-dasharray="157" stroke-dashoffset="15.7"/></svg>
          <span class="gauge-value mono">90</span>
          <span class="gauge-label">Industry Impact</span>
        </div>
        <div class="gauge">
          <svg viewBox="0 0 120 70"><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#2a3038" stroke-width="8"/><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#f2a93b" stroke-width="8" stroke-dasharray="157" stroke-dashoffset="23.55"/></svg>
          <span class="gauge-value mono">85</span>
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
    <h2 class="section-title">Industry Snapshot <span class="count">Today</span></h2>
    <div class="dash-grid">
      <div class="stat-panel">
        <h4>Top Manufacturers</h4>
        <ul class="rank-list">
          <li><span>Tesla</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:100%"></div></div><span class="rank-count">12</span></li>
          <li><span>BYD</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:83%"></div></div><span class="rank-count">10</span></li>
          <li><span>Hyundai</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:67%"></div></div><span class="rank-count">8</span></li>
          <li><span>BMW</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:58%"></div></div><span class="rank-count">7</span></li>
          <li><span>Audi</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:58%"></div></div><span class="rank-count">7</span></li>
          <li><span>Mercedes-Benz</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:58%"></div></div><span class="rank-count">7</span></li>
          <li><span>Rivian</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:50%"></div></div><span class="rank-count">6</span></li>
          <li><span>Volvo</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:42%"></div></div><span class="rank-count">5</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4>Top Brands</h4>
        <ul class="rank-list">
          <li><span>Genesis</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:80%"></div></div><span class="rank-count">8</span></li>
          <li><span>Kia</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:70%"></div></div><span class="rank-count">7</span></li>
          <li><span>Porsche</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:60%"></div></div><span class="rank-count">6</span></li>
          <li><span>Volkswagen</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:55%"></div></div><span class="rank-count">5</span></li>
          <li><span>Ford</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:45%"></div></div><span class="rank-count">4</span></li>
          <li><span>Ram</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:40%"></div></div><span class="rank-count">4</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4>Top Suppliers</h4>
        <ul class="rank-list">
          <li><span>EVgo</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:100%"></div></div><span class="rank-count">6</span></li>
          <li><span>Allego</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:83%"></div></div><span class="rank-count">5</span></li>
          <li><span>Beam Global</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:83%"></div></div><span class="rank-count">5</span></li>
          <li><span>MAHLE</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:67%"></div></div><span class="rank-count">4</span></li>
          <li><span>char.gy</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:50%"></div></div><span class="rank-count">3</span></li>
          <li><span>Wenea</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:33%"></div></div><span class="rank-count">2</span></li>
          <li><span>Mouser</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:33%"></div></div><span class="rank-count">2</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4>Most Mentioned Executives</h4>
        <ul class="rank-list">
          <li><span>Elon Musk (Tesla)</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:100%"></div></div><span class="rank-count">9</span></li>
          <li><span>RJ Scaringe (Rivian)</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:67%"></div></div><span class="rank-count">6</span></li>
          <li><span>Ola Källenius (Mercedes)</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:56%"></div></div><span class="rank-count">5</span></li>
          <li><span>Dmitri Dolgov (Waymo)</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:44%"></div></div><span class="rank-count">4</span></li>
          <li><span>Michael Leiters (Porsche)</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:33%"></div></div><span class="rank-count">3</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4>Trending Topics</h4>
        <div class="tagcloud">
          <span class="chip lg">Safety probes</span>
          <span class="chip">Charging build‑out</span>
          <span class="chip">Solid‑state batteries</span>
          <span class="chip">Lidar strategy</span>
          <span class="chip">EV demand rebound</span>
          <span class="chip">China exports</span>
          <span class="chip">Affordable EVs</span>
          <span class="chip">Robotaxis</span>
        </div>
      </div>

      <div class="stat-panel">
        <h4>Emerging Technologies</h4>
        <div class="tagcloud">
          <span class="chip lg">Iron‑air storage</span>
          <span class="chip">Sulfur‑crystal cells</span>
          <span class="chip">SDV platforms</span>
          <span class="chip">AI assistants in AVs</span>
          <span class="chip">800V architectures</span>
          <span class="chip">Virtual power plants</span>
        </div>
      </div>

      <div class="stat-panel">
        <h4>Government Activity</h4>
        <div class="tagcloud">
          <span class="chip lg">NHTSA suspension probe</span>
          <span class="chip">Denmark 97.6% EV share</span>
          <span class="chip">Philippines EV incentives</span>
          <span class="chip">UK EV grant updates</span>
          <span class="chip">Tariff/tax credit shifts</span>
        </div>
      </div>

      <div class="stat-panel">
        <h4>Supplier Activity</h4>
        <div class="tagcloud">
          <span class="chip lg">EVgo + Brixmor DCFC</span>
          <span class="chip">Allego UK investment</span>
          <span class="chip">Beam off‑grid pilots</span>
          <span class="chip">MAHLE range extender</span>
          <span class="chip">Teletrac energy analytics</span>
        </div>
      </div>

      <div class="stat-panel">
        <h4>Financial Activity</h4>
        <ul class="rank-list">
          <li><span>Rivian beats on Q2</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:100%"></div></div><span class="rank-count">A</span></li>
          <li><span>BYD July sales +22%</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:83%"></div></div><span class="rank-count">B</span></li>
          <li><span>Lucid stake disclosure</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:67%"></div></div><span class="rank-count">C</span></li>
          <li><span>Tesla China mix shift</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:67%"></div></div><span class="rank-count">C</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4>Global Regions</h4>
        <ul class="rank-list">
          <li><span>United States</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:100%"></div></div><span class="rank-count">12</span></li>
          <li><span>China</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:83%"></div></div><span class="rank-count">10</span></li>
          <li><span>United Kingdom</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:58%"></div></div><span class="rank-count">7</span></li>
          <li><span>EU (Rest of Europe)</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:58%"></div></div><span class="rank-count">7</span></li>
          <li><span>Nordics</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:42%"></div></div><span class="rank-count">5</span></li>
          <li><span>Mexico/Canada</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:33%"></div></div><span class="rank-count">4</span></li>
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
        <a href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">BMW puts G‑Class rival on hold as China headwinds hit home</a>
        <div class="fp-meta"><span>Score 78</span><span>Autocar</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/new-mercedes-gla-ev-bigger-400-miles-range/" target="_blank" rel="noopener">Mercedes debuts GLA EV with claimed 400+ mile range</a>
        <div class="fp-meta"><span>Score 82</span><span>Electrek</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/30/rivian-rivn-q2-2026-earnings-r2-deliveries-revenue-up-27/" target="_blank" rel="noopener">Rivian Q2: revenue up 27% and gross profit turns positive</a>
        <div class="fp-meta"><span>Score 81</span><span>Electrek</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.autocar.co.uk/car-news/new-cars/byd-goes-after-defender-boxy-%C2%A348k-402bhp-hybrid-suv" target="_blank" rel="noopener">BYD launches Ti7 in UK to undercut Defender with PHEV punch</a>
        <div class="fp-meta"><span>Score 77</span><span>Autocar</span></div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Technology</h3>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">SK On and Factorial team up to scale solid‑state batteries</a>
        <div class="fp-meta"><span>Score 80</span><span>Electrek</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/waymo-gemini-ai-ojai-robotaxi-redesigned-interface/" target="_blank" rel="noopener">Waymo adds Gemini assistant and new UI to robotaxi</a>
        <div class="fp-meta"><span>Score 78</span><span>Electrek</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.autocar.co.uk/car-news/new-cars/reborn-audi-a2-driven-electric-comeback-efficiency-king" target="_blank" rel="noopener">Audi A2 e‑tron returns as ultra‑efficient compact EV</a>
        <div class="fp-meta"><span>Score 79</span><span>Autocar</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.greencarreports.com/news/1146043_sulfur-crystal-battery-could-triple-ev-range-without-cobalt-or-nickel" target="_blank" rel="noopener">Startup touts sulfur‑crystal battery with 3× energy density</a>
        <div class="fp-meta"><span>Score 74</span><span>Green Car Reports</span></div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Government & Policy</h3>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">NHTSA opens probe into 1.2M Teslas over suspension failures</a>
        <div class="fp-meta"><span>Score 92</span><span>Electrek</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.electrive.com/2026/08/03/denmark-evs-account-for-almost-all-new-car-registrations-in-july/" target="_blank" rel="noopener">Denmark hits 97.6% EV share in July registrations</a>
        <div class="fp-meta"><span>Score 76</span><span>electrive</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.electrive.com/2026/08/04/philippines-launches-e850m-incentive-programme-for-ev-manufacturing/" target="_blank" rel="noopener">Philippines launches €850m incentives to attract EV manufacturing</a>
        <div class="fp-meta"><span>Score 73</span><span>electrive</span></div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Suppliers & Infrastructure</h3>
      <div class="fp-row">
        <a href="https://www.electrive.com/2026/08/04/evgo-and-brixmor-to-add-more-than-500-fast-charging-stalls-in-the-us/" target="_blank" rel="noopener">EVgo, Brixmor to add 500+ DC fast‑charging stalls in US</a>
        <div class="fp-meta"><span>Score 74</span><span>electrive</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.electrive.com/2026/08/01/allego-commits-e100-million-to-expand-uk-charging-network/" target="_blank" rel="noopener">Allego invests €100m to expand UK ultra‑rapid charging</a>
        <div class="fp-meta"><span>Score 72</span><span>electrive</span></div>
      </div>
      <div class="fp-row">
        <a href="https://chargedevs.com/newswire/beam-global-supplies-ev-arc-off-grid-charging-systems-for-dallas-municipal-fleet-and-massachusetts-carshare-pilot/" target="_blank" rel="noopener">Beam Global adds off‑grid EV ARC systems for fleets and carshare</a>
        <div class="fp-meta"><span>Score 70</span><span>Charged EVs</span></div>
      </div>
      <div class="fp-row">
        <a href="https://chargedevs.com/newswire/mahle-introduces-a-new-range-extender-engine-and-a-rare-earth-free-electric-motor/" target="_blank" rel="noopener">MAHLE unveils truck range‑extender and rare‑earth‑free motor</a>
        <div class="fp-meta"><span>Score 71</span><span>Charged EVs</span></div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Trending Topics</h3>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/477795/" target="_blank" rel="noopener">IEA: Global EV sales rebounded 35% in Q2; 50 countries set records</a>
        <div class="fp-meta"><span>Score 84</span><span>Electrek</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Volvo drops lidar on EX90/ES90 and compensates owners</a>
        <div class="fp-meta"><span>Score 86</span><span>Electrek</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.greencarreports.com/news/1146052_here-are-the-evs-made-in-mexico-and-canada" target="_blank" rel="noopener">Which EVs are built in Mexico and Canada amid tariff shifts?</a>
        <div class="fp-meta"><span>Score 73</span><span>Green Car Reports</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/08/04/volvos-next-electric-suv-will-start-in-the-upper-40000-range/" target="_blank" rel="noopener">Volvo preps entry EX50 to target Model Y price band</a>
        <div class="fp-meta"><span>Score 74</span><span>Electrek</span></div>
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
    <h2 class="section-title">Latest Articles <span class="count">24 analyzed today</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip high">92</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">NHTSA opens probe into 1.2M Tesla Model 3/Y over suspension failures</a>
          <div class="article-take">A widescale US safety investigation could force redesigns and recalls, raising quality costs for Tesla and peers.</div>
          <div class="article-tags">
            <span class="chip">Tesla</span><span class="chip">NHTSA</span><span class="chip">Safety</span><span class="chip">Recall</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek</span>
          <span>Today</span>
          <a href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip high">86</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Volvo drops lidar for good on EX90 and ES90, pays owner compensation</a>
          <div class="article-take">Backing away from lidar resets Volvo’s ADAS roadmap and ripples through supplier plans after the Luminar split.</div>
          <div class="article-tags">
            <span class="chip">Volvo</span><span class="chip">ADAS</span><span class="chip">Lidar</span><span class="chip">Suppliers</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek</span>
          <span>Today</span>
          <a href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">82</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/new-mercedes-gla-ev-bigger-400-miles-range/" target="_blank" rel="noopener">The new Mercedes GLA EV is bigger, smarter, and has a range of over 400 miles</a>
          <div class="article-take">Mercedes pushes its compact EV upmarket with 800V tech and long-range trims to fend off Audi and Volvo rivals.</div>
          <div class="article-tags">
            <span class="chip">Mercedes-Benz</span><span class="chip">EV</span><span class="chip">Manufacturing</span><span class="chip">Product</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek</span>
          <span>Today</span>
          <a href="https://electrek.co/2026/07/29/new-mercedes-gla-ev-bigger-400-miles-range/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">84</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/477795/" target="_blank" rel="noopener">IEA: Global EV sales jump 35% in Q2 and 50 countries set records</a>
          <div class="article-take">Demand momentum returned broadly in Q2, bolstering OEM volume plans and charging rollout assumptions.</div>
          <div class="article-tags">
            <span class="chip">EV</span><span class="chip">Markets</span><span class="chip">Finance</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek</span>
          <span>Today</span>
          <a href="https://electrek.co/2026/07/29/477795/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">83</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/04/tesla-china-sales-crash-exports-surge-h1-2026/" target="_blank" rel="noopener">Tesla China sales are crashing as exports surge</a>
          <div class="article-take">Shanghai is shifting from local demand to export hub, signaling competitive pressure in China and mix risk for margins.</div>
          <div class="article-tags">
            <span class="chip">Tesla</span><span class="chip">China</span><span class="chip">Trade</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek</span>
          <span>Today</span>
          <a href="https://electrek.co/2026/08/04/tesla-china-sales-crash-exports-surge-h1-2026/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">79</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/reborn-audi-a2-driven-electric-comeback-efficiency-king" target="_blank" rel="noopener">Reborn Audi A2 driven: Electric comeback for the efficiency king</a>
          <div class="article-take">Audi leans into aero and LFP packs to chase best‑in‑class efficiency below Q4 e‑tron pricing.</div>
          <div class="article-tags">
            <span class="chip">Audi</span><span class="chip">Efficiency</span><span class="chip">EV</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar</span>
          <span>Today</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/reborn-audi-a2-driven-electric-comeback-efficiency-king" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">80</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">Two solid-state EV battery leaders are joining forces to scale the ‘breakthrough’ tech</a>
          <div class="article-take">SK On and Factorial pool IP and capex to de‑risk solid‑state cell industrialization timelines.</div>
          <div class="article-tags">
            <span class="chip">SK On</span><span class="chip">Factorial</span><span class="chip">Battery</span><span class="chip">Solid‑state</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek</span>
          <span>Today</span>
          <a href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">78</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/waymo-gemini-ai-ojai-robotaxi-redesigned-interface/" target="_blank" rel="noopener">Waymo adds Google’s Gemini AI assistant and new UI to Ojai robotaxi</a>
          <div class="article-take">Conversational help and cleaner UX aim to widen AV adoption beyond early tech adopters.</div>
          <div class="article-tags">
            <span class="chip">Waymo</span><span class="chip">Autonomous</span><span class="chip">Software</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek</span>
          <span>Today</span>
          <a href="https://electrek.co/2026/07/29/waymo-gemini-ai-ojai-robotaxi-redesigned-interface/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">78</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">BMW puts G-Class rival on hold as China headwinds hit home</a>
          <div class="article-take">Shifting demand patterns and tariffs push BMW to re‑prioritize product mix and capex.</div>
          <div class="article-tags">
            <span class="chip">BMW</span><span class="chip">Strategy</span><span class="chip">China</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar</span>
          <span>Today</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">81</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/30/rivian-rivn-q2-2026-earnings-r2-deliveries-revenue-up-27/" target="_blank" rel="noopener">Rivian (RIVN) Q2 2026 earnings: revenue up 27%, gross margins soaring</a>
          <div class="article-take">Early R2 deliveries and cost cuts lift margins, improving cash runway and scaling prospects.</div>
          <div class="article-tags">
            <span class="chip">Rivian</span><span class="chip">Earnings</span><span class="chip">Finance</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek</span>
          <span>Today</span>
          <a href="https://electrek.co/2026/07/30/rivian-rivn-q2-2026-earnings-r2-deliveries-revenue-up-27/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">76</div>
        <div class="article-main">
          <a class="headline" href="https://www.greencarreports.com/news/1146051_gm-pilot-ev-charging-network-now-spans-over-25-states" target="_blank" rel="noopener">GM-Pilot EV charging network now spans over 25 states</a>
          <div class="article-take">Highway coverage expands as automakers co-invest to close charging gaps beyond Tesla’s network.</div>
          <div class="article-tags">
            <span class="chip">GM</span><span class="chip">Charging</span><span class="chip">EVgo</span>
          </div>
        </div>
        <div class="article-source">
          <span>Green Car Reports</span>
          <span>Today</span>
          <a href="https://www.greencarreports.com/news/1146051_gm-pilot-ev-charging-network-now-spans-over-25-states" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">74</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/evgo-and-brixmor-to-add-more-than-500-fast-charging-stalls-in-the-us/" target="_blank" rel="noopener">EVgo and Brixmor to add more than 500 fast charging stalls in the US</a>
          <div class="article-take">Retail‑center DCFC buildouts aim to boost convenience and utilization economics.</div>
          <div class="article-tags">
            <span class="chip">EVgo</span><span class="chip">Infrastructure</span><span class="chip">Retail</span>
          </div>
        </div>
        <div class="article-source">
          <span>electrive</span>
          <span>Today</span>
          <a href="https://www.electrive.com/2026/08/04/evgo-and-brixmor-to-add-more-than-500-fast-charging-stalls-in-the-us/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">77</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/byd-goes-after-defender-boxy-%C2%A348k-402bhp-hybrid-suv" target="_blank" rel="noopener">BYD goes after Defender with boxy £48k, 402bhp hybrid SUV</a>
          <div class="article-take">Aggressive UK pricing and rugged styling broaden BYD’s reach beyond city EVs.</div>
          <div class="article-tags">
            <span class="chip">BYD</span><span class="chip">PHEV</span><span class="chip">UK</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar</span>
          <span>Today</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/byd-goes-after-defender-boxy-%C2%A348k-402bhp-hybrid-suv" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">75</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/hyundai-reveals-ioniq-3-prices-start-30000-interest-surges/" target="_blank" rel="noopener">Hyundai reveals IONIQ 3 prices start at $30,000, and it already looks like a hit</a>
          <div class="article-take">A $30k entry point with 300+ miles range pressures competitors in the compact EV segment.</div>
          <div class="article-tags">
            <span class="chip">Hyundai</span><span class="chip">Pricing</span><span class="chip">EV</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek</span>
          <span>Today</span>
          <a href="https://electrek.co/2026/07/29/hyundai-reveals-ioniq-3-prices-start-30000-interest-surges/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">72</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/28/baidu-apollo-go-london-robotaxi-testing-uber-lyft/" target="_blank" rel="noopener">Baidu’s Apollo Go begins London robotaxi testing with Uber and Lyft</a>
          <div class="article-take">The Chinese AV service enters Europe via ride‑hailing alliances, signaling faster commercialization paths.</div>
          <div class="article-tags">
            <span class="chip">Baidu</span><span class="chip">Autonomous</span><span class="chip">International</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek</span>
          <span>Today</span>
          <a href="https://electrek.co/2026/07/28/baidu-apollo-go-london-robotaxi-testing-uber-lyft/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">73</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/philippines-launches-e850m-incentive-programme-for-ev-manufacturing/" target="_blank" rel="noopener">Philippines launches €850m incentive programme for EV manufacturing</a>
          <div class="article-take">New subsidies target local EV assembly and parts to attract regional investment.</div>
          <div class="article-tags">
            <span class="chip">Government</span><span class="chip">Manufacturing</span><span class="chip">APAC</span>
          </div>
        </div>
        <div class="article-source">
          <span>electrive</span>
          <span>Today</span>
          <a href="https://www.electrive.com/2026/08/04/philippines-launches-e850m-incentive-programme-for-ev-manufacturing/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">76</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/03/norways-ev-share-rises-to-97-6-in-july/" target="_blank" rel="noopener">Norway’s EV share rises to 97.6% in July</a>
          <div class="article-take">Norway remains the bellwether for end‑game electrification dynamics and policy design.</div>
          <div class="article-tags">
            <span class="chip">Norway</span><span class="chip">EV Adoption</span><span class="chip">Policy</span>
          </div>
        </div>
        <div class="article-source">
          <span>electrive</span>
          <span>Today</span>
          <a href="https://www.electrive.com/2026/08/03/norways-ev-share-rises-to-97-6-in-july/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">74</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/04/volvos-next-electric-suv-will-start-in-the-upper-40000-range/" target="_blank" rel="noopener">Volvo’s next electric SUV will start in the upper $40,000 range</a>
          <div class="article-take">An EX50 priced under $50k targets the US sweet spot as Volvo fills gaps below EX60.</div>
          <div class="article-tags">
            <span class="chip">Volvo</span><span class="chip">Pricing</span><span class="chip">Product</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek</span>
          <span>Today</span>
          <a href="https://electrek.co/2026/08/04/volvos-next-electric-suv-will-start-in-the-upper-40000-range/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">72</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/01/allego-commits-e100-million-to-expand-uk-charging-network/" target="_blank" rel="noopener">Allego commits €100 million to expand UK charging network</a>
          <div class="article-take">Capital targets urban and high‑traffic corridors to speed ultra‑rapid rollout by 2030.</div>
          <div class="article-tags">
            <span class="chip">Allego</span><span class="chip">Charging</span><span class="chip">UK</span>
          </div>
        </div>
        <div class="article-source">
          <span>electrive</span>
          <span>Today</span>
          <a href="https://www.electrive.com/2026/08/01/allego-commits-e100-million-to-expand-uk-charging-network/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">70</div>
        <div class="article-main">
          <a class="headline" href="https://chargedevs.com/newswire/beam-global-supplies-ev-arc-off-grid-charging-systems-for-dallas-municipal-fleet-and-massachusetts-carshare-pilot/" target="_blank" rel="noopener">Beam Global supplies EV ARC off-grid charging systems for fleets</a>
          <div class="article-take">Rapid‑deploy solar chargers bypass grid constraints for municipal use cases.</div>
          <div class="article-tags">
            <span class="chip">Beam Global</span><span class="chip">Off‑grid</span><span class="chip">Fleets</span>
          </div>
        </div>
        <div class="article-source">
          <span>Charged EVs</span>
          <span>Today</span>
          <a href="https://chargedevs.com/newswire/beam-global-supplies-ev-arc-off-grid-charging-systems-for-dallas-municipal-fleet-and-massachusetts-carshare-pilot/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">73</div>
        <div class="article-main">
          <a class="headline" href="https://www.greencarreports.com/news/1146052_here-are-the-evs-made-in-mexico-and-canada" target="_blank" rel="noopener">Here are the EVs made in Mexico and Canada</a>
          <div class="article-take">Sourcing shifts matter for tariffs, tax credits, and near‑term US pricing.</div>
          <div class="article-tags">
            <span class="chip">Trade</span><span class="chip">Manufacturing</span><span class="chip">North America</span>
          </div>
        </div>
        <div class="article-source">
          <span>Green Car Reports</span>
          <span>Today</span>
          <a href="https://www.greencarreports.com/news/1146052_here-are-the-evs-made-in-mexico-and-canada" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">70</div>
        <div class="article-main">
          <a class="headline" href="https://chargedevs.com/newswire/teletrac-navmans-energy-hub-gives-businesses-a-unified-view-of-energy-usage-in-mixed-ev-ice-fleets/" target="_blank" rel="noopener">Teletrac Navman launches Energy Hub for mixed EV/ICE fleets</a>
          <div class="article-take">Unified charging and fuel analytics help fleets optimize TCO during transition.</div>
          <div class="article-tags">
            <span class="chip">Teletrac Navman</span><span class="chip">Software</span><span class="chip">Fleet</span>
          </div>
        </div>
        <div class="article-source">
          <span>Charged EVs</span>
          <span>Today</span>
          <a href="https://chargedevs.com/newswire/teletrac-navmans-energy-hub-gives-businesses-a-unified-view-of-energy-usage-in-mixed-ev-ice-fleets/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">83</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/03/tesla-fsd-v14-lite-hw3-computer-failures/" target="_blank" rel="noopener">Tesla FSD v14 Lite tied to rising HW3 computer failures, owners report</a>
          <div class="article-take">Thermal headroom concerns re‑ignite debate over legacy hardware support and OTA feature loads.</div>
          <div class="article-tags">
            <span class="chip">Tesla</span><span class="chip">Software</span><span class="chip">Safety</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek</span>
          <span>Today</span>
          <a href="https://electrek.co/2026/08/03/tesla-fsd-v14-lite-hw3-computer-failures/" target="_blank" rel="noopener">Read original →</a>
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
    <h2 class="section-title">Industry News <span class="count">Key developments</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip high">92</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">NHTSA opens probe into 1.2M Tesla Model 3/Y over suspension failures</a>
          <div class="article-take">Regulatory heat rises on fast‑scaling EV programs and supplier validation.</div>
          <div class="article-tags"><span class="chip">Regulation</span><span class="chip">Safety</span></div>
        </div>
        <div class="article-source">
          <span>Electrek</span><span>Today</span>
          <a href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">84</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/477795/" target="_blank" rel="noopener">IEA: Global EV sales jump 35% in Q2 and 50 countries set records</a>
          <div class="article-take">Demand recovery supports OEM volume and network planning assumptions.</div>
          <div class="article-tags"><span class="chip">Markets</span><span class="chip">EV</span></div>
        </div>
        <div class="article-source">
          <span>Electrek</span><span>Today</span>
          <a href="https://electrek.co/2026/07/29/477795/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">78</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">BMW pauses hardcore off-roader as China headwinds mount</a>
          <div class="article-take">Capex shifts reflect diverging global demand and tariff risk.</div>
          <div class="article-tags"><span class="chip">Strategy</span><span class="chip">China</span></div>
        </div>
        <div class="article-source">
          <span>Autocar</span><span>Today</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="electric-vehicles">
    <h2 class="section-title">Electric Vehicles <span class="count">Product & adoption</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip">82</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/new-mercedes-gla-ev-bigger-400-miles-range/" target="_blank" rel="noopener">Mercedes GLA EV: more space, 800V fast charge, 400+ miles range</a>
          <div class="article-take">Compact luxury EV stakes rise with long‑range trims and high‑power charging.</div>
          <div class="article-tags"><span class="chip">Mercedes-Benz</span><span class="chip">EV</span></div>
        </div>
        <div class="article-source">
          <span>Electrek</span><span>Today</span>
          <a href="https://electrek.co/2026/07/29/new-mercedes-gla-ev-bigger-400-miles-range/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">76</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/03/norways-ev-share-rises-to-97-6-in-july/" target="_blank" rel="noopener">Norway posts 97.6% EV share in July</a>
          <div class="article-take">End‑state hints at future retail models and residual dynamics elsewhere.</div>
          <div class="article-tags"><span class="chip">EV Adoption</span><span class="chip">Policy</span></div>
        </div>
        <div class="article-source">
          <span>electrive</span><span>Today</span>
          <a href="https://www.electrive.com/2026/08/03/norways-ev-share-rises-to-97-6-in-july/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">79</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/reborn-audi-a2-driven-electric-comeback-efficiency-king" target="_blank" rel="noopener">Audi A2 e‑tron returns focused on extreme efficiency</a>
          <div class="article-take">Low‑drag compact targets cost‑efficient miles for mass buyers.</div>
          <div class="article-tags"><span class="chip">Audi</span><span class="chip">Efficiency</span></div>
        </div>
        <div class="article-source">
          <span>Autocar</span><span>Today</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/reborn-audi-a2-driven-electric-comeback-efficiency-king" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="manufacturers">
    <h2 class="section-title">Manufacturers <span class="count">Strategies & launches</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip">81</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/30/rivian-rivn-q2-2026-earnings-r2-deliveries-revenue-up-27/" target="_blank" rel="noopener">Rivian revenue and margins improve with R2 ramp</a>
          <div class="article-take">Scaling discipline begins to bend the cost curve in Rivian’s favor.</div>
          <div class="article-tags"><span class="chip">Rivian</span><span class="chip">Finance</span></div>
        </div>
        <div class="article-source">
          <span>Electrek</span><span>Today</span>
          <a href="https://electrek.co/2026/07/30/rivian-rivn-q2-2026-earnings-r2-deliveries-revenue-up-27/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">77</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/byd-goes-after-defender-boxy-%C2%A348k-402bhp-hybrid-suv" target="_blank" rel="noopener">BYD Ti7 targets UK family adventure segment</a>
          <div class="article-take">Value‑priced rugged PHEV expands BYD’s brand beyond city commuters.</div>
          <div class="article-tags"><span class="chip">BYD</span><span class="chip">UK</span></div>
        </div>
        <div class="article-source">
          <span>Autocar</span><span>Today</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/byd-goes-after-defender-boxy-%C2%A348k-402bhp-hybrid-suv" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="dealers">
    <h2 class="section-title">Dealers <span class="count">Retail & network</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip">70</div>
        <div class="article-main">
          <a class="headline" href="https://www.motor1.com/news/803722/costco-infiniti-discount/" target="_blank" rel="noopener">Costco is offering big discounts on new Infiniti SUVs</a>
          <div class="article-take">Warehouse partnerships keep showroom traffic flowing with turnkey incentives.</div>
          <div class="article-tags"><span class="chip">Retail</span><span class="chip">Incentives</span></div>
        </div>
        <div class="article-source">
          <span>Motor1</span><span>Today</span>
          <a href="https://www.motor1.com/news/803722/costco-infiniti-discount/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">69</div>
        <div class="article-main">
          <a class="headline" href="https://www.caranddriver.com/news/a73337003/hyundai-kia-genesis-record-sales-july-2026/" target="_blank" rel="noopener">Hyundai, Kia, and Genesis post record July US sales</a>
          <div class="article-take">Affordable hybrids and sharp pricing keep showrooms busy despite EV volatility.</div>
          <div class="article-tags"><span class="chip">Sales</span><span class="chip">Hybrids</span></div>
        </div>
        <div class="article-source">
          <span>Car and Driver</span><span>Today</span>
          <a href="https://www.caranddriver.com/news/a73337003/hyundai-kia-genesis-record-sales-july-2026/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="suppliers">
    <h2 class="section-title">Suppliers <span class="count">Ecosystem moves</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip">74</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/evgo-and-brixmor-to-add-more-than-500-fast-charging-stalls-in-the-us/" target="_blank" rel="noopener">EVgo and Brixmor expand fast charging across retail centers</a>
          <div class="article-take">Leveraging shopping trips to boost charger utilization and economics.</div>
          <div class="article-tags"><span class="chip">EVgo</span><span class="chip">Retail</span></div>
        </div>
        <div class="article-source">
          <span>electrive</span><span>Today</span>
          <a href="https://www.electrive.com/2026/08/04/evgo-and-brixmor-to-add-more-than-500-fast-charging-stalls-in-the-us/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">71</div>
        <div class="article-main">
          <a class="headline" href="https://chargedevs.com/newswire/mahle-introduces-a-new-range-extender-engine-and-a-rare-earth-free-electric-motor/" target="_blank" rel="noopener">MAHLE reveals range extender for heavy trucks and rare‑earth‑free e‑motor</a>
          <div class="article-take">Suppliers race to derisk cost and material exposure in electrified drivetrains.</div>
          <div class="article-tags"><span class="chip">MAHLE</span><span class="chip">Powertrain</span></div>
        </div>
        <div class="article-source">
          <span>Charged EVs</span><span>Today</span>
          <a href="https://chargedevs.com/newswire/mahle-introduces-a-new-range-extender-engine-and-a-rare-earth-free-electric-motor/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="government">
    <h2 class="section-title">Government <span class="count">Policy & regulation</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip high">92</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">US opens major safety probe into Tesla suspension failures</a>
          <div class="article-take">Outcome could reshape OEM validation norms and supplier accountability.</div>
          <div class="article-tags"><span class="chip">NHTSA</span><span class="chip">Safety</span></div>
        </div>
        <div class="article-source">
          <span>Electrek</span><span>Today</span>
          <a href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">73</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/philippines-launches-e850m-incentive-programme-for-ev-manufacturing/" target="_blank" rel="noopener">Philippines unveils EV manufacturing incentives</a>
          <div class="article-take">Southeast Asia competition for EV supply chain intensifies.</div>
          <div class="article-tags"><span class="chip">APAC</span><span class="chip">Investment</span></div>
        </div>
        <div class="article-source">
          <span>electrive</span><span>Today</span>
          <a href="https://www.electrive.com/2026/08/04/philippines-launches-e850m-incentive-programme-for-ev-manufacturing/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="technology">
    <h2 class="section-title">Technology <span class="count">Batteries & software</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip">80</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">SK On and Factorial join forces on solid‑state scale‑up</a>
          <div class="article-take">Partnerships aim to compress timelines from pilot lines to auto‑grade volumes.</div>
          <div class="article-tags"><span class="chip">Battery</span><span class="chip">Solid‑state</span></div>
        </div>
        <div class="article-source">
          <span>Electrek</span><span>Today</span>
          <a href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">78</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/waymo-gemini-ai-ojai-robotaxi-redesigned-interface/" target="_blank" rel="noopener">Waymo integrates Gemini AI to smooth robotaxi experience</a>
          <div class="article-take">Voice‑first UX could broaden appeal and reduce rider support friction.</div>
          <div class="article-tags"><span class="chip">Autonomous</span><span class="chip">AI</span></div>
        </div>
        <div class="article-source">
          <span>Electrek</span><span>Today</span>
          <a href="https://electrek.co/2026/07/29/waymo-gemini-ai-ojai-robotaxi-redesigned-interface/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">74</div>
        <div class="article-main">
          <a class="headline" href="https://www.greencarreports.com/news/1146043_sulfur-crystal-battery-could-triple-ev-range-without-cobalt-or-nickel" target="_blank" rel="noopener">Sulfur‑crystal battery promises higher energy without nickel/cobalt</a>
          <div class="article-take">If scalable, materials shift could ease costs and ESG pressure.</div>
          <div class="article-tags"><span class="chip">Battery</span><span class="chip">Chemistry</span></div>
        </div>
        <div class="article-source">
          <span>Green Car Reports</span><span>Today</span>
          <a href="https://www.greencarreports.com/news/1146043_sulfur-crystal-battery-could-triple-ev-range-without-cobalt-or-nickel" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="finance">
    <h2 class="section-title">Finance <span class="count">Earnings & sales</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip">81</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/30/rivian-rivn-q2-2026-earnings-r2-deliveries-revenue-up-27/" target="_blank" rel="noopener">Rivian beats on revenue and narrows losses in Q2</a>
          <div class="article-take">Improving gross profit signals healthier scaling curve.</div>
          <div class="article-tags"><span class="chip">Earnings</span><span class="chip">EV</span></div>
        </div>
        <div class="article-source">
          <span>Electrek</span><span>Today</span>
          <a href="https://electrek.co/2026/07/30/rivian-rivn-q2-2026-earnings-r2-deliveries-revenue-up-27/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">78</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/03/byd-boosts-sales-by-22-in-july/" target="_blank" rel="noopener">BYD boosts July sales by 22% as exports hit records</a>
          <div class="article-take">Overseas growth offsets slower China retail, sustaining volume.</div>
          <div class="article-tags"><span class="chip">BYD</span><span class="chip">Sales</span></div>
        </div>
        <div class="article-source">
          <span>electrive</span><span>Today</span>
          <a href="https://www.electrive.com/2026/08/03/byd-boosts-sales-by-22-in-july/" target="_blank" rel="noopener">Read original →</a>
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
          <a class="headline" href="https://electrek.co/2026/07/28/baidu-apollo-go-london-robotaxi-testing-uber-lyft/" target="_blank" rel="noopener">Baidu Apollo Go starts London AV tests with Uber and Lyft</a>
          <div class="article-take">Cross‑border AV pilots accelerate competitive learning cycles.</div>
          <div class="article-tags"><span class="chip">Baidu</span><span class="chip">AV</span></div>
        </div>
        <div class="article-source">
          <span>Electrek</span><span>Today</span>
          <a href="https://electrek.co/2026/07/28/baidu-apollo-go-london-robotaxi-testing-uber-lyft/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">73</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/philippines-launches-e850m-incentive-programme-for-ev-manufacturing/" target="_blank" rel="noopener">Philippines lures EV investment with €850m program</a>
          <div class="article-take">Regional manufacturing base competition intensifies in ASEAN.</div>
          <div class="article-tags"><span class="chip">Manufacturing</span><span class="chip">ASEAN</span></div>
        </div>
        <div class="article-source">
          <span>electrive</span><span>Today</span>
          <a href="https://www.electrive.com/2026/08/04/philippines-launches-e850m-incentive-programme-for-ev-manufacturing/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="opinion">
    <h2 class="section-title">Opinion <span class="count">Perspectives</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip">68</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/opinion/new-cars/ignore-jay-leno-your-dream-garage-only-needs-three-cars" target="_blank" rel="noopener">Ignore Jay Leno: your dream garage only needs three cars</a>
          <div class="article-take">A case for curation over collection in enthusiast car ownership.</div>
          <div class="article-tags"><span class="chip">Opinion</span><span class="chip">Culture</span></div>
        </div>
        <div class="article-source">
          <span>Autocar</span><span>Today</span>
          <a href="https://www.autocar.co.uk/opinion/new-cars/ignore-jay-leno-your-dream-garage-only-needs-three-cars" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">67</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/opinion/business-corporate/roof-boxes-top-car-accessory-market-defies-auto-downturn" target="_blank" rel="noopener">Roof boxes on top as car accessory market defies auto downturn</a>
          <div class="article-take">Premium accessory brands show resilience even as OEMs struggle in China.</div>
          <div class="article-tags"><span class="chip">Accessories</span><span class="chip">Margins</span></div>
        </div>
        <div class="article-source">
          <span>Autocar</span><span>Today</span>
          <a href="https://www.autocar.co.uk/opinion/business-corporate/roof-boxes-top-car-accessory-market-defies-auto-downturn" target="_blank" rel="noopener">Read original →</a>
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