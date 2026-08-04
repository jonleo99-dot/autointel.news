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
        <h1>NHTSA opens probe into 1.2 million Teslas over suspension failures</h1>
        <p class="exec-summary">US regulators launched a large-scale safety investigation into Model 3 and Model Y front suspension links detaching while driving. The probe targets core volume years and could culminate in a recall, new supplier controls, or design changes—affecting service costs and Tesla’s quality narrative at a sensitive moment for the brand.</p>

        <div class="takeaways">
          <h3>Key Takeaways</h3>
          <ul>
            
            <!-- repeat: <li>{{TAKEAWAY}}</li> -->
          </ul>
        </div>

        <div class="impact-row">
          <div class="impact-block">
            <h4>Industry Impact</h4>
            <p>Safety scrutiny on EV suspension durability will spill over to peers, raising the bar for validation and field monitoring. For Tesla, the outcome may drive warranty accruals and add friction to its cost-down roadmap just as competition intensifies in China and margins tighten. Suppliers will feel pressure to harden traceability and fatigue testing on high-volume chassis parts.</p>
          </div>
          <div class="impact-block">
            <h4>Companies Affected</h4>
            <div class="chip-row">
              <span class="chip entity-mfr">Tesla</span>
              <span class="chip">NHTSA</span>
              <span class="chip">Model 3</span>
              <span class="chip">Model Y</span>
              <span class="chip">Safety</span>
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
            <li><a href="https://www.electrive.com/2026/08/03/nhtsa-opens-probe-into-1-2-million-teslas/" target="_blank" rel="noopener">NHTSA launches preliminary evaluation into 1.2M Tesla Model 3/Y</a></li>
            <li><a href="https://electrek.co/2026/08/03/tesla-fsd-v14-lite-hw3-computer-failures/" target="_blank" rel="noopener">Owners report Autopilot computer overheating after FSD v14 Lite</a></li>
            <li><a href="https://electrek.co/2026/08/04/tesla-china-sales-crash-exports-surge-h1-2026/" target="_blank" rel="noopener">Tesla China sales slide while exports surge from Shanghai</a></li>
          </ul>
        </div>
      </div>

      <div class="hero-gauges">
        <div class="gauge">
          <svg viewBox="0 0 120 70"><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#2a3038" stroke-width="8"/><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#f2a93b" stroke-width="8" stroke-dasharray="157" stroke-dashoffset="11.0"/></svg>
          <span class="gauge-value mono">93</span>
          <span class="gauge-label">Importance</span>
        </div>
        <div class="gauge">
          <svg viewBox="0 0 120 70"><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#2a3038" stroke-width="8"/><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#3ecf8e" stroke-width="8" stroke-dasharray="157" stroke-dashoffset="18.8"/></svg>
          <span class="gauge-value mono">88</span>
          <span class="gauge-label">Editorial Quality</span>
        </div>
        <div class="gauge">
          <svg viewBox="0 0 120 70"><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#2a3038" stroke-width="8"/><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#e2604f" stroke-width="8" stroke-dasharray="157" stroke-dashoffset="15.7"/></svg>
          <span class="gauge-value mono">90</span>
          <span class="gauge-label">Industry Impact</span>
        </div>
        <div class="gauge">
          <svg viewBox="0 0 120 70"><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#2a3038" stroke-width="8"/><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#f2a93b" stroke-width="8" stroke-dasharray="157" stroke-dashoffset="23.6"/></svg>
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
    <h2 class="section-title">Industry Snapshot <span class="count">Last 24 hours</span></h2>
    <div class="dash-grid">
      
      <div class="stat-panel">
        <h4>Top Manufacturers</h4>
        <ul class="rank-list">
          <li><span>Tesla</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:100%"></div></div><span class="rank-count">12</span></li>
          <li><span>BYD</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:88%"></div></div><span class="rank-count">11</span></li>
          <li><span>Mercedes-Benz</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:75%"></div></div><span class="rank-count">9</span></li>
          <li><span>BMW</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:71%"></div></div><span class="rank-count">8</span></li>
          <li><span>Hyundai</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:67%"></div></div><span class="rank-count">8</span></li>
          <li><span>Audi</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:58%"></div></div><span class="rank-count">7</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4>Top Brands</h4>
        <ul class="rank-list">
          <li><span>Genesis</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:82%"></div></div><span class="rank-count">9</span></li>
          <li><span>Volkswagen</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:73%"></div></div><span class="rank-count">8</span></li>
          <li><span>Volvo</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:55%"></div></div><span class="rank-count">6</span></li>
          <li><span>Ram</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:45%"></div></div><span class="rank-count">5</span></li>
          <li><span>Porsche</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:45%"></div></div><span class="rank-count">5</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4>Top Suppliers & Networks</h4>
        <ul class="rank-list">
          <li><span>Luminar</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:100%"></div></div><span class="rank-count">6</span></li>
          <li><span>SK On</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:83%"></div></div><span class="rank-count">5</span></li>
          <li><span>Factorial Energy</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:67%"></div></div><span class="rank-count">4</span></li>
          <li><span>EVgo</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:67%"></div></div><span class="rank-count">4</span></li>
          <li><span>Allego</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:50%"></div></div><span class="rank-count">3</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4>Most Mentioned Executives</h4>
        <ul class="rank-list">
          <li><span>Elon Musk (Tesla)</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:100%"></div></div><span class="rank-count">8</span></li>
          <li><span>Ola Källenius (Mercedes)</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:75%"></div></div><span class="rank-count">6</span></li>
          <li><span>RJ Scaringe (Rivian)</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:63%"></div></div><span class="rank-count">5</span></li>
          <li><span>Michael Leiters (Porsche)</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:50%"></div></div><span class="rank-count">4</span></li>
          <li><span>Dmitri Dolgov (Waymo)</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:50%"></div></div><span class="rank-count">4</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4>Trending Topics</h4>
        <div class="tagcloud">
          <span class="chip lg">Recalls & Safety</span>
          <span class="chip lg">Solid‑state batteries</span>
          <span class="chip">Lidar strategy</span>
          <span class="chip">Fast charging</span>
          <span class="chip">Robotaxis</span>
          <span class="chip">EV affordability</span>
          <span class="chip">Software‑defined vehicles</span>
          <span class="chip">Tariffs & trade</span>
          <span class="chip">Record EV shares</span>
        </div>
      </div>

      <div class="stat-panel">
        <h4>Emerging Technologies</h4>
        <div class="tagcloud">
          <span class="chip lg">Iron‑air storage</span>
          <span class="chip">Camera vs lidar</span>
          <span class="chip">AI in-vehicle assistants</span>
          <span class="chip">Long‑duration storage</span>
          <span class="chip">V2X / VPP</span>
          <span class="chip">800V platforms</span>
          <span class="chip">High‑nickel alternatives (LFP)</span>
        </div>
      </div>

      <div class="stat-panel">
        <h4>Government & Regulation</h4>
        <ul class="rank-list">
          <li><span>NHTSA Tesla suspension probe</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:100%"></div></div><span class="rank-count">1</span></li>
          <li><span>Philippines EV incentives</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:75%"></div></div><span class="rank-count">1</span></li>
          <li><span>UK/Denmark EV grant & share</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:63%"></div></div><span class="rank-count">2</span></li>
          <li><span>California charging buildout</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:50%"></div></div><span class="rank-count">1</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4>Supplier & Network Activity</h4>
        <ul class="rank-list">
          <li><span>Volvo drops Luminar lidar</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:100%"></div></div><span class="rank-count">1</span></li>
          <li><span>SK On + Factorial alliance</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:83%"></div></div><span class="rank-count">1</span></li>
          <li><span>EVgo + Brixmor 500 stalls</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:75%"></div></div><span class="rank-count">1</span></li>
          <li><span>Allego UK expansion</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:63%"></div></div><span class="rank-count">1</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4>Financial & Market Signals</h4>
        <ul class="rank-list">
          <li><span>Rivian Q2: revenue +27%</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:100%"></div></div><span class="rank-count">1</span></li>
          <li><span>Lucid +5% stake disclosure</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:83%"></div></div><span class="rank-count">1</span></li>
          <li><span>Base Power raises $1B</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:75%"></div></div><span class="rank-count">1</span></li>
          <li><span>BYD July sales +22%</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:70%"></div></div><span class="rank-count">1</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4>Global Regions in Focus</h4>
        <div class="tagcloud">
          <span class="chip lg">United States</span>
          <span class="chip lg">China</span>
          <span class="chip">United Kingdom</span>
          <span class="chip">European Union</span>
          <span class="chip">Nordics</span>
          <span class="chip">Mexico</span>
          <span class="chip">Canada</span>
          <span class="chip">Southeast Asia</span>
        </div>
      </div>

      <!-- repeat one .stat-panel block per snapshot metric, e.g.: -->
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
        <a href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">BMW puts G‑Class rival on hold amid China headwinds</a>
        <div class="fp-meta"><span>Autocar</span><span>Aug 4, 2026</span><span>Score 82</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/new-mercedes-gla-ev-bigger-400-miles-range/" target="_blank" rel="noopener">Mercedes unveils new GLA EV with 400+ mile range</a>
        <div class="fp-meta"><span>Electrek</span><span>Jul 29, 2026</span><span>Score 80</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.autocar.co.uk/car-news/new-cars/audi-q9-suv-revealed-huge-%C2%A3100k-a8-successor" target="_blank" rel="noopener">Audi reveals Q9 flagship SUV as A8 successor</a>
        <div class="fp-meta"><span>Autocar</span><span>Aug 1, 2026</span><span>Score 78</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/08/04/hyundai-kias-record-us-sales-run/" target="_blank" rel="noopener">Hyundai and Kia extend US sales records on hybrids</a>
        <div class="fp-meta"><span>Electrek</span><span>Aug 4, 2026</span><span>Score 76</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/31/byd-undercuts-defender-first-7-seat-suv-uk/" target="_blank" rel="noopener">BYD brings boxy 7‑seat Ti 7 to UK at aggressive price</a>
        <div class="fp-meta"><span>Electrek</span><span>Jul 31, 2026</span><span>Score 74</span></div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Technology</h3>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Volvo drops lidar on EX90/ES90 and compensates owners</a>
        <div class="fp-meta"><span>Electrek</span><span>Jul 29, 2026</span><span>Score 89</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">SK On and Factorial team up to scale solid‑state batteries</a>
        <div class="fp-meta"><span>Electrek</span><span>Jul 29, 2026</span><span>Score 84</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/waymo-gemini-ai-ojai-robotaxi-redesigned-interface/" target="_blank" rel="noopener">Waymo integrates Google Gemini into next‑gen robotaxi UI</a>
        <div class="fp-meta"><span>Electrek</span><span>Jul 29, 2026</span><span>Score 79</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.electrive.com/2026/08/03/blue-solutions-and-avl-test-solid-state-battery-safety/" target="_blank" rel="noopener">AVL, Blue Solutions validate solid‑state safety measures</a>
        <div class="fp-meta"><span>electrive</span><span>Aug 3, 2026</span><span>Score 72</span></div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Government</h3>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">NHTSA opens safety probe into 1.2M Teslas</a>
        <div class="fp-meta"><span>Electrek</span><span>Jul 31, 2026</span><span>Score 93</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.electrive.com/2026/08/04/philippines-launches-e850m-incentive-programme-for-ev-manufacturing/" target="_blank" rel="noopener">Philippines launches €850m EV manufacturing incentives</a>
        <div class="fp-meta"><span>electrive</span><span>Aug 4, 2026</span><span>Score 78</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.electrive.com/2026/08/04/denmark-evs-account-for-almost-all-new-car-registrations-in-july/" target="_blank" rel="noopener">Denmark: EVs hit 97% of private registrations in July</a>
        <div class="fp-meta"><span>electrive</span><span>Aug 4, 2026</span><span>Score 75</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.greencarreports.com/news/1146045_california-has-nearly-50-more-public-ev-chargers-than-gas-nozzles" target="_blank" rel="noopener">California now has far more public EV plugs than gas nozzles</a>
        <div class="fp-meta"><span>Green Car Reports</span><span>Aug 3, 2026</span><span>Score 74</span></div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Suppliers & Infrastructure</h3>
      <div class="fp-row">
        <a href="https://electrek.co/2026/08/04/evgo-and-brixmor-to-add-more-than-500-fast-charging-stalls-in-the-us/" target="_blank" rel="noopener">EVgo, Brixmor to add 500+ DCFC stalls at shopping centers</a>
        <div class="fp-meta"><span>electrive (link via Electrek)</span><span>Aug 4, 2026</span><span>Score 77</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.electrive.com/2026/08/01/allego-commits-e100-million-to-expand-uk-charging-network/" target="_blank" rel="noopener">Allego earmarks €100m for 1,400 UK ultra‑rapid chargers</a>
        <div class="fp-meta"><span>electrive</span><span>Aug 1, 2026</span><span>Score 73</span></div>
      </div>
      <div class="fp-row">
        <a href="https://chargedevs.com/newswire/beam-global-supplies-ev-arc-off-grid-charging-systems-for-dallas-municipal-fleet-and-massachusetts-carshare-pilot/" target="_blank" rel="noopener">Beam Global lands new EV ARC municipal and carshare orders</a>
        <div class="fp-meta"><span>Charged EVs</span><span>Aug 2, 2026</span><span>Score 70</span></div>
      </div>
      <div class="fp-row">
        <a href="https://chargedevs.com/newswire/mahle-introduces-a-new-range-extender-engine-and-a-rare-earth-free-electric-motor/" target="_blank" rel="noopener">MAHLE unveils HD range‑extender and rare‑earth‑free e‑motor</a>
        <div class="fp-meta"><span>Charged EVs</span><span>Aug 3, 2026</span><span>Score 68</span></div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Trending Topics</h3>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">OEMs rethinking lidar vs. camera stacks</a>
        <div class="fp-meta"><span>Volvo case</span><span>Jul 29, 2026</span><span>Score 89</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">Solid‑state alliances accelerate scale‑up</a>
        <div class="fp-meta"><span>Battery</span><span>Jul 29, 2026</span><span>Score 84</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.electrive.com/2026/08/04/denmark-evs-account-for-almost-all-new-car-registrations-in-july/" target="_blank" rel="noopener">Nordic EV penetration records continue</a>
        <div class="fp-meta"><span>Market</span><span>Aug 4, 2026</span><span>Score 75</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">Safety probes test EV durability claims</a>
        <div class="fp-meta"><span>Regulation</span><span>Jul 31, 2026</span><span>Score 93</span></div>
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
        <div class="score-chip high">93</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">NHTSA probes 1.2M Tesla Model 3/Y over suspension failures</a>
          <div class="article-take">A large federal safety review puts Tesla’s high‑volume cars under the microscope and could trigger costly fixes.</div>
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
        <div class="score-chip high">89</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Volvo drops lidar on EX90/ES90 and pays owner compensation</a>
          <div class="article-take">Shifting away from lidar resets Volvo’s ADAS roadmap and pressures lidar suppliers to prove value at scale.</div>
          <div class="article-tags">
            <span class="chip">Volvo</span><span class="chip">ADAS</span><span class="chip">Lidar</span><span class="chip">Software</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">84</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">SK On and Factorial ally to scale solid‑state batteries</a>
          <div class="article-take">The tie‑up pairs deep cell IP with manufacturing heft to push solid‑state from pilot to production.</div>
          <div class="article-tags">
            <span class="chip">Battery</span><span class="chip">Solid‑state</span><span class="chip">SK On</span><span class="chip">Factorial</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      
      <div class="article-row">
        <div class="score-chip">82</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">BMW pauses G‑Class rival as China headwinds mount</a>
          <div class="article-take">Mixed regional demand and tariff risk are forcing BMW to recalibrate future product bets.</div>
          <div class="article-tags">
            <span class="chip">BMW</span><span class="chip">Manufacturing</span><span class="chip">Strategy</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 4, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      
      <div class="article-row">
        <div class="score-chip">80</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/new-mercedes-gla-ev-bigger-400-miles-range/" target="_blank" rel="noopener">New Mercedes GLA EV gains space, 400+ mile range</a>
          <div class="article-take">Mercedes pushes efficiency and charging speed down‑segment to keep entry EVs competitive.</div>
          <div class="article-tags">
            <span class="chip">Mercedes-Benz</span><span class="chip">EV</span><span class="chip">Range</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/new-mercedes-gla-ev-bigger-400-miles-range/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      
      <div class="article-row">
        <div class="score-chip">79</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/waymo-gemini-ai-ojai-robotaxi-redesigned-interface/" target="_blank" rel="noopener">Waymo adds Google Gemini and new UI to Ojai robotaxi</a>
          <div class="article-take">Conversational AI moves into the ride experience, signaling the next UX battleground for AVs.</div>
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
        <div class="score-chip">78</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/audi-q9-suv-revealed-huge-%C2%A3100k-a8-successor" target="_blank" rel="noopener">Audi unveils Q9, an “unapologetically high‑status” SUV</a>
          <div class="article-take">Audi doubles down on full‑size luxury as US and Middle East drive demand for seven‑seat flagships.</div>
          <div class="article-tags">
            <span class="chip">Audi</span><span class="chip">SUV</span><span class="chip">Luxury</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 1, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/audi-q9-suv-revealed-huge-%C2%A3100k-a8-successor" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      

      <div class="article-row">
        <div class="score-chip">77</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/04/evgo-and-brixmor-to-add-more-than-500-fast-charging-stalls-in-the-us/" target="_blank" rel="noopener">EVgo and Brixmor to build 500+ fast‑charging stalls in US</a>
          <div class="article-take">Retail‑site DCFC growth keeps pace with mainstream EV adoption and expands urban reliability.</div>
          <div class="article-tags">
            <span class="chip">Charging</span><span class="chip">EVgo</span><span class="chip">Retail</span>
          </div>
        </div>
        <div class="article-source">
          <span>electrive — Aug 4, 2026</span>
          <a href="https://electrek.co/2026/08/04/evgo-and-brixmor-to-add-more-than-500-fast-charging-stalls-in-the-us/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      

      <div class="article-row">
        <div class="score-chip">76</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/04/hyundai-kias-record-us-sales-run/" target="_blank" rel="noopener">Hyundai, Kia extend US sales streak as hybrids surge</a>
          <div class="article-take">Affordable hybrids are bridging shoppers to electrification and cushioning macro volatility.</div>
          <div class="article-tags">
            <span class="chip">Hybrids</span><span class="chip">Hyundai</span><span class="chip">Kia</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 4, 2026</span>
          <a href="https://electrek.co/2026/08/04/hyundai-kias-record-us-sales-run/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      

      <div class="article-row">
        <div class="score-chip">75</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/denmark-evs-account-for-almost-all-new-car-registrations-in-july/" target="_blank" rel="noopener">Denmark: EVs hit 97.6% of private registrations in July</a>
          <div class="article-take">Policy, product, and charging alignment show what a near‑complete market flip looks like.</div>
          <div class="article-tags">
            <span class="chip">Denmark</span><span class="chip">EV share</span><span class="chip">Policy</span>
          </div>
        </div>
        <div class="article-source">
          <span>electrive — Aug 4, 2026</span>
          <a href="https://www.electrive.com/2026/08/04/denmark-evs-account-for-almost-all-new-car-registrations-in-july/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      

      <div class="article-row">
        <div class="score-chip">74</div>
        <div class="article-main">
          <a class="headline" href="https://www.greencarreports.com/news/1146045_california-has-nearly-50-more-public-ev-chargers-than-gas-nozzles" target="_blank" rel="noopener">California now has nearly 50% more public EV chargers than gas nozzles</a>
          <div class="article-take">Public charging density is reaching critical mass in the US’s biggest EV market.</div>
          <div class="article-tags">
            <span class="chip">Charging</span><span class="chip">California</span><span class="chip">Infrastructure</span>
          </div>
        </div>
        <div class="article-source">
          <span>Green Car Reports — Aug 3, 2026</span>
          <a href="https://www.greencarreports.com/news/1146045_california-has-nearly-50-more-public-ev-chargers-than-gas-nozzles" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      

      <div class="article-row">
        <div class="score-chip">73</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/01/allego-commits-e100-million-to-expand-uk-charging-network/" target="_blank" rel="noopener">Allego commits €100m to expand UK ultra‑rapid charging</a>
          <div class="article-take">Capital flows continue into strategic corridors as UK ramps affordable mass‑market EVs.</div>
          <div class="article-tags">
            <span class="chip">Allego</span><span class="chip">UK</span><span class="chip">Fast Charging</span>
          </div>
        </div>
        <div class="article-source">
          <span>electrive — Aug 1, 2026</span>
          <a href="https://www.electrive.com/2026/08/01/allego-commits-e100-million-to-expand-uk-charging-network/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      

      <div class="article-row">
        <div class="score-chip">72</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/03/blue-solutions-and-avl-test-solid-state-battery-safety/" target="_blank" rel="noopener">AVL and Blue Solutions test solid‑state safety scenarios</a>
          <div class="article-take">Thermal propagation work is a prerequisite for certifying next‑gen cells in volume vehicles.</div>
          <div class="article-tags">
            <span class="chip">Battery</span><span class="chip">Safety</span><span class="chip">Solid‑state</span>
          </div>
        </div>
        <div class="article-source">
          <span>electrive — Aug 3, 2026</span>
          <a href="https://www.electrive.com/2026/08/03/blue-solutions-and-avl-test-solid-state-battery-safety/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      

      <div class="article-row">
        <div class="score-chip">71</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/04/waymo-co-ceo-camera-only-self-driving-tesla/" target="_blank" rel="noopener">Waymo CEO argues camera‑only autonomy won’t reach superhuman safety</a>
          <div class="article-take">The sensor‑stack debate heats up as AV players defend divergent technical paths.</div>
          <div class="article-tags">
            <span class="chip">Autonomous</span><span class="chip">Waymo</span><span class="chip">Sensors</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 4, 2026</span>
          <a href="https://electrek.co/2026/08/04/waymo-co-ceo-camera-only-self-driving-tesla/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      

      <div class="article-row">
        <div class="score-chip">70</div>
        <div class="article-main">
          <a class="headline" href="https://chargedevs.com/newswire/beam-global-supplies-ev-arc-off-grid-charging-systems-for-dallas-municipal-fleet-and-massachusetts-carshare-pilot/" target="_blank" rel="noopener">Beam Global ships more off‑grid solar EV ARC systems</a>
          <div class="article-take">Rapid‑deploy chargers offer a workaround for grid‑constrained municipal sites.</div>
          <div class="article-tags">
            <span class="chip">Charging</span><span class="chip">Municipal</span><span class="chip">Solar</span>
          </div>
        </div>
        <div class="article-source">
          <span>Charged EVs — Aug 2, 2026</span>
          <a href="https://chargedevs.com/newswire/beam-global-supplies-ev-arc-off-grid-charging-systems-for-dallas-municipal-fleet-and-massachusetts-carshare-pilot/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      

      <div class="article-row">
        <div class="score-chip">69</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/04/tesla-fsd-v14-lite-hw3-computer-failures/" target="_blank" rel="noopener">Owners report FSD v14 ‘Lite’ tied to HW3 computer issues</a>
          <div class="article-take">Thermal stress on legacy compute hints at rising software loads meeting hardware limits.</div>
          <div class="article-tags">
            <span class="chip">Tesla</span><span class="chip">Software</span><span class="chip">Autopilot</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 4, 2026</span>
          <a href="https://electrek.co/2026/08/03/tesla-fsd-v14-lite-hw3-computer-failures/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      

      <div class="article-row">
        <div class="score-chip">68</div>
        <div class="article-main">
          <a class="headline" href="https://chargedevs.com/newswire/mahle-introduces-a-new-range-extender-engine-and-a-rare-earth-free-electric-motor/" target="_blank" rel="noopener">MAHLE debuts HD truck range‑extender and rare‑earth‑free motor</a>
          <div class="article-take">Suppliers are carving pathways for long‑haul zero‑emission duty cycles without exotic materials.</div>
          <div class="article-tags">
            <span class="chip">Suppliers</span><span class="chip">Trucks</span><span class="chip">Powertrain</span>
          </div>
        </div>
        <div class="article-source">
          <span>Charged EVs — Aug 3, 2026</span>
          <a href="https://chargedevs.com/newswire/mahle-introduces-a-new-range-extender-engine-and-a-rare-earth-free-electric-motor/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      

      <div class="article-row">
        <div class="score-chip">67</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/31/byd-undercuts-defender-first-7-seat-suv-uk/" target="_blank" rel="noopener">BYD launches Ti 7 seven‑seat SUV in UK below Defender PHEV</a>
          <div class="article-take">Aggressive pricing keeps pressure on legacy SUVs as Chinese brands expand lineups.</div>
          <div class="article-tags">
            <span class="chip">BYD</span><span class="chip">SUV</span><span class="chip">Pricing</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 31, 2026</span>
          <a href="https://electrek.co/2026/07/31/byd-undercuts-defender-first-7-seat-suv-uk/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      

      <div class="article-row">
        <div class="score-chip">66</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/04/tesla-china-sales-crash-exports-surge-h1-2026/" target="_blank" rel="noopener">Tesla China sales fall as Shanghai exports surge</a>
          <div class="article-take">Shanghai is operating as an export hub while domestic share softens under heavy local competition.</div>
          <div class="article-tags">
            <span class="chip">Tesla</span><span class="chip">China</span><span class="chip">Exports</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 4, 2026</span>
          <a href="https://electrek.co/2026/08/04/tesla-china-sales-crash-exports-surge-h1-2026/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      

      <div class="article-row">
        <div class="score-chip">65</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/30/rivian-rivn-q2-2026-earnings-r2-deliveries-revenue-up-27/" target="_blank" rel="noopener">Rivian revenue up 27% YoY; R2 deliveries begin</a>
          <div class="article-take">Scaling a sub‑$50k model is giving Rivian a clearer path toward margin improvement.</div>
          <div class="article-tags">
            <span class="chip">Rivian</span><span class="chip">Earnings</span><span class="chip">Production</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 30, 2026</span>
          <a href="https://electrek.co/2026/07/30/rivian-rivn-q2-2026-earnings-r2-deliveries-revenue-up-27/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      

      <div class="article-row">
        <div class="score-chip">64</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/new-models-vital-ds-survival-uk-sales-hit-record-low" target="_blank" rel="noopener">DS sales slump in UK; new models key to survival</a>
          <div class="article-take">A product reset and brand repositioning are urgent as volumes fall to record lows.</div>
          <div class="article-tags">
            <span class="chip">DS Automobiles</span><span class="chip">Sales</span><span class="chip">Strategy</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 4, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/new-models-vital-ds-survival-uk-sales-hit-record-low" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      

      <div class="article-row">
        <div class="score-chip">63</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/03/nice-opens-former-mobilize-share-charging-network-to-public/" target="_blank" rel="noopener">Nice converts former Mobilize Share chargers to public network</a>
          <div class="article-take">Repurposing car‑share infrastructure is a quick win for urban public charging coverage.</div>
          <div class="article-tags">
            <span class="chip">Charging</span><span class="chip">France</span><span class="chip">City</span>
          </div>
        </div>
        <div class="article-source">
          <span>electrive — Aug 4, 2026</span>
          <a href="https://www.electrive.com/2026/08/03/nice-opens-former-mobilize-share-charging-network-to-public/" target="_blank" rel="noopener">Read original →</a>
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
    <h2 class="section-title">Industry News <span class="count">Top trends</span></h2>
    <div class="article-table">
      
      <div class="article-row">
        <div class="score-chip high">93</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">NHTSA probes 1.2M Teslas over suspension issues</a>
          <div class="article-take">A sweeping US safety action could reshape warranty costs and supplier controls.</div>
          <div class="article-tags">
            <span class="chip">Safety</span><span class="chip">Tesla</span><span class="chip">Regulation</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 31, 2026</span>
          <a href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      

      <div class="article-row">
        <div class="score-chip">82</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">BMW pauses off‑roader as China market shifts</a>
          <div class="article-take">Diverging global demand is forcing portfolio triage at premium OEMs.</div>
          <div class="article-tags">
            <span class="chip">BMW</span><span class="chip">China</span><span class="chip">Strategy</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 4, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      

      <div class="article-row">
        <div class="score-chip">65</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/30/rivian-rivn-q2-2026-earnings-r2-deliveries-revenue-up-27/" target="_blank" rel="noopener">Rivian grows revenue as R2 enters deliveries</a>
          <div class="article-take">A lower‑price vehicle is unlocking scale and improving unit economics.</div>
          <div class="article-tags">
            <span class="chip">Rivian</span><span class="chip">Earnings</span><span class="chip">Production</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 30, 2026</span>
          <a href="https://electrek.co/2026/07/30/rivian-rivn-q2-2026-earnings-r2-deliveries-revenue-up-27/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      

    </div>
  </div>

  <div class="sec-group reveal" id="electric-vehicles">
    <h2 class="section-title">Electric Vehicles <span class="count">Product & adoption</span></h2>
    <div class="article-table">
      
      <div class="article-row">
        <div class="score-chip">80</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/new-mercedes-gla-ev-bigger-400-miles-range/" target="_blank" rel="noopener">Mercedes GLA EV revealed with 400+ mile range</a>
          <div class="article-take">High‑efficiency compact EVs are raising expectations for entry segments.</div>
          <div class="article-tags">
            <span class="chip">EV</span><span class="chip">Mercedes-Benz</span><span class="chip">Range</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/new-mercedes-gla-ev-bigger-400-miles-range/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      

      <div class="article-row">
        <div class="score-chip">75</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/denmark-evs-account-for-almost-all-new-car-registrations-in-july/" target="_blank" rel="noopener">Denmark nears all‑EV private market in July</a>
          <div class="article-take">A preview of end‑state adoption when incentives, choice, and charging align.</div>
          <div class="article-tags">
            <span class="chip">Market</span><span class="chip">Denmark</span><span class="chip">EV adoption</span>
          </div>
        </div>
        <div class="article-source">
          <span>electrive — Aug 4, 2026</span>
          <a href="https://www.electrive.com/2026/08/04/denmark-evs-account-for-almost-all-new-car-registrations-in-july/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      

      <div class="article-row">
        <div class="score-chip">67</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/31/byd-undercuts-defender-first-7-seat-suv-uk/" target="_blank" rel="noopener">BYD’s Ti 7 seven‑seater lands in UK undercutting rivals</a>
          <div class="article-take">Price pressure intensifies as Chinese OEMs broaden body styles.</div>
          <div class="article-tags">
            <span class="chip">BYD</span><span class="chip">SUV</span><span class="chip">Pricing</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 31, 2026</span>
          <a href="https://electrek.co/2026/07/31/byd-undercuts-defender-first-7-seat-suv-uk/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      

    </div>
  </div>

  <div class="sec-group reveal" id="manufacturers">
    <h2 class="section-title">Manufacturers <span class="count">Strategy & launches</span></h2>
    <div class="article-table">
      
      <div class="article-row">
        <div class="score-chip">82</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">BMW reassesses model plans, puts G‑Class rival on ice</a>
          <div class="article-take">Macro headwinds in China are reshaping product prioritization.</div>
          <div class="article-tags">
            <span class="chip">BMW</span><span class="chip">Portfolio</span><span class="chip">China</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 4, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      

      <div class="article-row">
        <div class="score-chip">78</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/audi-q9-suv-revealed-huge-%C2%A3100k-a8-successor" target="_blank" rel="noopener">Audi Q9 becomes the new upper‑range flagship</a>
          <div class="article-take">Premium brands continue chasing high‑margin full‑size SUVs.</div>
          <div class="article-tags">
            <span class="chip">Audi</span><span class="chip">SUV</span><span class="chip">Luxury</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 1, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/audi-q9-suv-revealed-huge-%C2%A3100k-a8-successor" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      

      <div class="article-row">
        <div class="score-chip">76</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/04/hyundai-kias-record-us-sales-run/" target="_blank" rel="noopener">Hyundai & Kia post another US sales record</a>
          <div class="article-take">Balanced hybrid/EV mix is paying off in a cautious demand cycle.</div>
          <div class="article-tags">
            <span class="chip">Hyundai</span><span class="chip">Kia</span><span class="chip">Sales</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 4, 2026</span>
          <a href="https://electrek.co/2026/08/04/hyundai-kias-record-us-sales-run/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      

    </div>
  </div>

  <div class="sec-group reveal" id="dealers">
    <h2 class="section-title">Dealers <span class="count">Retail & networks</span></h2>
    <div class="article-table">
      
      <div class="article-row">
        <div class="score-chip">64</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/new-models-vital-ds-survival-uk-sales-hit-record-low" target="_blank" rel="noopener">DS UK sales slide; dealer viability hinges on new models</a>
          <div class="article-take">Low throughput strains boutique networks when lineups age.</div>
          <div class="article-tags">
            <span class="chip">Dealers</span><span class="chip">DS</span><span class="chip">Sales</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 4, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/new-models-vital-ds-survival-uk-sales-hit-record-low" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      

      <div class="article-row">
        <div class="score-chip">71</div>
        <div class="article-main">
          <a class="headline" href="https://www.greencarreports.com/news/1146045_california-has-nearly-50-more-public-ev-chargers-than-gas-nozzles" target="_blank" rel="noopener">California’s public EV chargers outnumber gas nozzles</a>
          <div class="article-take">Retail sites with charging gain a new reason to drive traffic and dwell time.</div>
          <div class="article-tags">
            <span class="chip">Retail</span><span class="chip">Charging</span><span class="chip">California</span>
          </div>
        </div>
        <div class="article-source">
          <span>Green Car Reports — Aug 3, 2026</span>
          <a href="https://www.greencarreports.com/news/1146045_california-has-nearly-50-more-public-ev-chargers-than-gas-nozzles" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      

    </div>
  </div>

  <div class="sec-group reveal" id="suppliers">
    <h2 class="section-title">Suppliers <span class="count">Ecosystem moves</span></h2>
    <div class="article-table">
      
      <div class="article-row">
        <div class="score-chip high">89</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Volvo dumps lidar supplier, compensates owners</a>
          <div class="article-take">A flagship pivot tests lidar business models and supplier resilience.</div>
          <div class="article-tags">
            <span class="chip">Volvo</span><span class="chip">Lidar</span><span class="chip">Suppliers</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      
      <div class="article-row">
        <div class="score-chip">84</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">SK On, Factorial partner on solid‑state scale up</a>
          <div class="article-take">Cross‑border alliances are becoming the fastest route to commercialization.</div>
          <div class="article-tags">
            <span class="chip">Battery</span><span class="chip">SK On</span><span class="chip">Factorial</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      
      <div class="article-row">
        <div class="score-chip">68</div>
        <div class="article-main">
          <a class="headline" href="https://chargedevs.com/newswire/mahle-introduces-a-new-range-extender-engine-and-a-rare-earth-free-electric-motor/" target="_blank" rel="noopener">MAHLE unveils diesel range‑extender, rare‑earth‑free e‑motor</a>
          <div class="article-take">Suppliers target cost and resource constraints with novel architectures.</div>
          <div class="article-tags">
            <span class="chip">Suppliers</span><span class="chip">Powertrain</span><span class="chip">Trucking</span>
          </div>
        </div>
        <div class="article-source">
          <span>Charged EVs — Aug 3, 2026</span>
          <a href="https://chargedevs.com/newswire/mahle-introduces-a-new-range-extender-engine-and-a-rare-earth-free-electric-motor/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      
    </div>
  </div>

  <div class="sec-group reveal" id="government">
    <h2 class="section-title">Government <span class="count">Policy & regulation</span></h2>
    <div class="article-table">
      
      <div class="article-row">
        <div class="score-chip high">93</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">NHTSA opens probe into 1.2M Teslas</a>
          <div class="article-take">A potential recall could ripple through service networks and supply chains.</div>
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
        <div class="score-chip">78</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/philippines-launches-e850m-incentive-programme-for-ev-manufacturing/" target="_blank" rel="noopener">Philippines unveils €850m EV manufacturing incentives</a>
          <div class="article-take">Southeast Asia sharpens its pitch to capture electrified supply chains.</div>
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
        <div class="score-chip">74</div>
        <div class="article-main">
          <a class="headline" href="https://www.greencarreports.com/news/1146045_california-has-nearly-50-more-public-ev-chargers-than-gas-nozzles" target="_blank" rel="noopener">California: public EV chargers surpass gas nozzles</a>
          <div class="article-take">Infrastructure momentum strengthens regulators’ ZEV timelines.</div>
          <div class="article-tags">
            <span class="chip">Infrastructure</span><span class="chip">California</span><span class="chip">Policy</span>
          </div>
        </div>
        <div class="article-source">
          <span>Green Car Reports — Aug 3, 2026</span>
          <a href="https://www.greencarreports.com/news/1146045_california-has-nearly-50-more-public-ev-chargers-than-gas-nozzles" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      
    </div>
  </div>

  <div class="sec-group reveal" id="technology">
    <h2 class="section-title">Technology <span class="count">Software & systems</span></h2>
    <div class="article-table">
      
      <div class="article-row">
        <div class="score-chip">79</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/waymo-gemini-ai-ojai-robotaxi-redesigned-interface/" target="_blank" rel="noopener">Waymo integrates Gemini AI into robotaxi experience</a>
          <div class="article-take">Voice co‑pilots are coming to the ride UX as AVs court mainstream users.</div>
          <div class="article-tags">
            <span class="chip">Autonomous</span><span class="chip">AI</span><span class="chip">UX</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/waymo-gemini-ai-ojai-robotaxi-redesigned-interface/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      
      <div class="article-row">
        <div class="score-chip">72</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/03/blue-solutions-and-avl-test-solid-state-battery-safety/" target="_blank" rel="noopener">Solid‑state battery safety work advances</a>
          <div class="article-take">OEMs will demand validated containment before volume deployment.</div>
          <div class="article-tags">
            <span class="chip">Battery</span><span class="chip">Solid‑state</span><span class="chip">Safety</span>
          </div>
        </div>
        <div class="article-source">
          <span>electrive — Aug 3, 2026</span>
          <a href="https://www.electrive.com/2026/08/03/blue-solutions-and-avl-test-solid-state-battery-safety/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      
      <div class="article-row">
        <div class="score-chip">69</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/04/tesla-fsd-v14-lite-hw3-computer-failures/" target="_blank" rel="noopener">Reports: Tesla HW3 overheating after FSD v14 Lite</a>
          <div class="article-take">Legacy compute constraints may force feature throttling or hardware swaps.</div>
          <div class="article-tags">
            <span class="chip">Tesla</span><span class="chip">Software</span><span class="chip">Compute</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 4, 2026</span>
          <a href="https://electrek.co/2026/08/03/tesla-fsd-v14-lite-hw3-computer-failures/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      
    </div>
  </div>

  <div class="sec-group reveal" id="finance">
    <h2 class="section-title">Finance <span class="count">Capital & earnings</span></h2>
    <div class="article-table">
      
      <div class="article-row">
        <div class="score-chip">65</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/30/rivian-rivn-q2-2026-earnings-r2-deliveries-revenue-up-27/" target="_blank" rel="noopener">Rivian Q2: revenue up; gross profit record</a>
          <div class="article-take">Scaling a cheaper model is moving the P&L in the right direction.</div>
          <div class="article-tags">
            <span class="chip">Rivian</span><span class="chip">Earnings</span><span class="chip">Margins</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 30, 2026</span>
          <a href="https://electrek.co/2026/07/30/rivian-rivn-q2-2026-earnings-r2-deliveries-revenue-up-27/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      
      <div class="article-row">
        <div class="score-chip">73</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/01/allego-commits-e100-million-to-expand-uk-charging-network/" target="_blank" rel="noopener">Allego invests €100m in UK fast charging</a>
          <div class="article-take">Funding targets high‑traffic corridors to capture utilization growth.</div>
          <div class="article-tags">
            <span class="chip">Investment</span><span class="chip">Charging</span><span class="chip">UK</span>
          </div>
        </div>
        <div class="article-source">
          <span>electrive — Aug 1, 2026</span>
          <a href="https://www.electrive.com/2026/08/01/allego-commits-e100-million-to-expand-uk-charging-network/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      
      <div class="article-row">
        <div class="score-chip">70</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/03/base-power-raises-1b-to-roll-out-its-giant-new-home-battery/" target="_blank" rel="noopener">Base Power raises $1B for oversized home battery rollout</a>
          <div class="article-take">Residential storage scales to backstop grids stressed by data centers and EVs.</div>
          <div class="article-tags">
            <span class="chip">Energy storage</span><span class="chip">Finance</span><span class="chip">Grid</span>
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
    <h2 class="section-title">International <span class="count">Global markets</span></h2>
    <div class="article-table">
      
      <div class="article-row">
        <div class="score-chip">66</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/04/tesla-china-sales-crash-exports-surge-h1-2026/" target="_blank" rel="noopener">Tesla’s China sales drop while exports surge</a>
          <div class="article-take">Shanghai pivots to export as local brands tighten the squeeze.</div>
          <div class="article-tags">
            <span class="chip">China</span><span class="chip">Exports</span><span class="chip">Tesla</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 4, 2026</span>
          <a href="https://electrek.co/2026/08/04/tesla-china-sales-crash-exports-surge-h1-2026/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      
      <div class="article-row">
        <div class="score-chip">75</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/denmark-evs-account-for-almost-all-new-car-registrations-in-july/" target="_blank" rel="noopener">Denmark’s EV share hits 97.6% for private buyers</a>
          <div class="article-take">A live case study in rapid electrification at national scale.</div>
          <div class="article-tags">
            <span class="chip">Denmark</span><span class="chip">EV adoption</span><span class="chip">Europe</span>
          </div>
        </div>
        <div class="article-source">
          <span>electrive — Aug 4, 2026</span>
          <a href="https://www.electrive.com/2026/08/04/denmark-evs-account-for-almost-all-new-car-registrations-in-july/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      
      <div class="article-row">
        <div class="score-chip">78</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/philippines-launches-e850m-incentive-programme-for-ev-manufacturing/" target="_blank" rel="noopener">Philippines launches major EV manufacturing incentives</a>
          <div class="article-take">New capital destinations emerge as global supply chains diversify.</div>
          <div class="article-tags">
            <span class="chip">ASEAN</span><span class="chip">Manufacturing</span><span class="chip">Policy</span>
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
    <h2 class="section-title">Opinion <span class="count">Analysis & commentary</span></h2>
    <div class="article-table">
      
      <div class="article-row">
        <div class="score-chip">71</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/04/waymo-co-ceo-camera-only-self-driving-tesla/" target="_blank" rel="noopener">Waymo co‑CEO on why camera‑only AV stacks fall short</a>
          <div class="article-take">A direct challenge to single‑sensor philosophy underscores diverging AV strategies.</div>
          <div class="article-tags">
            <span class="chip">Autonomous</span><span class="chip">Sensors</span><span class="chip">Opinion</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 4, 2026</span>
          <a href="https://electrek.co/2026/08/04/waymo-co-ceo-camera-only-self-driving-tesla/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      
      <div class="article-row">
        <div class="score-chip">62</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/opinion/new-cars/ignore-jay-leno-your-dream-garage-only-needs-three-cars" target="_blank" rel="noopener">Forget mega‑collections—your dream garage may only need three cars</a>
          <div class="article-take">A case for curation over accumulation in enthusiast ownership.</div>
          <div class="article-tags">
            <span class="chip">Opinion</span><span class="chip">Enthusiast</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 1, 2026</span>
          <a href="https://www.autocar.co.uk/opinion/new-cars/ignore-jay-leno-your-dream-garage-only-needs-three-cars" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      
      <div class="article-row">
        <div class="score-chip">60</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/business-manufacturing/chinese-car-makers-all-share-parts-will-world-follow" target="_blank" rel="noopener">China’s parts‑sharing playbook: will the world follow?</a>
          <div class="article-take">Industrial standardization is compressing cost and time‑to‑market across rivals.</div>
          <div class="article-tags">
            <span class="chip">China</span><span class="chip">Manufacturing</span><span class="chip">Opinion</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 3, 2026</span>
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