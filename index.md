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
        <h1>NHTSA opens investigation into 1.2 million Tesla Model 3/Y over front suspension failures</h1>
        <p class="exec-summary">US regulators launched a sweeping probe after reports that a key front-suspension link can detach on late‑2010s Model 3s and early‑2020s Model Ys. The review puts Tesla’s largest US nameplates under safety scrutiny, with potential implications for recalls, repair costs, and future design validation across the EV industry.</p>

        <div class="takeaways">
          <h3>Key Takeaways</h3>
          <ul>
            
            <!-- repeat: <li>{{TAKEAWAY}}</li> -->
          </ul>
        </div>

        <div class="impact-row">
          <div class="impact-block">
            <h4>Industry Impact</h4>
            <p>The case will test how quickly a high‑volume EV maker can diagnose field failures and execute fixes at scale, while competitors watch for regulatory appetite to more aggressively police new‑tech platforms. Any recall or parts rework could ripple into service capacity, resale values, and supplier qualification standards.</p>
          </div>
          <div class="impact-block">
            <h4>Companies Affected</h4>
            <div class="chip-row">
              <span class="chip entity-mfr">Tesla</span>
              <span class="chip">NHTSA</span>
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
            <li><a href="https://electrek.co/2026/07/30/tesla-10-millionth-vehicle-ev-growth-stalled/" target="_blank" rel="noopener">Tesla hits 10 million vehicles — growth stalls</a></li>
            <li><a href="https://electrek.co/2026/08/04/tesla-china-sales-crash-exports-surge-h1-2026/" target="_blank" rel="noopener">Tesla China sales fall as exports surge</a></li>
          </ul>
        </div>
      </div>

      <div class="hero-gauges">
        <div class="gauge">
          <svg viewBox="0 0 120 70"><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#2a3038" stroke-width="8"/><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#f2a93b" stroke-width="8" stroke-dasharray="157" stroke-dashoffset="14.13"/></svg>
          <span class="gauge-value mono">91</span>
          <span class="gauge-label">Importance</span>
        </div>
        <div class="gauge">
          <svg viewBox="0 0 120 70"><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#2a3038" stroke-width="8"/><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#3ecf8e" stroke-width="8" stroke-dasharray="157" stroke-dashoffset="21.98"/></svg>
          <span class="gauge-value mono">86</span>
          <span class="gauge-label">Editorial Quality</span>
        </div>
        <div class="gauge">
          <svg viewBox="0 0 120 70"><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#2a3038" stroke-width="8"/><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#e2604f" stroke-width="8" stroke-dasharray="157" stroke-dashoffset="18.84"/></svg>
          <span class="gauge-value mono">88</span>
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
    <h2 class="section-title">Industry Snapshot <span class="count">Past 24 hours</span></h2>
    <div class="dash-grid">
      <div class="stat-panel">
        <h4>Top Manufacturers</h4>
        <ul class="rank-list">
          <li><span>Tesla</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:100%"></div></div><span class="rank-count">14</span></li>
          <li><span>Mercedes-Benz</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:82%"></div></div><span class="rank-count">11</span></li>
          <li><span>BYD</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:78%"></div></div><span class="rank-count">10</span></li>
          <li><span>Hyundai/Kia</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:71%"></div></div><span class="rank-count">9</span></li>
          <li><span>BMW</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:68%"></div></div><span class="rank-count">8</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4>Top Brands</h4>
        <ul class="rank-list">
          <li><span>Audi</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:88%"></div></div><span class="rank-count">12</span></li>
          <li><span>Volkswagen</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:73%"></div></div><span class="rank-count">9</span></li>
          <li><span>Volvo</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:65%"></div></div><span class="rank-count">8</span></li>
          <li><span>Genesis</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:50%"></div></div><span class="rank-count">6</span></li>
          <li><span>Porsche</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:46%"></div></div><span class="rank-count">5</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4>Top Suppliers</h4>
        <ul class="rank-list">
          <li><span>SK On</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:100%"></div></div><span class="rank-count">5</span></li>
          <li><span>Factorial Energy</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:90%"></div></div><span class="rank-count">4</span></li>
          <li><span>MAHLE</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:80%"></div></div><span class="rank-count">4</span></li>
          <li><span>Beam Global</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:70%"></div></div><span class="rank-count">3</span></li>
          <li><span>Allego</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:60%"></div></div><span class="rank-count">3</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4>Most Mentioned Executives</h4>
        <ul class="rank-list">
          <li><span>Elon Musk (Tesla)</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:100%"></div></div><span class="rank-count">9</span></li>
          <li><span>Ola Källenius (Mercedes)</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:78%"></div></div><span class="rank-count">7</span></li>
          <li><span>RJ Scaringe (Rivian)</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:67%"></div></div><span class="rank-count">6</span></li>
          <li><span>Dmitri Dolgov (Waymo)</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:56%"></div></div><span class="rank-count">5</span></li>
          <li><span>Michael Leiters (Porsche)</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:44%"></div></div><span class="rank-count">4</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4>Trending Topics</h4>
        <div class="tagcloud">
          <span class="chip lg">NHTSA probe</span>
          <span class="chip">GLA EV launch</span>
          <span class="chip">Solid‑state batteries</span>
          <span class="chip">Robotaxis</span>
          <span class="chip">Charging build‑out</span>
          <span class="chip">EV sales rebound</span>
          <span class="chip">Lidar vs cameras</span>
          <span class="chip">Affordable EVs</span>
          <span class="chip">China exports</span>
        </div>
      </div>

      <div class="stat-panel">
        <h4>Emerging Technologies</h4>
        <div class="tagcloud">
          <span class="chip lg">Solid‑state cells</span>
          <span class="chip">Iron‑air storage</span>
          <span class="chip">800V platforms</span>
          <span class="chip">SDV architectures</span>
          <span class="chip">AI in HMI</span>
          <span class="chip">V2X/VPP</span>
        </div>
      </div>

      <div class="stat-panel">
        <h4>Government & Policy</h4>
        <div class="tagcloud">
          <span class="chip lg">NHTSA</span>
          <span class="chip">Philippines EV incentives</span>
          <span class="chip">Denmark EV share</span>
          <span class="chip">US tariffs discussion</span>
          <span class="chip">UK grants</span>
        </div>
      </div>

      <div class="stat-panel">
        <h4>Financial & Markets</h4>
        <ul class="rank-list">
          <li><span>Rivian beats Q2, margins up</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:95%"></div></div><span class="rank-count">A</span></li>
          <li><span>Lucid +5% stake disclosed</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:80%"></div></div><span class="rank-count">B</span></li>
          <li><span>BMW reevaluates lineup</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:72%"></div></div><span class="rank-count">C</span></li>
          <li><span>BYD July sales +22%</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:68%"></div></div><span class="rank-count">D</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4>Global Regions</h4>
        <div class="tagcloud">
          <span class="chip lg">United States</span>
          <span class="chip">China</span>
          <span class="chip">United Kingdom</span>
          <span class="chip">European Union</span>
          <span class="chip">Nordics</span>
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
        <a href="https://www.autocar.co.uk/car-news/new-cars/audi-q9-suv-revealed-huge-%C2%A3100k-a8-successor" target="_blank" rel="noopener">Audi reveals Q9 flagship SUV as A8 successor</a>
        <div class="fp-meta"><span>Score 82</span><span>•</span><span>Autocar</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/28/bmw-ramps-up-ix3-output-orders-near-100000/" target="_blank" rel="noopener">BMW ramps iX3 output as orders near 100k</a>
        <div class="fp-meta"><span>Score 78</span><span>•</span><span>Electrek</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.autocar.co.uk/car-news/electric-cars/new-mercedes-gla-revealed-audi-q4-rival-408-mile-range" target="_blank" rel="noopener">Mercedes unveils new GLA EV with 408‑mile range</a>
        <div class="fp-meta"><span>Score 85</span><span>•</span><span>Autocar</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">BMW puts G‑Class rival on hold amid China headwinds</a>
        <div class="fp-meta"><span>Score 73</span><span>•</span><span>Autocar</span></div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Technology</h3>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/waymo-gemini-ai-ojai-robotaxi-redesigned-interface/" target="_blank" rel="noopener">Waymo adds Gemini AI and new UI to robotaxi</a>
        <div class="fp-meta"><span>Score 79</span><span>•</span><span>Electrek</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">SK On + Factorial team up on solid‑state batteries</a>
        <div class="fp-meta"><span>Score 80</span><span>•</span><span>Electrek</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Volvo drops lidar on EX90/ES90, compensates owners</a>
        <div class="fp-meta"><span>Score 77</span><span>•</span><span>Electrek</span></div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Government</h3>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">NHTSA probes 1.2M Teslas for suspension failures</a>
        <div class="fp-meta"><span>Score 91</span><span>•</span><span>Electrek</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.electrive.com/2026/08/04/philippines-launches-e850m-incentive-programme-for-ev-manufacturing/" target="_blank" rel="noopener">Philippines launches €850m EV manufacturing incentives</a>
        <div class="fp-meta"><span>Score 74</span><span>•</span><span>electrive</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.electrive.com/2026/08/04/denmark-evs-account-for-almost-all-new-car-registrations-in-july/" target="_blank" rel="noopener">Denmark: EVs hit 97.6% of private registrations in July</a>
        <div class="fp-meta"><span>Score 72</span><span>•</span><span>electrive</span></div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Suppliers & Infrastructure</h3>
      <div class="fp-row">
        <a href="https://chargedevs.com/newswire/beam-global-supplies-ev-arc-off-grid-charging-systems-for-dallas-municipal-fleet-and-massachusetts-carshare-pilot/" target="_blank" rel="noopener">Beam Global wins municipal off‑grid charging orders</a>
        <div class="fp-meta"><span>Score 70</span><span>•</span><span>Charged EVs</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.electrive.com/2026/08/01/allego-commits-e100-million-to-expand-uk-charging-network/" target="_blank" rel="noopener">Allego to invest €100m in UK ultra‑rapid charging</a>
        <div class="fp-meta"><span>Score 71</span><span>•</span><span>electrive</span></div>
      </div>
      <div class="fp-row">
        <a href="https://chargedevs.com/newswire/mahle-introduces-a-new-range-extender-engine-and-a-rare-earth-free-electric-motor/" target="_blank" rel="noopener">MAHLE unveils HD range‑extender and rare‑earth‑free motor</a>
        <div class="fp-meta"><span>Score 69</span><span>•</span><span>Charged EVs</span></div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Trending Topics</h3>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/477795/" target="_blank" rel="noopener">IEA: Global EV sales rebounded 35% in Q2</a>
        <div class="fp-meta"><span>Score 83</span><span>•</span><span>Electrek</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/08/04/waymo-co-ceo-camera-only-self-driving-tesla/" target="_blank" rel="noopener">Waymo CEO: camera‑only autonomy hits a safety ceiling</a>
        <div class="fp-meta"><span>Score 76</span><span>•</span><span>Electrek</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/28/volkswagen-launches-cheaper-id-polo-ev-orders-25000/" target="_blank" rel="noopener">VW launches cheaper ID. Polo after 25k pre‑orders</a>
        <div class="fp-meta"><span>Score 75</span><span>•</span><span>Electrek</span></div>
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
    <h2 class="section-title">Latest Articles <span class="count">18 analyzed today</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip high">91</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">NHTSA opens probe into 1.2M Tesla Model 3/Y over suspension failures</a>
          <div class="article-take">A sweeping safety review could force large‑scale fixes on Tesla’s highest‑volume models.</div>
          <div class="article-tags">
            <span class="chip">Tesla</span><span class="chip">NHTSA</span><span class="chip">Safety</span><span class="chip">Government</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek • Today</span>
          <a href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip high">85</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/electric-cars/new-mercedes-gla-revealed-audi-q4-rival-408-mile-range" target="_blank" rel="noopener">New Mercedes GLA EV revealed with up to 408‑mile range</a>
          <div class="article-take">Mercedes pushes its compact EV platform upmarket with range, charging speed and software polish.</div>
          <div class="article-tags">
            <span class="chip">Mercedes-Benz</span><span class="chip">GLA EV</span><span class="chip">EV</span><span class="chip">Production</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar • Today</span>
          <a href="https://www.autocar.co.uk/car-news/electric-cars/new-mercedes-gla-revealed-audi-q4-rival-408-mile-range" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">78</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">SK On and Factorial team up to scale solid‑state batteries</a>
          <div class="article-take">A fresh alliance aims to accelerate commercialization timelines beyond lab pilots.</div>
          <div class="article-tags">
            <span class="chip">SK On</span><span class="chip">Factorial</span><span class="chip">Battery</span><span class="chip">Solid‑state</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek • Today</span>
          <a href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">80</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/waymo-gemini-ai-ojai-robotaxi-redesigned-interface/" target="_blank" rel="noopener">Waymo integrates Google Gemini AI in new robotaxi UI</a>
          <div class="article-take">Conversational assistance moves front‑and‑center as Waymo readies wider Ojai access.</div>
          <div class="article-tags">
            <span class="chip">Waymo</span><span class="chip">Autonomous</span><span class="chip">Software</span><span class="chip">Mobility</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek • Today</span>
          <a href="https://electrek.co/2026/07/29/waymo-gemini-ai-ojai-robotaxi-redesigned-interface/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">74</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/philippines-launches-e850m-incentive-programme-for-ev-manufacturing/" target="_blank" rel="noopener">Philippines unveils €850m incentives to attract EV manufacturing</a>
          <div class="article-take">Manila targets local assembly and component ecosystems with production‑linked support.</div>
          <div class="article-tags">
            <span class="chip">Government</span><span class="chip">Trade</span><span class="chip">Manufacturing</span><span class="chip">Southeast Asia</span>
          </div>
        </div>
        <div class="article-source">
          <span>electrive • Today</span>
          <a href="https://www.electrive.com/2026/08/04/philippines-launches-e850m-incentive-programme-for-ev-manufacturing/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">83</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/477795/" target="_blank" rel="noopener">IEA: Global EV sales jump 35% in Q2; 50 countries hit records</a>
          <div class="article-take">Demand reaccelerated after a slow start to 2026, easing fears of a prolonged slump.</div>
          <div class="article-tags">
            <span class="chip">EV market</span><span class="chip">IEA</span><span class="chip">Finance</span><span class="chip">Global</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek • Today</span>
          <a href="https://electrek.co/2026/07/29/477795/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">77</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Volvo ditches lidar on EX90/ES90, compensates affected owners</a>
          <div class="article-take">The brand pivots sensor strategy and absorbs goodwill costs to protect launch momentum.</div>
          <div class="article-tags">
            <span class="chip">Volvo</span><span class="chip">ADAS</span><span class="chip">Lidar</span><span class="chip">Software</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek • Today</span>
          <a href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">72</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/01/allego-commits-e100-million-to-expand-uk-charging-network/" target="_blank" rel="noopener">Allego commits €100m to expand UK ultra‑rapid charging</a>
          <div class="article-take">Scale moves to retail hubs and dense urban corridors as public fast charging matures.</div>
          <div class="article-tags">
            <span class="chip">Charging</span><span class="chip">Allego</span><span class="chip">Infrastructure</span><span class="chip">UK</span>
          </div>
        </div>
        <div class="article-source">
          <span>electrive • Today</span>
          <a href="https://www.electrive.com/2026/08/01/allego-commits-e100-million-to-expand-uk-charging-network/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">75</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/28/volkswagen-launches-cheaper-id-polo-ev-orders-25000/" target="_blank" rel="noopener">VW launches cheaper ID. Polo EV after 25,000 early orders</a>
          <div class="article-take">A smaller pack option pulls the sub‑$30k segment deeper into mainstream buyers.</div>
          <div class="article-tags">
            <span class="chip">Volkswagen</span><span class="chip">Affordable EV</span><span class="chip">EV</span><span class="chip">Retail</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek • Today</span>
          <a href="https://electrek.co/2026/07/28/volkswagen-launches-cheaper-id-polo-ev-orders-25000/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">73</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">BMW rethinks product roadmap; G‑Class rival put on ice</a>
          <div class="article-take">Diverging global demand and China pressure are reshaping late‑decade model bets.</div>
          <div class="article-tags">
            <span class="chip">BMW</span><span class="chip">Strategy</span><span class="chip">Manufacturers</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar • Today</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">70</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/denmark-evs-account-for-almost-all-new-car-registrations-in-july/" target="_blank" rel="noopener">Denmark nears 100% EV share of private registrations in July</a>
          <div class="article-take">Policy stability and product choice show how quickly a market can tip once economics align.</div>
          <div class="article-tags">
            <span class="chip">Denmark</span><span class="chip">EV Adoption</span><span class="chip">Government</span>
          </div>
        </div>
        <div class="article-source">
          <span>electrive • Today</span>
          <a href="https://www.electrive.com/2026/08/04/denmark-evs-account-for-almost-all-new-car-registrations-in-july/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">76</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/04/volvos-next-electric-suv-will-start-in-the-upper-40000-range/" target="_blank" rel="noopener">Volvo’s next electric SUV to start under $50k in US</a>
          <div class="article-take">EX50 targets Model Y pricing with Scandinavian spec discipline and brand safety halo.</div>
          <div class="article-tags">
            <span class="chip">Volvo</span><span class="chip">Pricing</span><span class="chip">EV</span><span class="chip">Retail</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek • Today</span>
          <a href="https://electrek.co/2026/08/04/volvos-next-electric-suv-will-start-in-the-upper-40000-range/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">79</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/04/waymo-co-ceo-camera-only-self-driving-tesla/" target="_blank" rel="noopener">Waymo co‑CEO argues camera‑only autonomy falls short</a>
          <div class="article-take">The sensor‑stack debate sharpens as safety thresholds move beyond human parity.</div>
          <div class="article-tags">
            <span class="chip">Waymo</span><span class="chip">Autonomous</span><span class="chip">Safety</span><span class="chip">Software</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek • Today</span>
          <a href="https://electrek.co/2026/08/04/waymo-co-ceo-camera-only-self-driving-tesla/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">68</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/04/revoy-ev-promises-to-electrify-diesel-semis-in-minutes/" target="_blank" rel="noopener">Revoy raises $27M to electrify diesel semis via add‑on tandem</a>
          <div class="article-take">Hybridizing existing tractors could slash fleet fuel costs faster than full truck swaps.</div>
          <div class="article-tags">
            <span class="chip">Fleet</span><span class="chip">Hybridization</span><span class="chip">Logistics</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek • Today</span>
          <a href="https://electrek.co/2026/08/04/revoy-ev-promises-to-electrify-diesel-semis-in-minutes/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">71</div>
        <div class="article-main">
          <a class="headline" href="https://www.greencarreports.com/news/1146051_gm-pilot-ev-charging-network-now-spans-over-25-states" target="_blank" rel="noopener">GM‑Pilot fast‑charging network now spans 25+ states</a>
          <div class="article-take">Anchor sites on highway corridors broaden non‑Tesla DCFC access ahead of NACS shift.</div>
          <div class="article-tags">
            <span class="chip">GM</span><span class="chip">EVgo</span><span class="chip">Charging</span><span class="chip">Infrastructure</span>
          </div>
        </div>
        <div class="article-source">
          <span>Green Car Reports • Today</span>
          <a href="https://www.greencarreports.com/news/1146051_gm-pilot-ev-charging-network-now-spans-over-25-states" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">69</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/28/baidu-apollo-go-london-robotaxi-testing-uber-lyft/" target="_blank" rel="noopener">Baidu’s Apollo Go begins London robotaxi testing with Uber and Lyft</a>
          <div class="article-take">China’s AV leader pilots right‑hand‑drive ops with platform partners in the UK.</div>
          <div class="article-tags">
            <span class="chip">Baidu</span><span class="chip">Robotaxi</span><span class="chip">International</span><span class="chip">Mobility</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek • Today</span>
          <a href="https://electrek.co/2026/07/28/baidu-apollo-go-london-robotaxi-testing-uber-lyft/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">67</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/30/tesla-elon-musk-2026-x-meltdown/" target="_blank" rel="noopener">Opinion: Tesla governance faces renewed investor scrutiny</a>
          <div class="article-take">Communication risks are bleeding into brand and regulatory exposure for a public automaker.</div>
          <div class="article-tags">
            <span class="chip">Tesla</span><span class="chip">Governance</span><span class="chip">Finance</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek • Today</span>
          <a href="https://electrek.co/2026/07/30/tesla-elon-musk-2026-x-meltdown/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">66</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/opinion/business-corporate/roof-boxes-top-car-accessory-market-defies-auto-downturn" target="_blank" rel="noopener">Accessory makers thrive as car sales wobble</a>
          <div class="article-take">Premium carriers and racks show pricing power even as OEMs fight discounting and tariffs.</div>
          <div class="article-tags">
            <span class="chip">Aftermarket</span><span class="chip">Retail</span><span class="chip">Europe</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar • Today</span>
          <a href="https://www.autocar.co.uk/car-news/opinion/business-corporate/roof-boxes-top-car-accessory-market-defies-auto-downturn" target="_blank" rel="noopener">Read original →</a>
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
    <h2 class="section-title">Industry News <span class="count">6 items</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip high">91</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">NHTSA investigates 1.2M Teslas over suspension issues</a>
          <div class="article-take">Regulatory heat lands on the EV market leader’s core models.</div>
          <div class="article-tags"><span class="chip">Government</span><span class="chip">Safety</span><span class="chip">Tesla</span></div>
        </div>
        <div class="article-source">
          <span>Electrek • Today</span>
          <a href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">83</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/477795/" target="_blank" rel="noopener">IEA: EV sales bounce back 35% in Q2</a>
          <div class="article-take">Momentum returns across key regions after Q1 softness.</div>
          <div class="article-tags"><span class="chip">Market</span><span class="chip">EV</span><span class="chip">Finance</span></div>
        </div>
        <div class="article-source">
          <span>Electrek • Today</span>
          <a href="https://electrek.co/2026/07/29/477795/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">73</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">BMW pauses rugged SUV project amid China headwinds</a>
          <div class="article-take">The brand recalibrates its late‑decade portfolio to changing demand.</div>
          <div class="article-tags"><span class="chip">BMW</span><span class="chip">Strategy</span><span class="chip">Manufacturers</span></div>
        </div>
        <div class="article-source">
          <span>Autocar • Today</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">71</div>
        <div class="article-main">
          <a class="headline" href="https://www.greencarreports.com/news/1146051_gm-pilot-ev-charging-network-now-spans-over-25-states" target="_blank" rel="noopener">GM‑Pilot/EVgo highway charging spans 25 states</a>
          <div class="article-take">US corridor coverage keeps expanding beyond Superchargers.</div>
          <div class="article-tags"><span class="chip">Charging</span><span class="chip">Infrastructure</span></div>
        </div>
        <div class="article-source">
          <span>Green Car Reports • Today</span>
          <a href="https://www.greencarreports.com/news/1146051_gm-pilot-ev-charging-network-now-spans-over-25-states" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">70</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/denmark-evs-account-for-almost-all-new-car-registrations-in-july/" target="_blank" rel="noopener">Denmark approaches all‑EV private registrations</a>
          <div class="article-take">A glimpse of a post‑ICE retail market at national scale.</div>
          <div class="article-tags"><span class="chip">Policy</span><span class="chip">EV Adoption</span></div>
        </div>
        <div class="article-source">
          <span>electrive • Today</span>
          <a href="https://www.electrive.com/2026/08/04/denmark-evs-account-for-almost-all-new-car-registrations-in-july/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">66</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/opinion/business-corporate/roof-boxes-top-car-accessory-market-defies-auto-downturn" target="_blank" rel="noopener">Accessory profits defy auto slowdown</a>
          <div class="article-take">Premium carriers and racks keep margins healthy even as car prices wobble.</div>
          <div class="article-tags"><span class="chip">Aftermarket</span><span class="chip">Retail</span></div>
        </div>
        <div class="article-source">
          <span>Autocar • Today</span>
          <a href="https://www.autocar.co.uk/car-news/opinion/business-corporate/roof-boxes-top-car-accessory-market-defies-auto-downturn" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="electric-vehicles">
    <h2 class="section-title">Electric Vehicles <span class="count">6 items</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip high">85</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/electric-cars/new-mercedes-gla-revealed-audi-q4-rival-408-mile-range" target="_blank" rel="noopener">Mercedes GLA EV debuts with 800V and long range</a>
          <div class="article-take">Compact luxury EVs continue to stretch capability and charging speeds.</div>
          <div class="article-tags"><span class="chip">Mercedes-Benz</span><span class="chip">GLA</span><span class="chip">EV</span></div>
        </div>
        <div class="article-source">
          <span>Autocar • Today</span>
          <a href="https://www.autocar.co.uk/car-news/electric-cars/new-mercedes-gla-revealed-audi-q4-rival-408-mile-range" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">75</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/28/volkswagen-launches-cheaper-id-polo-ev-orders-25000/" target="_blank" rel="noopener">VW opens orders for cheaper ID. Polo EV</a>
          <div class="article-take">Lower entry pricing broadens access to 300‑mile class EVs.</div>
          <div class="article-tags"><span class="chip">Volkswagen</span><span class="chip">Affordable EV</span></div>
        </div>
        <div class="article-source">
          <span>Electrek • Today</span>
          <a href="https://electrek.co/2026/07/28/volkswagen-launches-cheaper-id-polo-ev-orders-25000/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">78</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/28/bmw-ramps-up-ix3-output-orders-near-100000/" target="_blank" rel="noopener">BMW accelerates iX3 production on strong orderbook</a>
          <div class="article-take">Fastest ramp at Debrecen underscores demand for the new platform.</div>
          <div class="article-tags"><span class="chip">BMW</span><span class="chip">iX3</span><span class="chip">Production</span></div>
        </div>
        <div class="article-source">
          <span>Electrek • Today</span>
          <a href="https://electrek.co/2026/07/28/bmw-ramps-up-ix3-output-orders-near-100000/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">76</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/04/volvos-next-electric-suv-will-start-in-the-upper-40000-range/" target="_blank" rel="noopener">Volvo’s EX50 targets sub‑$50k price point</a>
          <div class="article-take">Aiming squarely at the heart of the US crossover segment.</div>
          <div class="article-tags"><span class="chip">Volvo</span><span class="chip">Pricing</span></div>
        </div>
        <div class="article-source">
          <span>Electrek • Today</span>
          <a href="https://electrek.co/2026/08/04/volvos-next-electric-suv-will-start-in-the-upper-40000-range/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">69</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/477795/" target="_blank" rel="noopener">EV sales surge back: where demand is strongest</a>
          <div class="article-take">Record quarters in 50 countries hint at regained consumer confidence.</div>
          <div class="article-tags"><span class="chip">Market</span><span class="chip">EV</span></div>
        </div>
        <div class="article-source">
          <span>Electrek • Today</span>
          <a href="https://electrek.co/2026/07/29/477795/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">71</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/audi-further-strips-a2-e-tron-of-its-camouflage/" target="_blank" rel="noopener">Audi A2 e‑tron: new details on range and efficiency</a>
          <div class="article-take">Audi’s entry EV sharpens aero and LFP strategy for daily use.</div>
          <div class="article-tags"><span class="chip">Audi</span><span class="chip">Efficiency</span><span class="chip">EV</span></div>
        </div>
        <div class="article-source">
          <span>electrive • Today</span>
          <a href="https://www.electrive.com/2026/08/04/audi-further-strips-a2-e-tron-of-its-camouflage/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="manufacturers">
    <h2 class="section-title">Manufacturers <span class="count">5 items</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip">82</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/audi-q9-suv-revealed-huge-%C2%A3100k-a8-successor" target="_blank" rel="noopener">Audi launches Q9 as luxury SUV flagship</a>
          <div class="article-take">Bigger than X7/GLS, the Q9 anchors Audi’s top‑end push.</div>
          <div class="article-tags"><span class="chip">Audi</span><span class="chip">SUV</span><span class="chip">Luxury</span></div>
        </div>
        <div class="article-source">
          <span>Autocar • Today</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/audi-q9-suv-revealed-huge-%C2%A3100k-a8-successor" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">73</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/04/new-porsche-boss-says-electric-718-is-still-coming-taycan-isnt-going-anywhere/" target="_blank" rel="noopener">Porsche CEO says electric 718 is back on track</a>
          <div class="article-take">Signals continued EV commitment alongside Taycan refresh cadence.</div>
          <div class="article-tags"><span class="chip">Porsche</span><span class="chip">EV Strategy</span></div>
        </div>
        <div class="article-source">
          <span>Electrek • Today</span>
          <a href="https://electrek.co/2026/08/04/new-porsche-boss-says-electric-718-is-still-coming-taycan-isnt-going-anywhere/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">73</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">BMW reevaluates late‑decade lineup</a>
          <div class="article-take">Market divergence pushes BMW toward tighter capital allocation.</div>
          <div class="article-tags"><span class="chip">BMW</span><span class="chip">Planning</span></div>
        </div>
        <div class="article-source">
          <span>Autocar • Today</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">70</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/03/hyundai-kias-record-us-sales-run/" target="_blank" rel="noopener">Hyundai & Kia extend record US sales streak on hybrids</a>
          <div class="article-take">Electrified trims keep momentum while EV capacity scales.</div>
          <div class="article-tags"><span class="chip">Hyundai</span><span class="chip">Kia</span><span class="chip">Sales</span></div>
        </div>
        <div class="article-source">
          <span>Electrek • Today</span>
          <a href="https://electrek.co/2026/08/03/hyundai-kias-record-us-sales-run/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">68</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/byd-goes-after-defender-boxy-%C2%A348k-402bhp-hybrid-suv" target="_blank" rel="noopener">BYD brings boxy Ti7 hybrid SUV to UK at £47,995</a>
          <div class="article-take">A rugged‑style seven‑seater undercuts legacy 4x4 rivals.</div>
          <div class="article-tags"><span class="chip">BYD</span><span class="chip">Hybrid</span><span class="chip">UK</span></div>
        </div>
        <div class="article-source">
          <span>Autocar • Today</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/byd-goes-after-defender-boxy-%C2%A348k-402bhp-hybrid-suv" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="dealers">
    <h2 class="section-title">Dealers <span class="count">2 items</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip">60</div>
        <div class="article-main">
          <a class="headline" href="https://www.carscoops.com/2026/08/costco-infiniti-discount/" target="_blank" rel="noopener">Costco offers discounts on new Infiniti SUVs, incl. QX65</a>
          <div class="article-take">Big‑box partnerships continue to funnel traffic to dealer lots.</div>
          <div class="article-tags"><span class="chip">Retail</span><span class="chip">Infiniti</span><span class="chip">Dealers</span></div>
        </div>
        <div class="article-source">
          <span>Carscoops • Today</span>
          <a href="https://www.carscoops.com/2026/08/costco-infiniti-discount/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">58</div>
        <div class="article-main">
          <a class="headline" href="https://www.carscoops.com/2026/08/servicemember-repossession-settlement/" target="_blank" rel="noopener">US DOJ settles with dealer for improper repossessions</a>
          <div class="article-take">Enforcement raises the stakes on compliance for auto retailers.</div>
          <div class="article-tags"><span class="chip">Dealers</span><span class="chip">Legal</span><span class="chip">US</span></div>
        </div>
        <div class="article-source">
          <span>Carscoops • Today</span>
          <a href="https://www.carscoops.com/2026/08/servicemember-repossession-settlement/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="suppliers">
    <h2 class="section-title">Suppliers <span class="count">4 items</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip">78</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">SK On + Factorial align on solid‑state scale‑up</a>
          <div class="article-take">Partnerships remain critical to cross the pilot‑to‑plant chasm.</div>
          <div class="article-tags"><span class="chip">Battery</span><span class="chip">Solid‑state</span></div>
        </div>
        <div class="article-source">
          <span>Electrek • Today</span>
          <a href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">69</div>
        <div class="article-main">
          <a class="headline" href="https://chargedevs.com/newswire/mahle-introduces-a-new-range-extender-engine-and-a-rare-earth-free-electric-motor/" target="_blank" rel="noopener">MAHLE debuts HD range‑extender, rare‑earth‑free e‑motor</a>
          <div class="article-take">Suppliers diversify solutions across battery and hybrid freight.</div>
          <div class="article-tags"><span class="chip">MAHLE</span><span class="chip">Powertrain</span></div>
        </div>
        <div class="article-source">
          <span>Charged EVs • Today</span>
          <a href="https://chargedevs.com/newswire/mahle-introduces-a-new-range-extender-engine-and-a-rare-earth-free-electric-motor/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">70</div>
        <div class="article-main">
          <a class="headline" href="https://chargedevs.com/newswire/beam-global-supplies-ev-arc-off-grid-charging-systems-for-dallas-municipal-fleet-and-massachusetts-carshare-pilot/" target="_blank" rel="noopener">Beam Global secures new municipal EV ARC orders</a>
          <div class="article-take">Off‑grid charging fills deployment gaps without utility delays.</div>
          <div class="article-tags"><span class="chip">Charging</span><span class="chip">Beam Global</span></div>
        </div>
        <div class="article-source">
          <span>Charged EVs • Today</span>
          <a href="https://chargedevs.com/newswire/beam-global-supplies-ev-arc-off-grid-charging-systems-for-dallas-municipal-fleet-and-massachusetts-carshare-pilot/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">65</div>
        <div class="article-main">
          <a class="headline" href="https://chargedevs.com/newswire/danisenses-new-current-transducer-measures-isolated-dc-and-ac-current-in-power-electronics/" target="_blank" rel="noopener">Danisense launches high‑precision DC/AC current transducer</a>
          <div class="article-take">Measurement fidelity improves EV power electronics design loops.</div>
          <div class="article-tags"><span class="chip">Components</span><span class="chip">Power Electronics</span></div>
        </div>
        <div class="article-source">
          <span>Charged EVs • Today</span>
          <a href="https://chargedevs.com/newswire/danisenses-new-current-transducer-measures-isolated-dc-and-ac-current-in-power-electronics/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="government">
    <h2 class="section-title">Government <span class="count">4 items</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip high">91</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">NHTSA probe targets 1.2M Teslas</a>
          <div class="article-take">A major US safety action centered on suspension integrity.</div>
          <div class="article-tags"><span class="chip">NHTSA</span><span class="chip">Safety</span><span class="chip">Tesla</span></div>
        </div>
        <div class="article-source">
          <span>Electrek • Today</span>
          <a href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">74</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/philippines-launches-e850m-incentive-programme-for-ev-manufacturing/" target="_blank" rel="noopener">Philippines launches EV manufacturing incentive scheme</a>
          <div class="article-take">A bid to capture regional EV and component investment.</div>
          <div class="article-tags"><span class="chip">Policy</span><span class="chip">Manufacturing</span></div>
        </div>
        <div class="article-source">
          <span>electrive • Today</span>
          <a href="https://www.electrive.com/2026/08/04/philippines-launches-e850m-incentive-programme-for-ev-manufacturing/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">71</div>
        <div class="article-main">
          <a class="headline" href="https://www.greencarreports.com/news/1146052_here-are-the-evs-made-in-mexico-and-canada" target="_blank" rel="noopener">Tariff uncertainty looms for Mexico/Canada‑built EVs</a>
          <div class="article-take">Policy could reshape pricing and sourcing in North America.</div>
          <div class="article-tags"><span class="chip">Tariffs</span><span class="chip">Trade</span><span class="chip">North America</span></div>
        </div>
        <div class="article-source">
          <span>Green Car Reports • Today</span>
          <a href="https://www.greencarreports.com/news/1146052_here-are-the-evs-made-in-mexico-and-canada" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">70</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/hyundai-kona-electric-now-qualifies-for-full-uk-electric-car-grant/" target="_blank" rel="noopener">Hyundai Kona Electric qualifies for full UK EV grant</a>
          <div class="article-take">Supply‑chain criteria unlock higher incentives for buyers.</div>
          <div class="article-tags"><span class="chip">Incentives</span><span class="chip">UK</span><span class="chip">Hyundai</span></div>
        </div>
        <div class="article-source">
          <span>electrive • Today</span>
          <a href="https://www.electrive.com/2026/08/04/hyundai-kona-electric-now-qualifies-for-full-uk-electric-car-grant/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="technology">
    <h2 class="section-title">Technology <span class="count">5 items</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip">80</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/waymo-gemini-ai-ojai-robotaxi-redesigned-interface/" target="_blank" rel="noopener">Waymo integrates Gemini AI into robotaxi UX</a>
          <div class="article-take">AI assistance becomes part of the passenger experience.</div>
          <div class="article-tags"><span class="chip">Autonomous</span><span class="chip">AI</span><span class="chip">Mobility</span></div>
        </div>
        <div class="article-source">
          <span>Electrek • Today</span>
          <a href="https://electrek.co/2026/07/29/waymo-gemini-ai-ojai-robotaxi-redesigned-interface/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">77</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Volvo ends lidar plan on two flagships, pays owners</a>
          <div class="article-take">A high‑profile sensor pivot reshapes ADAS roadmaps.</div>
          <div class="article-tags"><span class="chip">ADAS</span><span class="chip">Volvo</span><span class="chip">Sensors</span></div>
        </div>
        <div class="article-source">
          <span>Electrek • Today</span>
          <a href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">79</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/04/waymo-co-ceo-camera-only-self-driving-tesla/" target="_blank" rel="noopener">Waymo: camera‑only autonomy won’t reach needed safety</a>
          <div class="article-take">Sensor fusion remains the consensus path to full autonomy.</div>
          <div class="article-tags"><span class="chip">Waymo</span><span class="chip">Autonomy</span><span class="chip">Safety</span></div>
        </div>
        <div class="article-source">
          <span>Electrek • Today</span>
          <a href="https://electrek.co/2026/08/04/waymo-co-ceo-camera-only-self-driving-tesla/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">71</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/blue-solutions-and-avl-test-solid-state-battery-safety/" target="_blank" rel="noopener">AVL, Blue Solutions validate solid‑state safety behaviors</a>
          <div class="article-take">Thermal propagation tests set the stage for series development.</div>
          <div class="article-tags"><span class="chip">Battery</span><span class="chip">Safety</span><span class="chip">R&D</span></div>
        </div>
        <div class="article-source">
          <span>electrive • Today</span>
          <a href="https://www.electrive.com/2026/08/04/blue-solutions-and-avl-test-solid-state-battery-safety/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">70</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">Solid‑state alliance eyes mass‑market timelines</a>
          <div class="article-take">Consortia are converging on manufacturable chemistries and supply.</div>
          <div class="article-tags"><span class="chip">Solid‑state</span><span class="chip">Battery</span></div>
        </div>
        <div class="article-source">
          <span>Electrek • Today</span>
          <a href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="finance">
    <h2 class="section-title">Finance <span class="count">4 items</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip">84</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/30/rivian-rivn-q2-2026-earnings-r2-deliveries-revenue-up-27/" target="_blank" rel="noopener">Rivian beats on Q2 with record gross profit and R2 deliveries</a>
          <div class="article-take">Cost work and cheaper models are moving the margin needle.</div>
          <div class="article-tags"><span class="chip">Rivian</span><span class="chip">Earnings</span><span class="chip">Finance</span></div>
        </div>
        <div class="article-source">
          <span>Electrek • Today</span>
          <a href="https://electrek.co/2026/07/30/rivian-rivn-q2-2026-earnings-r2-deliveries-revenue-up-27/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">76</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/06/saudi-prince-alwaleed-5-percent-lucid-stake-lcid/" target="_blank" rel="noopener">Saudi Prince Alwaleed discloses 5% Lucid stake</a>
          <div class="article-take">Fresh capital confidence steadies sentiment around the EV startup.</div>
          <div class="article-tags"><span class="chip">Lucid</span><span class="chip">Investment</span></div>
        </div>
        <div class="article-source">
          <span>Electrek • Recent</span>
          <a href="https://electrek.co/2026/06/saudi-prince-alwaleed-5-percent-lucid-stake-lcid/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">72</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/30/tesla-10-millionth-vehicle-ev-growth-stalled/" target="_blank" rel="noopener">Tesla hits 10M vehicles as growth cools below capacity</a>
          <div class="article-take">A production milestone arrives alongside utilization questions.</div>
          <div class="article-tags"><span class="chip">Tesla</span><span class="chip">Production</span><span class="chip">Markets</span></div>
        </div>
        <div class="article-source">
          <span>Electrek • Recent</span>
          <a href="https://electrek.co/2026/07/30/tesla-10-millionth-vehicle-ev-growth-stalled/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">70</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/03/byd-boosts-sales-by-22-in-july/" target="_blank" rel="noopener">BYD July sales +22%, exports hold record share</a>
          <div class="article-take">Overseas growth offsets softness at home in China.</div>
          <div class="article-tags"><span class="chip">BYD</span><span class="chip">Sales</span><span class="chip">Exports</span></div>
        </div>
        <div class="article-source">
          <span>electrive • Today</span>
          <a href="https://www.electrive.com/2026/08/03/byd-boosts-sales-by-22-in-july/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="international">
    <h2 class="section-title">International <span class="count">4 items</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip">69</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/28/baidu-apollo-go-london-robotaxi-testing-uber-lyft/" target="_blank" rel="noopener">Baidu starts robotaxi tests in London with Uber/Lyft</a>
          <div class="article-take">A fast step from Hong Kong to Europe for Apollo Go.</div>
          <div class="article-tags"><span class="chip">Baidu</span><span class="chip">UK</span><span class="chip">Autonomous</span></div>
        </div>
        <div class="article-source">
          <span>Electrek • Today</span>
          <a href="https://electrek.co/2026/07/28/baidu-apollo-go-london-robotaxi-testing-uber-lyft/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">67</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/greenmobility-to-bring-weride-robotaxis-to-denmark/" target="_blank" rel="noopener">WeRide robotaxis headed to Denmark with GreenMobility</a>
          <div class="article-take">A new operator partnership pilots autonomous ride‑hailing in the Nordics.</div>
          <div class="article-tags"><span class="chip">WeRide</span><span class="chip">Denmark</span><span class="chip">Mobility</span></div>
        </div>
        <div class="article-source">
          <span>electrive • Today</span>
          <a href="https://www.electrive.com/2026/08/04/greenmobility-to-bring-weride-robotaxis-to-denmark/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      
      <div class="article-row">
        <div class="score-chip">72</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/04/tesla-china-sales-crash-exports-surge-h1-2026/" target="_blank" rel="noopener">Tesla China sales fall while exports surge 127%</a>
          <div class="article-take">Shanghai increasingly serves overseas demand as local rivals intensify.</div>
          <div class="article-tags"><span class="chip">Tesla</span><span class="chip">China</span><span class="chip">Exports</span></div>
        </div>
        <div class="article-source">
          <span>Electrek • Today</span>
          <a href="https://electrek.co/2026/08/04/tesla-china-sales-crash-exports-surge-h1-2026/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      
      <div class="article-row">
        <div class="score-chip">70</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/03/norways-ev-share-rises-to-97-6-in-july/" target="_blank" rel="noopener">Norway: EVs reach 97.6% of July private registrations</a>
          <div class="article-take">The world’s leading EV market keeps breaking records.</div>
          <div class="article-tags"><span class="chip">Norway</span><span class="chip">EV Share</span><span class="chip">Policy</span></div>
        </div>
        <div class="article-source">
          <span>electrive • Today</span>
          <a href="https://www.electrive.com/2026/08/03/norways-ev-share-rises-to-97-6-in-july/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      
    </div>
  </div>

  <div class="sec-group reveal" id="opinion">
    <h2 class="section-title">Opinion <span class="count">3 items</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip">66</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/opinion/business-corporate/roof-boxes-top-car-accessory-market-defies-auto-downturn" target="_blank" rel="noopener">Accessory profits defy the auto downturn</a>
          <div class="article-take">Premium hardware can be resilient even when car margins compress.</div>
          <div class="article-tags"><span class="chip">Aftermarket</span><span class="chip">Strategy</span></div>
        </div>
        <div class="article-source">
          <span>Autocar • Today</span>
          <a href="https://www.autocar.co.uk/car-news/opinion/business-corporate/roof-boxes-top-car-accessory-market-defies-auto-downturn" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      
      <div class="article-row">
        <div class="score-chip">64</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/opinion/new-cars/ignore-jay-leno-your-dream-garage-only-needs-three-cars" target="_blank" rel="noopener">Your dream garage only needs three cars</a>
          <div class="article-take">A case for fewer vehicles and more use, not museum fleets.</div>
          <div class="article-tags"><span class="chip">Opinion</span><span class="chip">Culture</span></div>
        </div>
        <div class="article-source">
          <span>Autocar • Today</span>
          <a href="https://www.autocar.co.uk/opinion/new-cars/ignore-jay-leno-your-dream-garage-only-needs-three-cars" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      
      <div class="article-row">
        <div class="score-chip">68</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/business-manufacturing/chinese-car-makers-all-share-parts-will-world-follow" target="_blank" rel="noopener">China’s parts standardization: will the world follow?</a>
          <div class="article-take">Shared tooling and commoditized parts slash cost and time to market.</div>
          <div class="article-tags"><span class="chip">China</span><span class="chip">Supply Chain</span><span class="chip">Strategy</span></div>
        </div>
        <div class="article-source">
          <span>Autocar • Today</span>
          <a href="https://www.autocar.co.uk/car-news/business-manufacturing/chinese-car-makers-all-share-parts-will-world-follow" target="_blank" rel="noopener">Read original →</a>
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