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
        <h1>NHTSA opens probe into 1.2 million Tesla Model 3/Y over front-suspension failures</h1>
        <p class="exec-summary">US safety regulators are examining reports that the front lower lateral link can detach on certain Model 3 and Model Y vehicles, potentially leading to loss of steering control. The review puts Tesla’s largest-volume products under immediate regulatory scrutiny, with possible implications for repairs, costs and brand trust at a moment when the automaker faces softer demand in key markets.</p>

        <div class="takeaways">
          <h3>Key Takeaways</h3>
          <ul>
            <li>Scope covers ~1.2 million vehicles (2018–2020 Model 3; 2021–2023 Model Y), concentrating risk on Tesla’s core lineup.</li>
            <li>156 complaints triggered the probe; outcomes could range from monitoring to a large-scale recall.</li>
            <li>Any mandated fixes would add cost pressure during a period of margin sensitivity for EV makers.</li>
            <li>Heightened regulatory attention may spill over to adjacent Tesla programs (FSD hardware, Autopilot computers).</li>
          </ul>
        </div>

        <div class="impact-row">
          <div class="impact-block">
            <h4>Industry Impact</h4>
            <p>Large-volume safety actions can reshape repair networks, supplier accountability and warranty reserves across the sector. If NHTSA finds systemic issues, the resulting remedy could be one of the largest EV-era suspension campaigns, prompting peers to re-audit fasteners and subframes on skateboard platforms. Expect short-term volatility in Tesla customer sentiment and potential knock-on effects for resale values and fleet risk models.</p>
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
          <span>Source: <b>Electrive</b></span>
          <span>August 3, 2026</span>
          <a href="https://www.electrive.com/2026/08/03/nhtsa-opens-probe-into-1-2-million-teslas/" target="_blank" rel="noopener">Read original →</a>
        </div>

        <div class="related">
          <h4>Related Coverage</h4>
          <ul>
            <li><a href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">NHTSA probes 1.2M Tesla Model 3/Y over suspension failures</a></li>
            <li><a href="https://electrek.co/2026/07/28/tesla-sues-cybertruck-supplier-angstrom-tooling/" target="_blank" rel="noopener">Tesla sues Cybertruck supplier amid standoff keeping production hostage</a></li>
            <li><a href="https://electrek.co/2026/08/03/tesla-fsd-v14-lite-hw3-computer-failures/" target="_blank" rel="noopener">Tesla FSD v14 Lite tied to rising HW3 computer failures, owners report</a></li>
            <li><a href="https://electrek.co/2026/08/04/tesla-china-sales-crash-exports-surge-h1-2026/" target="_blank" rel="noopener">Tesla China sales are crashing as exports surge</a></li>
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
    <h2 class="section-title">Industry Snapshot <span class="count">August 4, 2026</span></h2>
    <div class="dash-grid">
      <div class="stat-panel">
        <h4>Top Manufacturers</h4>
        <ul class="rank-list">
          <li><span>BMW</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:88%"></span></span><span class="rank-count">22</span></li>
          <li><span>Mercedes-Benz</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:84%"></span></span><span class="rank-count">21</span></li>
          <li><span>BYD</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:80%"></span></span><span class="rank-count">20</span></li>
          <li><span>Tesla</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:76%"></span></span><span class="rank-count">19</span></li>
          <li><span>Hyundai/Kia</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:72%"></span></span><span class="rank-count">18</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4>Top Brands</h4>
        <ul class="rank-list">
          <li><span>Audi</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:78%"></span></span><span class="rank-count">18</span></li>
          <li><span>Genesis</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:60%"></span></span><span class="rank-count">14</span></li>
          <li><span>Volkswagen</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:58%"></span></span><span class="rank-count">13</span></li>
          <li><span>Ferrari</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:49%"></span></span><span class="rank-count">11</span></li>
          <li><span>Volvo</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:47%"></span></span><span class="rank-count">10</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4>Top Suppliers</h4>
        <ul class="rank-list">
          <li><span>SK On</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:70%"></span></span><span class="rank-count">9</span></li>
          <li><span>Factorial Energy</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:60%"></span></span><span class="rank-count">8</span></li>
          <li><span>MAHLE</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:52%"></span></span><span class="rank-count">7</span></li>
          <li><span>EVgo</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:41%"></span></span><span class="rank-count">5</span></li>
          <li><span>Allego</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:33%"></span></span><span class="rank-count">4</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4>Most Mentioned Executives</h4>
        <ul class="rank-list">
          <li><span>Ola Källenius (Mercedes)</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:90%"></span></span><span class="rank-count">12</span></li>
          <li><span>Elon Musk (Tesla)</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:82%"></span></span><span class="rank-count">11</span></li>
          <li><span>RJ Scaringe (Rivian)</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:60%"></span></span><span class="rank-count">8</span></li>
          <li><span>Gernot Döllner (Audi)</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:45%"></span></span><span class="rank-count">6</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4>Trending Topics</h4>
        <div class="tagcloud">
          <span class="chip lg">Safety investigations</span>
          <span class="chip">Solid-state batteries</span>
          <span class="chip">Fast charging build-out</span>
          <span class="chip">EV range claims</span>
          <span class="chip">Software-defined vehicles</span>
          <span class="chip">Lidar strategy</span>
          <span class="chip">Dealer network shifts</span>
        </div>
      </div>

      <div class="stat-panel">
        <h4>Emerging Technologies</h4>
        <div class="tagcloud">
          <span class="chip lg">Solid-state cells</span>
          <span class="chip">Iron-air storage</span>
          <span class="chip">Autonomous UI & assistants</span>
          <span class="chip">800V platforms</span>
          <span class="chip">Range-extender for HD trucks</span>
        </div>
      </div>

      <div class="stat-panel">
        <h4>Government & Policy</h4>
        <ul class="rank-list">
          <li><span>NHTSA investigations</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:90%"></span></span><span class="rank-count">12</span></li>
          <li><span>Tariff & trade actions</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:55%"></span></span><span class="rank-count">7</span></li>
          <li><span>Regional EV grants</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:45%"></span></span><span class="rank-count">6</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4>Financial Activity</h4>
        <ul class="rank-list">
          <li><span>Rivian earnings beat</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:86%"></span></span><span class="rank-count">10</span></li>
          <li><span>BYD sales rebound</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:70%"></span></span><span class="rank-count">8</span></li>
          <li><span>Prince Alwaleed in Lucid</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:60%"></span></span><span class="rank-count">7</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4>Global Regions</h4>
        <ul class="rank-list">
          <li><span>Europe (record EV shares)</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:88%"></span></span><span class="rank-count">14</span></li>
          <li><span>China (exports surge)</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:76%"></span></span><span class="rank-count">12</span></li>
          <li><span>US (infrastructure)</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:60%"></span></span><span class="rank-count">9</span></li>
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
        <a href="https://www.autocar.co.uk/car-news/electric-cars/new-mercedes-gla-revealed-audi-q4-rival-408-mile-range" target="_blank" rel="noopener">New Mercedes GLA EV revealed with up to 408-mile range</a>
        <div class="fp-meta"><span>Autocar — Jul 29, 2026</span><span>• Score 86</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/28/bmw-ramps-up-ix3-output-orders-near-100000/" target="_blank" rel="noopener">BMW ramps up iX3 output as orders near 100,000</a>
        <div class="fp-meta"><span>Electrek — Jul 28, 2026</span><span>• Score 78</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/08/04/tesla-china-sales-crash-exports-surge-h1-2026/" target="_blank" rel="noopener">Tesla’s China sales fall while exports surge</a>
        <div class="fp-meta"><span>Electrek — Aug 4, 2026</span><span>• Score 82</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">BMW pauses G-Class rival as China headwinds bite</a>
        <div class="fp-meta"><span>Autocar — Aug 4, 2026</span><span>• Score 75</span></div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Technology</h3>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">SK On and Factorial team up on solid-state batteries</a>
        <div class="fp-meta"><span>Electrek — Jul 29, 2026</span><span>• Score 84</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/waymo-gemini-ai-ojai-robotaxi-redesigned-interface/" target="_blank" rel="noopener">Waymo integrates Gemini AI in robotaxi UI refresh</a>
        <div class="fp-meta"><span>Electrek — Jul 29, 2026</span><span>• Score 77</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.greencarreports.com/news/1146039_ev-battery-recycling-breakthrough-recovers-99-99-of-lithium" target="_blank" rel="noopener">Researchers claim 99.99% lithium recovery in recycling</a>
        <div class="fp-meta"><span>Green Car Reports — Aug 2, 2026</span><span>• Score 76</span></div>
      </div>
      <div class="fp-row">
        <a href="https://chargedevs.com/newswire/mahle-introduces-a-new-range-extender-engine-and-a-rare-earth-free-electric-motor/" target="_blank" rel="noopener">MAHLE unveils HD truck range-extender and rare-earth-free motor</a>
        <div class="fp-meta"><span>Charged EVs — Jul 31, 2026</span><span>• Score 72</span></div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Government</h3>
      <div class="fp-row">
        <a href="https://www.electrive.com/2026/08/03/nhtsa-opens-probe-into-1-2-million-teslas/" target="_blank" rel="noopener">NHTSA opens probe into 1.2M Teslas</a>
        <div class="fp-meta"><span>Electrive — Aug 3, 2026</span><span>• Score 92</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.electrive.com/2026/08/04/denmark-evs-account-for-almost-all-new-car-registrations-in-july/" target="_blank" rel="noopener">Denmark hits 97% EV share for private buyers in July</a>
        <div class="fp-meta"><span>Electrive — Aug 4, 2026</span><span>• Score 79</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.greencarreports.com/news/1146051_gm-pilot-ev-charging-network-now-spans-over-25-states" target="_blank" rel="noopener">GM-Pilot charging network crosses 25 US states</a>
        <div class="fp-meta"><span>Green Car Reports — Aug 4, 2026</span><span>• Score 74</span></div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Suppliers</h3>
      <div class="fp-row">
        <a href="https://chargedevs.com/newswire/beam-global-supplies-ev-arc-off-grid-charging-systems-for-dallas-municipal-fleet-and-massachusetts-carshare-pilot/" target="_blank" rel="noopener">Beam Global expands off-grid charging deployments</a>
        <div class="fp-meta"><span>Charged EVs — Jul 30, 2026</span><span>• Score 68</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.electrive.com/2026/08/04/evgo-and-brixmor-to-add-more-than-500-fast-charging-stalls-in-the-us/" target="_blank" rel="noopener">EVgo, Brixmor to add 500+ DC fast stalls</a>
        <div class="fp-meta"><span>Electrive — Aug 4, 2026</span><span>• Score 73</span></div>
      </div>
      <div class="fp-row">
        <a href="https://chargedevs.com/newswire/automat-solutions-new-lytematch-and-lyteguide-software-platforms-facilitate-battery-electrolyte-development/" target="_blank" rel="noopener">New tools speed electrolyte discovery and design</a>
        <div class="fp-meta"><span>Charged EVs — Aug 1, 2026</span><span>• Score 62</span></div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Trending Topics</h3>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/waymo-gemini-ai-ojai-robotaxi-redesigned-interface/" target="_blank" rel="noopener">AI assistants move inside vehicles</a>
        <div class="fp-meta"><span>Electrek — Jul 29, 2026</span><span>• Score 77</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Volvo exits lidar on EX90/ES90 and compensates owners</a>
        <div class="fp-meta"><span>Electrek — Jul 29, 2026</span><span>• Score 80</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/477795/" target="_blank" rel="noopener">IEA: Global EV sales jump 35% in Q2; 50 countries set records</a>
        <div class="fp-meta"><span>Electrek — Jul 29, 2026</span><span>• Score 81</span></div>
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
    <h2 class="section-title">Latest Articles <span class="count">16 analyzed today</span></h2>
    <div class="article-table">
      
      <div class="article-row">
        <div class="score-chip high">92</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/03/nhtsa-opens-probe-into-1-2-million-teslas/" target="_blank" rel="noopener">NHTSA opens probe into 1.2 million Tesla vehicles over suspension failures</a>
          <div class="article-take">A large-scale safety review puts Tesla’s highest-volume models under intense regulatory pressure and could trigger a costly remedy.</div>
          <div class="article-tags">
            <span class="chip">Tesla</span><span class="chip">NHTSA</span><span class="chip">Safety</span><span class="chip">Recall</span><span class="chip">Government</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrive — Aug 3, 2026</span>
          <a href="https://www.electrive.com/2026/08/03/nhtsa-opens-probe-into-1-2-million-teslas/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip high">88</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/electric-cars/new-mercedes-gla-revealed-audi-q4-rival-408-mile-range" target="_blank" rel="noopener">New Mercedes GLA EV revealed with 408-mile range and 800V fast charging</a>
          <div class="article-take">Mercedes folds its compact lineup into a higher-efficiency EV that pushes mainstream range and charging expectations upward.</div>
          <div class="article-tags">
            <span class="chip">Mercedes-Benz</span><span class="chip">EV</span><span class="chip">Charging</span><span class="chip">Manufacturing</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar — Jul 29, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/electric-cars/new-mercedes-gla-revealed-audi-q4-rival-408-mile-range" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip high">86</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Volvo drops lidar on EX90/ES90, compensates owners</a>
          <div class="article-take">A dramatic ADAS strategy pivot reduces hardware complexity and costs, while forcing market-by-market make-goods.</div>
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
        <div class="score-chip">81</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">SK On and Factorial partner to scale solid-state batteries</a>
          <div class="article-take">A fresh alliance signals accelerating industrialization plans for next-gen cells beyond lab pilots.</div>
          <div class="article-tags">
            <span class="chip">SK On</span><span class="chip">Factorial</span><span class="chip">Battery</span><span class="chip">Solid-state</span>
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
          <a class="headline" href="https://electrek.co/2026/08/04/tesla-china-sales-crash-exports-surge-h1-2026/" target="_blank" rel="noopener">Tesla’s China sales slump while exports surge 127%</a>
          <div class="article-take">Shanghai shifts from local demand engine to export hub, reshaping Tesla’s regional mix and logistics.</div>
          <div class="article-tags">
            <span class="chip">Tesla</span><span class="chip">China</span><span class="chip">Trade</span><span class="chip">Production</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 4, 2026</span>
          <a href="https://electrek.co/2026/08/04/tesla-china-sales-crash-exports-surge-h1-2026/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">79</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/audi-q9-suv-revealed-huge-%C2%A3100k-a8-successor" target="_blank" rel="noopener">Audi reveals Q9 as digital-heavy flagship SUV</a>
          <div class="article-take">Audi leans into in-car experience and hands-free features to anchor its top-end move in key markets.</div>
          <div class="article-tags">
            <span class="chip">Audi</span><span class="chip">ADAS</span><span class="chip">Manufacturers</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar — Jul 31, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/audi-q9-suv-revealed-huge-%C2%A3100k-a8-successor" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">78</div>
        <div class="article-main">
          <a class="headline" href="https://www.greencarreports.com/news/1146051_gm-pilot-ev-charging-network-now-spans-over-25-states" target="_blank" rel="noopener">GM-Pilot EV fast-charging network now in 25+ states</a>
          <div class="article-take">Automaker-backed corridors keep filling in, challenging incumbents on reliability and coverage.</div>
          <div class="article-tags">
            <span class="chip">GM</span><span class="chip">EVgo</span><span class="chip">Charging</span><span class="chip">Infrastructure</span>
          </div>
        </div>
        <div class="article-source">
          <span>Green Car Reports — Aug 4, 2026</span>
          <a href="https://www.greencarreports.com/news/1146051_gm-pilot-ev-charging-network-now-spans-over-25-states" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">75</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">BMW reassesses product roadmap, puts G-Class rival on hold</a>
          <div class="article-take">Macro uncertainty and market divergence force sharper capital discipline on niche programs.</div>
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
        <div class="score-chip">74</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/477795/" target="_blank" rel="noopener">IEA: Global EV sales rebound 35% in Q2; 50 country records</a>
          <div class="article-take">After a soft Q1, demand momentum reasserts, strengthening full-year outlooks for volume players.</div>
          <div class="article-tags">
            <span class="chip">EV</span><span class="chip">Finance</span><span class="chip">Global</span>
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
          <a class="headline" href="https://www.electrive.com/2026/08/04/europe-misses-out-on-billion-euro-battery-cell-profits/" target="_blank" rel="noopener">Europe risks missing out on battery cell value as Asia leads</a>
          <div class="article-take">Supply chains keep tilting East, pressing EU for faster gigafactory execution and local content rules.</div>
          <div class="article-tags">
            <span class="chip">Battery</span><span class="chip">Europe</span><span class="chip">Supply Chain</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrive — Aug 4, 2026</span>
          <a href="https://www.electrive.com/2026/08/04/europe-misses-out-on-billion-euro-battery-cell-profits/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">71</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/28/tesla-sues-cybertruck-supplier-angstrom-tooling/" target="_blank" rel="noopener">Tesla sues Cybertruck supplier to access tooling, avert delays</a>
          <div class="article-take">A dispute over dies spotlights single-point risk in low-volume, unique-stamping programs.</div>
          <div class="article-tags">
            <span class="chip">Tesla</span><span class="chip">Supply Chain</span><span class="chip">Manufacturing</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 28, 2026</span>
          <a href="https://electrek.co/2026/07/28/tesla-sues-cybertruck-supplier-angstrom-tooling/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">70</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/audi-further-strips-a2-e-tron-of-its-camouflage/" target="_blank" rel="noopener">Audi teases ultra-efficient A2 e-tron technical details</a>
          <div class="article-take">Efficiency-first design indicates a new wave of compact premium EVs targeting low cost per mile.</div>
          <div class="article-tags">
            <span class="chip">Audi</span><span class="chip">EV</span><span class="chip">Efficiency</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrive — Aug 4, 2026</span>
          <a href="https://www.electrive.com/2026/08/04/audi-further-strips-a2-e-tron-of-its-camouflage/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">69</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/new-models-vital-ds-survival-uk-sales-hit-record-low" target="_blank" rel="noopener">DS brand faces record-low UK sales; new models critical</a>
          <div class="article-take">A lineup reset and tighter Stellantis positioning will test DS’s path to sustainable niche volumes.</div>
          <div class="article-tags">
            <span class="chip">DS</span><span class="chip">Dealers</span><span class="chip">Strategy</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 4, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/new-models-vital-ds-survival-uk-sales-hit-record-low" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">68</div>
        <div class="article-main">
          <a class="headline" href="https://www.greencarreports.com/news/1146052_here-are-the-evs-made-in-mexico-and-canada" target="_blank" rel="noopener">Which EVs are made in Mexico and Canada amid tariff talk?</a>
          <div class="article-take">Sourcing location stays pivotal for pricing, tax-credit eligibility and near-term market share.</div>
          <div class="article-tags">
            <span class="chip">Trade</span><span class="chip">Manufacturing</span><span class="chip">North America</span>
          </div>
        </div>
        <div class="article-source">
          <span>Green Car Reports — Jul 29, 2026</span>
          <a href="https://www.greencarreports.com/news/1146052_here-are-the-evs-made-in-mexico-and-canada" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">67</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/28/baidu-apollo-go-london-robotaxi-testing-uber-lyft/" target="_blank" rel="noopener">Baidu’s Apollo Go begins London robotaxi testing with Uber & Lyft</a>
          <div class="article-take">China’s AV heavyweight enters a right-hand-drive market with major ride-hail partners in tow.</div>
          <div class="article-tags">
            <span class="chip">Autonomous</span><span class="chip">Mobility</span><span class="chip">Baidu</span><span class="chip">Uber</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 28, 2026</span>
          <a href="https://electrek.co/2026/07/28/baidu-apollo-go-london-robotaxi-testing-uber-lyft/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">66</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/evgo-and-brixmor-to-add-more-than-500-fast-charging-stalls-in-the-us/" target="_blank" rel="noopener">EVgo, Brixmor to install 500+ new DC fast chargers at retail centers</a>
          <div class="article-take">Retail-anchored charging expands convenience and grid diversity for everyday drivers.</div>
          <div class="article-tags">
            <span class="chip">Charging</span><span class="chip">Retail</span><span class="chip">EVgo</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrive — Aug 4, 2026</span>
          <a href="https://www.electrive.com/2026/08/04/evgo-and-brixmor-to-add-more-than-500-fast-charging-stalls-in-the-us/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">64</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/28/mercedes-new-gla-ev-leaks-day-ahead-of-debut/" target="_blank" rel="noopener">Mercedes GLA EV leaks ahead of official debut</a>
          <div class="article-take">Early imagery previews a mainstream entry EV positioned to scale volume quickly.</div>
          <div class="article-tags">
            <span class="chip">Mercedes-Benz</span><span class="chip">EV</span><span class="chip">Product</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 28, 2026</span>
          <a href="https://electrek.co/2026/07/28/mercedes-new-gla-ev-leaks-day-ahead-of-debut/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">63</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/byd-goes-after-defender-boxy-%C2%A348k-402bhp-hybrid-suv" target="_blank" rel="noopener">BYD launches Ti7 hybrid SUV in the UK, undercutting premium rivals</a>
          <div class="article-take">A boxy, performance-leaning PHEV targets Defender buyers at a sharper price point.</div>
          <div class="article-tags">
            <span class="chip">BYD</span><span class="chip">Hybrid</span><span class="chip">UK Market</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar — Jul 31, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/byd-goes-after-defender-boxy-%C2%A348k-402bhp-hybrid-suv" target="_blank" rel="noopener">Read original →</a>
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
    <h2 class="section-title">Industry News <span class="count">Focused highlights</span></h2>
    <div class="article-table">

      <div class="article-row">
        <div class="score-chip high">92</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/03/nhtsa-opens-probe-into-1-2-million-teslas/" target="_blank" rel="noopener">NHTSA opens probe into 1.2M Teslas</a>
          <div class="article-take">A potential high-volume fix could ripple across warranty reserves and service capacity.</div>
          <div class="article-tags">
            <span class="chip">Safety</span><span class="chip">Government</span><span class="chip">Tesla</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrive — Aug 3, 2026</span>
          <a href="https://www.electrive.com/2026/08/03/nhtsa-opens-probe-into-1-2-million-teslas/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      
      <div class="article-row">
        <div class="score-chip">74</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/477795/" target="_blank" rel="noopener">IEA: Global EV sales jump 35% in Q2</a>
          <div class="article-take">Momentum returns, easing fears of an extended demand pause.</div>
          <div class="article-tags">
            <span class="chip">EV</span><span class="chip">Demand</span><span class="chip">Finance</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/477795/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

    </div>
  </div>

  <div class="sec-group reveal" id="electric-vehicles">
    <h2 class="section-title">Electric Vehicles <span class="count">Key launches and shifts</span></h2>
    <div class="article-table">

      <div class="article-row">
        <div class="score-chip high">88</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/electric-cars/new-mercedes-gla-revealed-audi-q4-rival-408-mile-range" target="_blank" rel="noopener">Mercedes GLA EV claims over 400 miles of range</a>
          <div class="article-take">A compact EV pushes premium range norms in the volume sweet spot.</div>
          <div class="article-tags">
            <span class="chip">EV</span><span class="chip">Charging</span><span class="chip">Mercedes-Benz</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar — Jul 29, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/electric-cars/new-mercedes-gla-revealed-audi-q4-rival-408-mile-range" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      
      <div class="article-row">
        <div class="score-chip">80</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/28/bmw-ramps-up-ix3-output-orders-near-100000/" target="_blank" rel="noopener">BMW ramps iX3 production after strong preorders</a>
          <div class="article-take">Scaling a single model fast to capture pent-up demand in the crossover core.</div>
          <div class="article-tags">
            <span class="chip">BMW</span><span class="chip">Production</span><span class="chip">EV</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 28, 2026</span>
          <a href="https://electrek.co/2026/07/28/bmw-ramps-up-ix3-output-orders-near-100000/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

    </div>
  </div>

  <div class="sec-group reveal" id="manufacturers">
    <h2 class="section-title">Manufacturers <span class="count">Strategy and product</span></h2>
    <div class="article-table">

      <div class="article-row">
        <div class="score-chip">75</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">BMW pauses off-roader as market shifts</a>
          <div class="article-take">A real-time reminder that portfolio mix must flex with region-by-region demand.</div>
          <div class="article-tags">
            <span class="chip">BMW</span><span class="chip">Manufacturers</span><span class="chip">Strategy</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 4, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      
      <div class="article-row">
        <div class="score-chip">63</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/byd-goes-after-defender-boxy-%C2%A348k-402bhp-hybrid-suv" target="_blank" rel="noopener">BYD’s Ti7 hybrid SUV undercuts premium rivals</a>
          <div class="article-take">Aggressive pricing meets rugged styling to broaden brand reach in the UK.</div>
          <div class="article-tags">
            <span class="chip">BYD</span><span class="chip">Hybrid</span><span class="chip">UK</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar — Jul 31, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/byd-goes-after-defender-boxy-%C2%A348k-402bhp-hybrid-suv" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

    </div>
  </div>

  <div class="sec-group reveal" id="dealers">
    <h2 class="section-title">Dealers <span class="count">Network & retail</span></h2>
    <div class="article-table">

      <div class="article-row">
        <div class="score-chip">69</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/new-models-vital-ds-survival-uk-sales-hit-record-low" target="_blank" rel="noopener">DS’s UK sales slump; new launches to support dealer viability</a>
          <div class="article-take">A lean premium brand must restore throughput to sustain its network economics.</div>
          <div class="article-tags">
            <span class="chip">DS</span><span class="chip">Dealers</span><span class="chip">Sales</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 4, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/new-models-vital-ds-survival-uk-sales-hit-record-low" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

    </div>
  </div>

  <div class="sec-group reveal" id="suppliers">
    <h2 class="section-title">Suppliers <span class="count">Ecosystem moves</span></h2>
    <div class="article-table">

      <div class="article-row">
        <div class="score-chip">81</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">SK On, Factorial ally on solid-state scale-up</a>
          <div class="article-take">Partnership momentum shifts from pilots to pre-industrial ramp planning.</div>
          <div class="article-tags">
            <span class="chip">Battery</span><span class="chip">Solid-state</span><span class="chip">Suppliers</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      
      <div class="article-row">
        <div class="score-chip">73</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/evgo-and-brixmor-to-add-more-than-500-fast-charging-stalls-in-the-us/" target="_blank" rel="noopener">EVgo and Brixmor expand US DC fast footprint</a>
          <div class="article-take">Shopping-center sites become key nodes in everyday charging behavior.</div>
          <div class="article-tags">
            <span class="chip">EVgo</span><span class="chip">Charging</span><span class="chip">Suppliers</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrive — Aug 4, 2026</span>
          <a href="https://www.electrive.com/2026/08/04/evgo-and-brixmor-to-add-more-than-500-fast-charging-stalls-in-the-us/" target="_blank" rel="noopener">Read original →</a>
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
          <a class="headline" href="https://www.electrive.com/2026/08/03/nhtsa-opens-probe-into-1-2-million-teslas/" target="_blank" rel="noopener">NHTSA’s Tesla probe expands safety scrutiny on EVs</a>
          <div class="article-take">A pivotal case could shape future defect standards on skateboard suspensions.</div>
          <div class="article-tags">
            <span class="chip">NHTSA</span><span class="chip">Safety</span><span class="chip">Government</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrive — Aug 3, 2026</span>
          <a href="https://www.electrive.com/2026/08/03/nhtsa-opens-probe-into-1-2-million-teslas/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">79</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/denmark-evs-account-for-almost-all-new-car-registrations-in-july/" target="_blank" rel="noopener">Denmark’s private EV share nears 98% in July</a>
          <div class="article-take">Sharp incentives and product availability converge to accelerate adoption.</div>
          <div class="article-tags">
            <span class="chip">Government</span><span class="chip">EV Share</span><span class="chip">Europe</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrive — Aug 4, 2026</span>
          <a href="https://www.electrive.com/2026/08/04/denmark-evs-account-for-almost-all-new-car-registrations-in-july/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

    </div>
  </div>

  <div class="sec-group reveal" id="technology">
    <h2 class="section-title">Technology <span class="count">Breakthroughs & software</span></h2>
    <div class="article-table">

      <div class="article-row">
        <div class="score-chip">77</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/waymo-gemini-ai-ojai-robotaxi-redesigned-interface/" target="_blank" rel="noopener">Waymo adds Gemini AI and new rider UI</a>
          <div class="article-take">Natural-language assistance moves from phones to the cabin for AV riders.</div>
          <div class="article-tags">
            <span class="chip">Autonomous</span><span class="chip">Software</span><span class="chip">AI</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/waymo-gemini-ai-ojai-robotaxi-redesigned-interface/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      
      <div class="article-row">
        <div class="score-chip">76</div>
        <div class="article-main">
          <a class="headline" href="https://www.greencarreports.com/news/1146039_ev-battery-recycling-breakthrough-recovers-99-99-of-lithium" target="_blank" rel="noopener">Study claims 99.99% lithium recovery from used EV batteries</a>
          <div class="article-take">Higher recovery factors could meaningfully lower cell costs and primary mining demand.</div>
          <div class="article-tags">
            <span class="chip">Battery</span><span class="chip">Recycling</span><span class="chip">Sustainability</span>
          </div>
        </div>
        <div class="article-source">
          <span>Green Car Reports — Aug 2, 2026</span>
          <a href="https://www.greencarreports.com/news/1146039_ev-battery-recycling-breakthrough-recovers-99-99-of-lithium" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

    </div>
  </div>

  <div class="sec-group reveal" id="finance">
    <h2 class="section-title">Finance <span class="count">Earnings & deals</span></h2>
    <div class="article-table">

      <div class="article-row">
        <div class="score-chip">78</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/03/rivian-boosts-q2-revenue-and-reduces-losses/" target="_blank" rel="noopener">Rivian grows Q2 revenue 27% and narrows losses</a>
          <div class="article-take">Volume lift and mix improvements support a more durable gross profit trajectory.</div>
          <div class="article-tags">
            <span class="chip">Rivian</span><span class="chip">Earnings</span><span class="chip">Finance</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrive — Aug 3, 2026</span>
          <a href="https://www.electrive.com/2026/08/03/rivian-boosts-q2-revenue-and-reduces-losses/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      
      <div class="article-row">
        <div class="score-chip">70</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/28/saudi-prince-alwaleed-5-percent-lucid-stake-lcid/" target="_blank" rel="noopener">Prince Alwaleed discloses 5% Lucid stake; shares jump</a>
          <div class="article-take">A high-profile backer signals continued sovereign support for the EV challenger.</div>
          <div class="article-tags">
            <span class="chip">Lucid</span><span class="chip">Finance</span><span class="chip">Capital</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 28, 2026</span>
          <a href="https://electrek.co/2026/07/28/saudi-prince-alwaleed-5-percent-lucid-stake-lcid/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

    </div>
  </div>

  <div class="sec-group reveal" id="international">
    <h2 class="section-title">International <span class="count">Global markets</span></h2>
    <div class="article-table">

      <div class="article-row">
        <div class="score-chip">80</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/04/tesla-china-sales-crash-exports-surge-h1-2026/" target="_blank" rel="noopener">Tesla pivots Shanghai output to exports amid China slowdown</a>
          <div class="article-take">Allocation changes rebalance inventory risk but complicate lead times by region.</div>
          <div class="article-tags">
            <span class="chip">China</span><span class="chip">Manufacturing</span><span class="chip">Tesla</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 4, 2026</span>
          <a href="https://electrek.co/2026/08/04/tesla-china-sales-crash-exports-surge-h1-2026/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      
      <div class="article-row">
        <div class="score-chip">72</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/03/norways-ev-share-rises-to-97-6-in-july/" target="_blank" rel="noopener">Norway’s EV share rises to 97.6% in July</a>
          <div class="article-take">The bellwether market demonstrates what mature adoption looks like at scale.</div>
          <div class="article-tags">
            <span class="chip">Norway</span><span class="chip">EV Share</span><span class="chip">Policy</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrive — Aug 3, 2026</span>
          <a href="https://www.electrive.com/2026/08/03/norways-ev-share-rises-to-97-6-in-july/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

    </div>
  </div>

  <div class="sec-group reveal" id="opinion">
    <h2 class="section-title">Opinion <span class="count">Perspectives</span></h2>
    <div class="article-table">

      <div class="article-row">
        <div class="score-chip">60</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/opinion/new-cars/ignore-jay-leno-your-dream-garage-only-needs-three-cars" target="_blank" rel="noopener">Ignore Jay Leno: your dream garage only needs three cars</a>
          <div class="article-take">A case for curation over collection in the age of endless choice.</div>
          <div class="article-tags">
            <span class="chip">Opinion</span><span class="chip">Enthusiast</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 4, 2026</span>
          <a href="https://www.autocar.co.uk/opinion/new-cars/ignore-jay-leno-your-dream-garage-only-needs-three-cars" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      
      <div class="article-row">
        <div class="score-chip">58</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/business-manufacturing/chinese-car-makers-all-share-parts-will-world-follow" target="_blank" rel="noopener">Chinese car makers all share parts — will the world follow?</a>
          <div class="article-take">Standardization trims costs and time-to-market, but challenges brand differentiation.</div>
          <div class="article-tags">
            <span class="chip">Supply Chain</span><span class="chip">China</span><span class="chip">Opinion</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 4, 2026</span>
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