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
        <h1>NHTSA opens safety probe into 1.2M Tesla Model 3/Y over front suspension failures</h1>
        <p class="exec-summary">US regulators launched a sweeping investigation after reports that a key front suspension link can detach on certain Tesla Model 3 and Y vehicles. The case puts fresh scrutiny on Tesla’s quality controls and could trigger recalls or design changes across its highest-volume models.</p>

        <div class="takeaways">
          <h3>Key Takeaways</h3>
          <ul>
            <li>Preliminary evaluation targets 2018–2020 Model 3 and 2021–2023 Model Y for front lower lateral link separation.</li>
            <li>156 complaints triggered the probe; outcomes can range from data requests to a mandatory recall.</li>
            <li>Risk profile spans millions of in-service vehicles, directly affecting residual values and service loads.</li>
            <li>Adds to Tesla’s 2026 regulatory stack as it contends with software, Autopilot and supplier disputes.</li>
          </ul>
        </div>

        <div class="impact-row">
          <div class="impact-block">
            <h4>Industry Impact</h4>
            <p>Large-scale suspension scrutiny on the top-selling EVs in the US can ripple through warranty reserves, supplier relationships and repair capacity. It also sharpens regulator focus on EV durability as the market matures, setting precedent for how quickly hardware issues must be addressed at fleet scale.</p>
          </div>
          <div class="impact-block">
            <h4>Companies Affected</h4>
            <div class="chip-row">
              <span class="chip entity-mfr">Tesla</span>
              <span class="chip">NHTSA / ODI</span>
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
            <li><a href="https://electrek.co/2026/08/03/tesla-fsd-v14-lite-hw3-computer-failures/" target="_blank" rel="noopener">Owners report Autopilot computer overheating after FSD v14 “Lite” rollout</a></li>
            <li><a href="https://electrek.co/2026/07/28/tesla-sues-cybertruck-supplier-angstrom-tooling/" target="_blank" rel="noopener">Tesla sues Cybertruck supplier in tooling standoff that risks output</a></li>
            <li><a href="https://electrek.co/2026/08/04/tesla-china-sales-crash-exports-surge-h1-2026/" target="_blank" rel="noopener">Tesla China sales slide as Shanghai pivots to exports</a></li>
            <li><a href="https://electrek.co/2026/07/30/tesla-10-millionth-vehicle-ev-growth-stalled/" target="_blank" rel="noopener">Tesla builds 10 millionth vehicle as growth cools vs. capacity</a></li>
          </ul>
        </div>
      </div>

      <div class="hero-gauges">
        <div class="gauge">
          <svg viewBox="0 0 120 70"><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#2a3038" stroke-width="8"/><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#f2a93b" stroke-width="8" stroke-dasharray="157" stroke-dashoffset="7.9"/></svg>
          <span class="gauge-value mono">95</span>
          <span class="gauge-label">Importance</span>
        </div>
        <div class="gauge">
          <svg viewBox="0 0 120 70"><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#2a3038" stroke-width="8"/><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#3ecf8e" stroke-width="8" stroke-dasharray="157" stroke-dashoffset="12.6"/></svg>
          <span class="gauge-value mono">92</span>
          <span class="gauge-label">Editorial Quality</span>
        </div>
        <div class="gauge">
          <svg viewBox="0 0 120 70"><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#2a3038" stroke-width="8"/><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#e2604f" stroke-width="8" stroke-dasharray="157" stroke-dashoffset="15.7"/></svg>
          <span class="gauge-value mono">90</span>
          <span class="gauge-label">Industry Impact</span>
        </div>
        <div class="gauge">
          <svg viewBox="0 0 120 70"><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#2a3038" stroke-width="8"/><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#f2a93b" stroke-width="8" stroke-dasharray="157" stroke-dashoffset="18.8"/></svg>
          <span class="gauge-value mono">88</span>
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
          <li><span>Tesla</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:100%"></span></span><span class="rank-count">9</span></li>
          <li><span>BMW</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:78%"></span></span><span class="rank-count">7</span></li>
          <li><span>Mercedes-Benz</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:67%"></span></span><span class="rank-count">6</span></li>
          <li><span>Hyundai / Kia</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:67%"></span></span><span class="rank-count">6</span></li>
          <li><span>BYD</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:56%"></span></span><span class="rank-count">5</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4>Top Brands</h4>
        <ul class="rank-list">
          <li><span>Audi</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:100%"></span></span><span class="rank-count">6</span></li>
          <li><span>Volvo</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:67%"></span></span><span class="rank-count">4</span></li>
          <li><span>Genesis</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:50%"></span></span><span class="rank-count">3</span></li>
          <li><span>Rivian</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:50%"></span></span><span class="rank-count">3</span></li>
          <li><span>Ferrari</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:33%"></span></span><span class="rank-count">2</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4>Top Suppliers / Networks</h4>
        <ul class="rank-list">
          <li><span>EVgo</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:100%"></span></span><span class="rank-count">3</span></li>
          <li><span>Allego</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:100%"></span></span><span class="rank-count">3</span></li>
          <li><span>SK On</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:67%"></span></span><span class="rank-count">2</span></li>
          <li><span>Factorial Energy</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:67%"></span></span><span class="rank-count">2</span></li>
          <li><span>Beam Global</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:67%"></span></span><span class="rank-count">2</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4>Most Mentioned Executives</h4>
        <ul class="rank-list">
          <li><span>Elon Musk (Tesla)</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:100%"></span></span><span class="rank-count">5</span></li>
          <li><span>Ola Källenius (Mercedes)</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:80%"></span></span><span class="rank-count">4</span></li>
          <li><span>RJ Scaringe (Rivian)</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:60%"></span></span><span class="rank-count">3</span></li>
          <li><span>Dmitri Dolgov (Waymo)</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:40%"></span></span><span class="rank-count">2</span></li>
          <li><span>Michael Leiters (Porsche)</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:40%"></span></span><span class="rank-count">2</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4>Trending Topics</h4>
        <div class="tagcloud">
          <span class="chip lg">Safety probes</span>
          <span class="chip lg">Affordable EVs</span>
          <span class="chip">Fast charging buildout</span>
          <span class="chip">Solid-state batteries</span>
          <span class="chip">Hands-free driving</span>
          <span class="chip">Lidar strategy</span>
          <span class="chip">EV market shares (Nordics)</span>
          <span class="chip">Supplier disputes</span>
        </div>
      </div>

      <div class="stat-panel">
        <h4>Emerging Technologies</h4>
        <div class="tagcloud">
          <span class="chip lg">Solid-state cells</span>
          <span class="chip">LFP packs to 100% SOC</span>
          <span class="chip">800V architectures</span>
          <span class="chip">Level 2 hands-free</span>
          <span class="chip">Robotaxi UX (AI)</span>
        </div>
      </div>

      <div class="stat-panel">
        <h4>Government & Safety</h4>
        <ul class="rank-list">
          <li><span>NHTSA Tesla suspension probe</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:100%"></span></span><span class="rank-count">1</span></li>
          <li><span>Ram 1500 seat-belt recall</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:75%"></span></span><span class="rank-count">1</span></li>
          <li><span>Philippines EV incentives</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:75%"></span></span><span class="rank-count">1</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4>Financial & Market Activity</h4>
        <ul class="rank-list">
          <li><span>Rivian beats on Q2</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:100%"></span></span><span class="rank-count">1</span></li>
          <li><span>Base Power raises $1B</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:90%"></span></span><span class="rank-count">1</span></li>
          <li><span>BYD July sales +22%</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:90%"></span></span><span class="rank-count">1</span></li>
          <li><span>BMW product review shift</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:80%"></span></span><span class="rank-count">1</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4>Global Regions</h4>
        <ul class="rank-list">
          <li><span>United States</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:100%"></span></span><span class="rank-count">10</span></li>
          <li><span>China</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:80%"></span></span><span class="rank-count">8</span></li>
          <li><span>United Kingdom</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:60%"></span></span><span class="rank-count">6</span></li>
          <li><span>Nordics (NO/DK)</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:60%"></span></span><span class="rank-count">6</span></li>
          <li><span>EU (general)</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:50%"></span></span><span class="rank-count">5</span></li>
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
        <a href="https://www.autocar.co.uk/car-news/electric-cars/new-mercedes-gla-revealed-audi-q4-rival-408-mile-range" target="_blank" rel="noopener">Mercedes unveils new GLA EV with up to 408-mile range</a>
        <div class="fp-meta"><span>Score 88</span><span>•</span><span>Aug 4</span></div>
        <div class="fp-meta">Compact MMA-based SUV resets Mercedes’ small EV play with 800V charging.</div>
      </div>
      <div class="fp-row">
        <a href="https://www.autocar.co.uk/car-news/new-cars/audi-q9-suv-revealed-huge-%C2%A3100k-a8-successor" target="_blank" rel="noopener">Audi reveals Q9 flagship SUV</a>
        <div class="fp-meta"><span>Score 84</span><span>•</span><span>Aug 4</span></div>
        <div class="fp-meta">Seven-seat, tech-heavy halo targets US and Middle East luxury demand.</div>
      </div>
      <div class="fp-row">
        <a href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">BMW puts hardcore off-roader on hold amid China headwinds</a>
        <div class="fp-meta"><span>Score 82</span><span>•</span><span>Aug 4</span></div>
        <div class="fp-meta">Shift underscores fast-moving model strategy and market divergence.</div>
      </div>
      <div class="fp-row">
        <a href="https://www.autocar.co.uk/car-news/new-cars/byd-goes-after-defender-boxy-%C2%A348k-402bhp-hybrid-suv" target="_blank" rel="noopener">BYD brings boxy Ti7 hybrid SUV to the UK at £47,995</a>
        <div class="fp-meta"><span>Score 78</span><span>•</span><span>Aug 4</span></div>
        <div class="fp-meta">Rugged styling plus long EV-only range challenge legacy 4x4s on price.</div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Technology</h3>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">SK On and Factorial team up on solid-state scaling</a>
        <div class="fp-meta"><span>Score 86</span><span>•</span><span>Aug 4</span></div>
        <div class="fp-meta">Alliance accelerates commercialization path for high-density cells.</div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Volvo drops lidar from EX90/ES90 and compensates buyers</a>
        <div class="fp-meta"><span>Score 85</span><span>•</span><span>Aug 4</span></div>
        <div class="fp-meta">A major ADAS strategy pivot with direct owner impact and supplier fallout.</div>
      </div>
      <div class="fp-row">
        <a href="https://www.carscoops.com/2026/08/audi-hands-free-driving-system/" target="_blank" rel="noopener">Audi launches Level 2 hands-free on new Q9</a>
        <div class="fp-meta"><span>Score 80</span><span>•</span><span>Aug 4</span></div>
        <div class="fp-meta">Highway automation up to 85 mph rolls out in US and abroad.</div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/08/03/tesla-fsd-v14-lite-hw3-computer-failures/" target="_blank" rel="noopener">Owners report HW3 overheating after FSD v14 “Lite”</a>
        <div class="fp-meta"><span>Score 77</span><span>•</span><span>Aug 4</span></div>
        <div class="fp-meta">Thermal margins on legacy compute face stress under new software load.</div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Government & Safety</h3>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">NHTSA probes 1.2M Tesla vehicles for suspension issues</a>
        <div class="fp-meta"><span>Score 95</span><span>•</span><span>Aug 4</span></div>
        <div class="fp-meta">Potential recall exposure on the US market’s leading EVs.</div>
      </div>
      <div class="fp-row">
        <a href="https://www.caranddriver.com/news/a73319471/ram-1500-seatbelt-buckle-one-million-truck-recall/" target="_blank" rel="noopener">Ram to recall ~1.2M 1500 pickups for seat-belt anchors</a>
        <div class="fp-meta"><span>Score 83</span><span>•</span><span>Aug 4</span></div>
        <div class="fp-meta">Second-row restraints trigger a large-scale safety campaign.</div>
      </div>
      <div class="fp-row">
        <a href="https://www.electrive.com/2026/08/04/philippines-launches-e850m-incentive-programme-for-ev-manufacturing/" target="_blank" rel="noopener">Philippines launches €850m EV manufacturing incentives</a>
        <div class="fp-meta"><span>Score 72</span><span>•</span><span>Aug 4</span></div>
        <div class="fp-meta">New SEA production hub emerges for EVs and components.</div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Suppliers & Infrastructure</h3>
      <div class="fp-row">
        <a href="https://www.electrive.com/2026/08/04/evgo-and-brixmor-to-add-more-than-500-fast-charging-stalls-in-the-us/" target="_blank" rel="noopener">EVgo, Brixmor to add 500+ DC fast stalls at US retail centers</a>
        <div class="fp-meta"><span>Score 79</span><span>•</span><span>Aug 4</span></div>
        <div class="fp-meta">Convenience charging push ties into mainstream shopping trips.</div>
      </div>
      <div class="fp-row">
        <a href="https://www.electrive.com/2026/08/01/allego-commits-e100-million-to-expand-uk-charging-network/" target="_blank" rel="noopener">Allego commits €100m to expand UK ultra-rapid network</a>
        <div class="fp-meta"><span>Score 78</span><span>•</span><span>Aug 4</span></div>
        <div class="fp-meta">1,400 chargers targeted by 2030, prioritizing London and high-traffic sites.</div>
      </div>
      <div class="fp-row">
        <a href="https://www.electrive.com/2026/08/03/devon-and-torbay-commission-nearly-3000-public-ev-charging-points/" target="_blank" rel="noopener">Devon & Torbay commission ~3,000 kerbside points</a>
        <div class="fp-meta"><span>Score 73</span><span>•</span><span>Aug 4</span></div>
        <div class="fp-meta">Public-private rollout accelerates UK on-street access.</div>
      </div>
      <div class="fp-row">
        <a href="https://chargedevs.com/newswire/beam-global-supplies-ev-arc-off-grid-charging-systems-for-dallas-municipal-fleet-and-massachusetts-carshare-pilot/" target="_blank" rel="noopener">Beam Global wins off-grid charging orders in TX and MA</a>
        <div class="fp-meta"><span>Score 68</span><span>•</span><span>Aug 4</span></div>
        <div class="fp-meta">Rapid-deploy solar + storage helps fleets and shared mobility pilots.</div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Trending Topics</h3>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/hyundai-reveals-ioniq-3-prices-start-30000-interest-surges/" target="_blank" rel="noopener">Affordable EV momentum: Hyundai IONIQ 3 from ~$30k</a>
        <div class="fp-meta"><span>Score 82</span><span>•</span><span>Aug 4</span></div>
        <div class="fp-meta">High interest signals price-sensitive demand returning to market.</div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/27/rivian-r2-tesla-model-y-real-world-efficiency-test/" target="_blank" rel="noopener">Efficiency gap: R2 uses up to 26% more energy than Model Y</a>
        <div class="fp-meta"><span>Score 76</span><span>•</span><span>Aug 4</span></div>
        <div class="fp-meta">Real-world tests highlight aero/drive-unit tradeoffs in mid-size EVs.</div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/08/04/waymo-co-ceo-camera-only-self-driving-tesla/" target="_blank" rel="noopener">AD perception debate heats up: Waymo critiques camera-only</a>
        <div class="fp-meta"><span>Score 74</span><span>•</span><span>Aug 4</span></div>
        <div class="fp-meta">Sensor fusion vs. vision-only becomes a public technical showdown.</div>
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
    <h2 class="section-title">Latest Articles <span class="count">20 analyzed today</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip high">95</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">NHTSA probes 1.2M Tesla Model 3/Y over front suspension failures</a>
          <div class="article-take">A large-scale safety inquiry could force design or service actions on Tesla’s core models.</div>
          <div class="article-tags">
            <span class="chip">Government</span><span class="chip">Safety</span><span class="chip">Recall</span>
            <span class="chip">Tesla</span><span class="chip">NHTSA</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 4, 2026</span>
          <a href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip high">90</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Volvo drops lidar on EX90/ES90; pays owners compensation</a>
          <div class="article-take">Axing lidar resets Volvo’s ADAS roadmap and reverberates through its supplier stack.</div>
          <div class="article-tags">
            <span class="chip">ADAS</span><span class="chip">Technology</span><span class="chip">Volvo</span><span class="chip">Lidar</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 4, 2026</span>
          <a href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">84</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/audi-q9-suv-revealed-huge-%C2%A3100k-a8-successor" target="_blank" rel="noopener">Audi Q9 revealed as tech-forward flagship SUV</a>
          <div class="article-take">A new halo SUV pushes Audi’s in-car experience and luxury positioning upward.</div>
          <div class="article-tags">
            <span class="chip">Manufacturers</span><span class="chip">Audi</span><span class="chip">Luxury</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 4, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/audi-q9-suv-revealed-huge-%C2%A3100k-a8-successor" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">88</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/electric-cars/new-mercedes-gla-revealed-audi-q4-rival-408-mile-range" target="_blank" rel="noopener">New Mercedes GLA EV launches with up to 408-mile range</a>
          <div class="article-take">Mercedes refreshes its entry SUV with long-range specs and 800V fast charging.</div>
          <div class="article-tags">
            <span class="chip">EV</span><span class="chip">Manufacturers</span><span class="chip">Mercedes-Benz</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 4, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/electric-cars/new-mercedes-gla-revealed-audi-q4-rival-408-mile-range" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">82</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/hyundai-reveals-ioniq-3-prices-start-30000-interest-surges/" target="_blank" rel="noopener">Hyundai’s IONIQ 3 starts around $30,000 with 300+ miles range</a>
          <div class="article-take">A mainstream-priced EV with long range rekindles consumer interest at scale.</div>
          <div class="article-tags">
            <span class="chip">EV</span><span class="chip">Pricing</span><span class="chip">Hyundai</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 4, 2026</span>
          <a href="https://electrek.co/2026/07/29/hyundai-reveals-ioniq-3-prices-start-30000-interest-surges/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">86</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">SK On, Factorial form alliance to scale solid-state batteries</a>
          <div class="article-take">Partnership consolidates IP and manufacturing know-how to de-risk commercialization.</div>
          <div class="article-tags">
            <span class="chip">Battery</span><span class="chip">Solid-state</span><span class="chip">Suppliers</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 4, 2026</span>
          <a href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip high">89</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/30/rivian-rivn-q2-2026-earnings-r2-deliveries-revenue-up-27/" target="_blank" rel="noopener">Rivian Q2: revenue up 27%, record gross profit, R2 deliveries begin</a>
          <div class="article-take">Execution improves as Rivian pivots toward its mass-market crossover.</div>
          <div class="article-tags">
            <span class="chip">Finance</span><span class="chip">EV</span><span class="chip">Rivian</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 4, 2026</span>
          <a href="https://electrek.co/2026/07/30/rivian-rivn-q2-2026-earnings-r2-deliveries-revenue-up-27/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">76</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/27/rivian-r2-tesla-model-y-real-world-efficiency-test/" target="_blank" rel="noopener">Test: Rivian R2 uses 18–26% more energy than Tesla Model Y</a>
          <div class="article-take">Real-world efficiency gap could influence total cost of ownership and road-trip planning.</div>
          <div class="article-tags">
            <span class="chip">EV</span><span class="chip">Efficiency</span><span class="chip">Rivian</span><span class="chip">Tesla</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 4, 2026</span>
          <a href="https://electrek.co/2026/07/27/rivian-r2-tesla-model-y-real-world-efficiency-test/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">82</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">BMW reassesses product plan; off-roader on hold amid China pressure</a>
          <div class="article-take">Global demand divergence forces tighter portfolio choices and pacing.</div>
          <div class="article-tags">
            <span class="chip">Manufacturing</span><span class="chip">Strategy</span><span class="chip">BMW</span>
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
          <a class="headline" href="https://electrek.co/2026/07/28/bmw-ramps-up-ix3-output-orders-near-100000/" target="_blank" rel="noopener">BMW ramps iX3 output as orders near 100,000</a>
          <div class="article-take">Accelerated plant ramp shows early pull for Neue Klasse-based crossover.</div>
          <div class="article-tags">
            <span class="chip">Production</span><span class="chip">EV</span><span class="chip">BMW</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 4, 2026</span>
          <a href="https://electrek.co/2026/07/28/bmw-ramps-up-ix3-output-orders-near-100000/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">78</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/28/tesla-sues-cybertruck-supplier-angstrom-tooling/" target="_blank" rel="noopener">Tesla sues Cybertruck supplier in tooling access dispute</a>
          <div class="article-take">A legal scramble over dies threatens near-term throughput on a constrained program.</div>
          <div class="article-tags">
            <span class="chip">Supply Chain</span><span class="chip">Tesla</span><span class="chip">Manufacturing</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 4, 2026</span>
          <a href="https://electrek.co/2026/07/28/tesla-sues-cybertruck-supplier-angstrom-tooling/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">79</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/evgo-and-brixmor-to-add-more-than-500-fast-charging-stalls-in-the-us/" target="_blank" rel="noopener">EVgo, Brixmor to add 500+ fast chargers across US shopping centers</a>
          <div class="article-take">Retail-anchored charging expands access where dwell times already exist.</div>
          <div class="article-tags">
            <span class="chip">Charging</span><span class="chip">Infrastructure</span><span class="chip">EVgo</span>
          </div>
        </div>
        <div class="article-source">
          <span>electrive — Aug 4, 2026</span>
          <a href="https://www.electrive.com/2026/08/04/evgo-and-brixmor-to-add-more-than-500-fast-charging-stalls-in-the-us/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">78</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/01/allego-commits-e100-million-to-expand-uk-charging-network/" target="_blank" rel="noopener">Allego invests €100m to expand UK ultra-rapid charging</a>
          <div class="article-take">Operator targets 1,400 stalls by 2030 with focus on high-traffic corridors.</div>
          <div class="article-tags">
            <span class="chip">Charging</span><span class="chip">UK</span><span class="chip">Allego</span>
          </div>
        </div>
        <div class="article-source">
          <span>electrive — Aug 4, 2026</span>
          <a href="https://www.electrive.com/2026/08/01/allego-commits-e100-million-to-expand-uk-charging-network/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">73</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/03/devon-and-torbay-commission-nearly-3000-public-ev-charging-points/" target="_blank" rel="noopener">Devon & Torbay to deploy nearly 3,000 public EV chargers</a>
          <div class="article-take">Local authorities lean on multiple partners to speed kerbside access.</div>
          <div class="article-tags">
            <span class="chip">Charging</span><span class="chip">Municipal</span><span class="chip">UK</span>
          </div>
        </div>
        <div class="article-source">
          <span>electrive — Aug 4, 2026</span>
          <a href="https://www.electrive.com/2026/08/03/devon-and-torbay-commission-nearly-3000-public-ev-charging-points/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">72</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/denmark-evs-account-for-almost-all-new-car-registrations-in-july/" target="_blank" rel="noopener">Denmark: EVs hit 97% of private registrations in July</a>
          <div class="article-take">Nordic adoption remains a bellwether for policy + product working in tandem.</div>
          <div class="article-tags">
            <span class="chip">International</span><span class="chip">EV Market</span><span class="chip">Denmark</span>
          </div>
        </div>
        <div class="article-source">
          <span>electrive — Aug 4, 2026</span>
          <a href="https://www.electrive.com/2026/08/04/denmark-evs-account-for-almost-all-new-car-registrations-in-july/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">70</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/03/norways-ev-share-rises-to-97-6-in-july/" target="_blank" rel="noopener">Norway’s EV share rises to 97.6% in July</a>
          <div class="article-take">Mature EV market sustains near-total share, anchoring European transition metrics.</div>
          <div class="article-tags">
            <span class="chip">International</span><span class="chip">EV Market</span><span class="chip">Norway</span>
          </div>
        </div>
        <div class="article-source">
          <span>electrive — Aug 4, 2026</span>
          <a href="https://www.electrive.com/2026/08/03/norways-ev-share-rises-to-97-6-in-july/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">78</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/byd-goes-after-defender-boxy-%C2%A348k-402bhp-hybrid-suv" target="_blank" rel="noopener">BYD launches Ti7 hybrid SUV in UK at £47,995</a>
          <div class="article-take">Value-forward, rugged design aims to siphon buyers from legacy 4x4s.</div>
          <div class="article-tags">
            <span class="chip">Manufacturers</span><span class="chip">BYD</span><span class="chip">Hybrid</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 4, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/byd-goes-after-defender-boxy-%C2%A348k-402bhp-hybrid-suv" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">75</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/03/hyundai-kias-record-us-sales-run/" target="_blank" rel="noopener">Hyundai and Kia extend record US sales streak</a>
          <div class="article-take">Hybrids and affordable EVs are powering steady share gains.</div>
          <div class="article-tags">
            <span class="chip">Sales</span><span class="chip">Hyundai</span><span class="chip">Kia</span><span class="chip">Hybrid</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 4, 2026</span>
          <a href="https://electrek.co/2026/08/03/hyundai-kias-record-us-sales-run/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">74</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/07/31/tesla-tops-10-million-electric-vehicles-built/" target="_blank" rel="noopener">Tesla crosses 10 million EVs built</a>
          <div class="article-take">A historic volume milestone arrives as growth lags installed capacity.</div>
          <div class="article-tags">
            <span class="chip">Production</span><span class="chip">Tesla</span><span class="chip">Milestone</span>
          </div>
        </div>
        <div class="article-source">
          <span>electrive — Aug 4, 2026</span>
          <a href="https://www.electrive.com/2026/07/31/tesla-tops-10-million-electric-vehicles-built/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">74</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/04/waymo-co-ceo-camera-only-self-driving-tesla/" target="_blank" rel="noopener">Waymo co-CEO details why camera-only autonomy falls short</a>
          <div class="article-take">The sensor stack debate intensifies as robotaxi operators scale up.</div>
          <div class="article-tags">
            <span class="chip">Autonomous</span><span class="chip">ADAS</span><span class="chip">Waymo</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 4, 2026</span>
          <a href="https://electrek.co/2026/08/04/waymo-co-ceo-camera-only-self-driving-tesla/" target="_blank" rel="noopener">Read original →</a>
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
    <h2 class="section-title">Industry News <span class="count">Today</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip high">95</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">NHTSA opens safety probe into 1.2M Tesla vehicles</a>
          <div class="article-take">A potential recall across Tesla’s volume leaders would reshape 2H service ops.</div>
          <div class="article-tags"><span class="chip">Safety</span><span class="chip">Government</span><span class="chip">Tesla</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 4, 2026</span>
          <a href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">84</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/audi-q9-suv-revealed-huge-%C2%A3100k-a8-successor" target="_blank" rel="noopener">Audi debuts Q9 as upmarket SUV flagship</a>
          <div class="article-take">Big footprint, bigger tech: Audi pushes further into luxury territory.</div>
          <div class="article-tags"><span class="chip">Manufacturers</span><span class="chip">Luxury</span><span class="chip">Audi</span></div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 4, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/audi-q9-suv-revealed-huge-%C2%A3100k-a8-successor" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">82</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">BMW pauses G-Class rival in strategy review</a>
          <div class="article-take">Slower China and tariff risk prompt sharper model focus.</div>
          <div class="article-tags"><span class="chip">Strategy</span><span class="chip">BMW</span><span class="chip">Manufacturers</span></div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 4, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="electric-vehicles">
    <h2 class="section-title">Electric Vehicles <span class="count">Today</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip">88</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/electric-cars/new-mercedes-gla-revealed-audi-q4-rival-408-mile-range" target="_blank" rel="noopener">Mercedes’ new GLA EV claims up to 408 miles</a>
          <div class="article-take">More space, faster charging and a long-range spec bolster the segment.</div>
          <div class="article-tags"><span class="chip">EV</span><span class="chip">Mercedes-Benz</span></div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 4, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/electric-cars/new-mercedes-gla-revealed-audi-q4-rival-408-mile-range" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">82</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/hyundai-reveals-ioniq-3-prices-start-30000-interest-surges/" target="_blank" rel="noopener">IONIQ 3 priced to move at ~$30k</a>
          <div class="article-take">Hyundai leans into value to reignite mass-market EV demand.</div>
          <div class="article-tags"><span class="chip">EV</span><span class="chip">Hyundai</span><span class="chip">Pricing</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 4, 2026</span>
          <a href="https://electrek.co/2026/07/29/hyundai-reveals-ioniq-3-prices-start-30000-interest-surges/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">86</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">Solid-state alliance: SK On x Factorial</a>
          <div class="article-take">Scaling plans move next-gen cells closer to vehicles.</div>
          <div class="article-tags"><span class="chip">Battery</span><span class="chip">Solid-state</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 4, 2026</span>
          <a href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="manufacturers">
    <h2 class="section-title">Manufacturers <span class="count">Today</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip">80</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/28/bmw-ramps-up-ix3-output-orders-near-100000/" target="_blank" rel="noopener">BMW accelerates iX3 production after strong orders</a>
          <div class="article-take">Capacity flex at Debrecen signals confidence in the new platform.</div>
          <div class="article-tags"><span class="chip">Production</span><span class="chip">BMW</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 4, 2026</span>
          <a href="https://electrek.co/2026/07/28/bmw-ramps-up-ix3-output-orders-near-100000/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">78</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/byd-goes-after-defender-boxy-%C2%A348k-402bhp-hybrid-suv" target="_blank" rel="noopener">BYD Ti7: UK launch undercuts rivals</a>
          <div class="article-take">Aggressive pricing highlights BYD’s fast-moving UK strategy.</div>
          <div class="article-tags"><span class="chip">BYD</span><span class="chip">Hybrid</span></div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 4, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/byd-goes-after-defender-boxy-%C2%A348k-402bhp-hybrid-suv" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">84</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/audi-q9-suv-revealed-huge-%C2%A3100k-a8-successor" target="_blank" rel="noopener">Audi raises stakes with Q9 flagship</a>
          <div class="article-take">Premium push brings new software and upscale cabin options.</div>
          <div class="article-tags"><span class="chip">Audi</span><span class="chip">Luxury</span></div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 4, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/audi-q9-suv-revealed-huge-%C2%A3100k-a8-successor" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="dealers">
    <h2 class="section-title">Dealers & Retail <span class="count">Today</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip">60</div>
        <div class="article-main">
          <a class="headline" href="https://www.motor1.com/news/803722/costco-infiniti-discount/" target="_blank" rel="noopener">Costco adds discounts on new Infiniti SUVs</a>
          <div class="article-take">Warehouse club channels keep moving metal via member-only pricing.</div>
          <div class="article-tags"><span class="chip">Retail</span><span class="chip">Dealers</span><span class="chip">Infiniti</span></div>
        </div>
        <div class="article-source">
          <span>Motor1 — Aug 4, 2026</span>
          <a href="https://www.motor1.com/news/803722/costco-infiniti-discount/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="suppliers">
    <h2 class="section-title">Suppliers <span class="count">Today</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip">86</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">SK On + Factorial align on solid-state scale-up</a>
          <div class="article-take">Joint roadmap aims to compress time-to-market for next-gen cells.</div>
          <div class="article-tags"><span class="chip">Battery</span><span class="chip">Suppliers</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 4, 2026</span>
          <a href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">78</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/01/allego-commits-e100-million-to-expand-uk-charging-network/" target="_blank" rel="noopener">Allego invests in UK ultra-rapid expansion</a>
          <div class="article-take">Supplier capital flows to strategic corridors and metro clusters.</div>
          <div class="article-tags"><span class="chip">Charging</span><span class="chip">Allego</span></div>
        </div>
        <div class="article-source">
          <span>electrive — Aug 4, 2026</span>
          <a href="https://www.electrive.com/2026/08/01/allego-commits-e100-million-to-expand-uk-charging-network/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">68</div>
        <div class="article-main">
          <a class="headline" href="https://chargedevs.com/newswire/beam-global-supplies-ev-arc-off-grid-charging-systems-for-dallas-municipal-fleet-and-massachusetts-carshare-pilot/" target="_blank" rel="noopener">Beam Global secures off-grid charging deployments</a>
          <div class="article-take">Solar + storage units fill gaps where grid upgrades lag.</div>
          <div class="article-tags"><span class="chip">Charging</span><span class="chip">Beam Global</span></div>
        </div>
        <div class="article-source">
          <span>Charged EVs — Aug 4, 2026</span>
          <a href="https://chargedevs.com/newswire/beam-global-supplies-ev-arc-off-grid-charging-systems-for-dallas-municipal-fleet-and-massachusetts-carshare-pilot/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="government">
    <h2 class="section-title">Government <span class="count">Today</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip high">95</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">NHTSA opens probe into Tesla suspension failures</a>
          <div class="article-take">Regulatory focus turns to mechanical durability at EV fleet scale.</div>
          <div class="article-tags"><span class="chip">Safety</span><span class="chip">Government</span><span class="chip">Tesla</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 4, 2026</span>
          <a href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">83</div>
        <div class="article-main">
          <a class="headline" href="https://www.caranddriver.com/news/a73319471/ram-1500-seatbelt-buckle-one-million-truck-recall/" target="_blank" rel="noopener">Ram recalls ~1.2M 1500 pickups for seat-belt anchors</a>
          <div class="article-take">Another large recall underscores tightening safety oversight.</div>
          <div class="article-tags"><span class="chip">Recall</span><span class="chip">Safety</span><span class="chip">Ram</span></div>
        </div>
        <div class="article-source">
          <span>Car and Driver — Aug 4, 2026</span>
          <a href="https://www.caranddriver.com/news/a73319471/ram-1500-seatbelt-buckle-one-million-truck-recall/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">72</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/philippines-launches-e850m-incentive-programme-for-ev-manufacturing/" target="_blank" rel="noopener">Philippines unveils €850m EV manufacturing incentives</a>
          <div class="article-take">Policy aims to attract new plants and supply chains to the region.</div>
          <div class="article-tags"><span class="chip">Policy</span><span class="chip">Manufacturing</span><span class="chip">Philippines</span></div>
        </div>
        <div class="article-source">
          <span>electrive — Aug 4, 2026</span>
          <a href="https://www.electrive.com/2026/08/04/philippines-launches-e850m-incentive-programme-for-ev-manufacturing/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="technology">
    <h2 class="section-title">Technology <span class="count">Today</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip">85</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Volvo ends lidar plan and compensates buyers</a>
          <div class="article-take">Shifting sensor strategy resets content and cost on flagship EVs.</div>
          <div class="article-tags"><span class="chip">ADAS</span><span class="chip">Volvo</span><span class="chip">Technology</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 4, 2026</span>
          <a href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">80</div>
        <div class="article-main">
          <a class="headline" href="https://www.carscoops.com/2026/08/audi-hands-free-driving-system/" target="_blank" rel="noopener">Audi introduces hands-free Level 2 system on Q9</a>
          <div class="article-take">High-speed lane-centering creeps toward broader autonomy—carefully.</div>
          <div class="article-tags"><span class="chip">ADAS</span><span class="chip">Audi</span></div>
        </div>
        <div class="article-source">
          <span>Carscoops — Aug 4, 2026</span>
          <a href="https://www.carscoops.com/2026/08/audi-hands-free-driving-system/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">77</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/03/tesla-fsd-v14-lite-hw3-computer-failures/" target="_blank" rel="noopener">Reports: HW3 compute overheating after FSD update</a>
          <div class="article-take">Software load meets older hardware—raising reliability questions.</div>
          <div class="article-tags"><span class="chip">Software</span><span class="chip">Tesla</span><span class="chip">Autonomy</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 4, 2026</span>
          <a href="https://electrek.co/2026/08/03/tesla-fsd-v14-lite-hw3-computer-failures/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="finance">
    <h2 class="section-title">Finance <span class="count">Today</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip high">89</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/30/rivian-rivn-q2-2026-earnings-r2-deliveries-revenue-up-27/" target="_blank" rel="noopener">Rivian beats on revenue, margins improve</a>
          <div class="article-take">A turning point as sub-$50k vehicles reach customers.</div>
          <div class="article-tags"><span class="chip">Earnings</span><span class="chip">Rivian</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 4, 2026</span>
          <a href="https://electrek.co/2026/07/30/rivian-rivn-q2-2026-earnings-r2-deliveries-revenue-up-27/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">81</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/03/base-power-raises-1b-to-roll-out-its-giant-new-home-battery/" target="_blank" rel="noopener">Base Power raises $1B for 39.2-kWh home battery rollout</a>
          <div class="article-take">Big storage for homes supports EV load and grid flexibility.</div>
          <div class="article-tags"><span class="chip">Energy</span><span class="chip">Finance</span><span class="chip">Storage</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 4, 2026</span>
          <a href="https://electrek.co/2026/08/03/base-power-raises-1b-to-roll-out-its-giant-new-home-battery/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">78</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/03/byd-boosts-sales-by-22-in-july/" target="_blank" rel="noopener">BYD July sales climb 22%, exports hit record share</a>
          <div class="article-take">Overseas growth offsets domestic softness for China’s EV giant.</div>
          <div class="article-tags"><span class="chip">Sales</span><span class="chip">BYD</span><span class="chip">Exports</span></div>
        </div>
        <div class="article-source">
          <span>electrive — Aug 4, 2026</span>
          <a href="https://www.electrive.com/2026/08/03/byd-boosts-sales-by-22-in-july/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

    </div>
  </div>

  <div class="sec-group reveal" id="international">
    <h2 class="section-title">International <span class="count">Today</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip">72</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/denmark-evs-account-for-almost-all-new-car-registrations-in-july/" target="_blank" rel="noopener">Denmark nears all-EV new car market</a>
          <div class="article-take">Policy + product mix continues to compress ICE share in Nordics.</div>
          <div class="article-tags"><span class="chip">EV Market</span><span class="chip">Denmark</span></div>
        </div>
        <div class="article-source">
          <span>electrive — Aug 4, 2026</span>
          <a href="https://www.electrive.com/2026/08/04/denmark-evs-account-for-almost-all-new-car-registrations-in-july/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">70</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/03/norways-ev-share-rises-to-97-6-in-july/" target="_blank" rel="noopener">Norway’s EV share climbs to 97.6%</a>
          <div class="article-take">The bellwether market shows sustained consumer acceptance at scale.</div>
          <div class="article-tags"><span class="chip">EV Market</span><span class="chip">Norway</span></div>
        </div>
        <div class="article-source">
          <span>electrive — Aug 4, 2026</span>
          <a href="https://www.electrive.com/2026/08/03/norways-ev-share-rises-to-97-6-in-july/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">72</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/philippines-launches-e850m-incentive-programme-for-ev-manufacturing/" target="_blank" rel="noopener">Philippines courts EV manufacturing with incentives</a>
          <div class="article-take">SEA manufacturing base competition intensifies.</div>
          <div class="article-tags"><span class="chip">Manufacturing</span><span class="chip">Policy</span><span class="chip">Philippines</span></div>
        </div>
        <div class="article-source">
          <span>electrive — Aug 4, 2026</span>
          <a href="https://www.electrive.com/2026/08/04/philippines-launches-e850m-incentive-programme-for-ev-manufacturing/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="opinion">
    <h2 class="section-title">Opinion & Analysis <span class="count">Today</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip">60</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/opinion/new-cars/ignore-jay-leno-your-dream-garage-only-needs-three-cars" target="_blank" rel="noopener">Ignore Jay Leno: your dream garage only needs three cars</a>
          <div class="article-take">A case for purposeful ownership over sprawling collections.</div>
          <div class="article-tags"><span class="chip">Opinion</span><span class="chip">Ownership</span></div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 4, 2026</span>
          <a href="https://www.autocar.co.uk/opinion/new-cars/ignore-jay-leno-your-dream-garage-only-needs-three-cars" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">58</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/mercedes-big-screens-stay-we-went-too-far-removing-buttons" target="_blank" rel="noopener">Mercedes: Big screens stay—but some buttons return</a>
          <div class="article-take">UX pendulum swings back toward tactile controls after customer feedback.</div>
          <div class="article-tags"><span class="chip">Opinion</span><span class="chip">HMI</span><span class="chip">Mercedes-Benz</span></div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 4, 2026</span>
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