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
        <p class="exec-summary">US safety regulators launched a preliminary investigation into 2018–2020 Model 3 and 2021–2023 Model Y vehicles after reports that a front lower lateral link can detach while driving. The probe puts fresh scrutiny on Tesla’s quality controls and could culminate in a large recall with material, supplier and service-center implications across the company’s biggest-volume products.</p>

        <div class="takeaways">
          <h3>Key Takeaways</h3>
          <ul>
            <li>Scope covers roughly 1.2 million vehicles after 156 complaints tied to a lower control-arm separation; investigators will assess design, parts and assembly processes.</li>
            <li>A recall would hit Tesla’s most common models, straining parts supply and service lane capacity heading into peak delivery months.</li>
            <li>Safety scrutiny intensifies alongside other Tesla issues (software/ADAS and hardware reliability), amplifying regulatory and insurance pressure.</li>
            <li>Outcome may ripple to Tier‑1/2 suppliers and set new validation expectations for EV chassis components industry‑wide.</li>
          </ul>
        </div>

        <div class="impact-row">
          <div class="impact-block">
            <h4>Industry Impact</h4>
            <p>Large-scale corrective action on a high-volume EV platform would reinforce that electrification does not relax legacy safety and durability disciplines. Expect heightened supplier audits, more conservative validation timelines and elevated warranty provisioning across OEMs scaling new EV nameplates. If repair rates are significant, used‑EV residuals and insurance pricing on affected VIN ranges could shift as well.</p>
          </div>
          <div class="impact-block">
            <h4>Companies Affected</h4>
            <div class="chip-row">
              <span class="chip entity-mfr">Tesla</span>
              <span class="chip">NHTSA</span>
              <span class="chip">Tier‑1 chassis suppliers</span>
              <span class="chip">US dealers & repair networks</span>
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
            <li><a href="https://www.electrive.com/2026/08/03/nhtsa-opens-probe-into-1-2-million-teslas/" target="_blank" rel="noopener">NHTSA opens probe into 1.2 million Teslas</a></li>
            <li><a href="https://electrek.co/2026/08/03/tesla-fsd-v14-lite-hw3-computer-failures/" target="_blank" rel="noopener">Owners report HW3 computer failures after FSD v14 “Lite” update</a></li>
            <li><a href="https://electrek.co/2026/07/28/tesla-sues-cybertruck-supplier-angstrom-tooling/" target="_blank" rel="noopener">Tesla sues Cybertruck supplier over access to tooling</a></li>
          </ul>
        </div>
      </div>

      <div class="hero-gauges">
        <div class="gauge">
          <svg viewBox="0 0 120 70"><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#2a3038" stroke-width="8"/><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#f2a93b" stroke-width="8" stroke-dasharray="157" stroke-dashoffset="12.56"/></svg>
          <span class="gauge-value mono">92</span>
          <span class="gauge-label">Importance</span>
        </div>
        <div class="gauge">
          <svg viewBox="0 0 120 70"><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#2a3038" stroke-width="8"/><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#3ecf8e" stroke-width="8" stroke-dasharray="157" stroke-dashoffset="15.70"/></svg>
          <span class="gauge-value mono">90</span>
          <span class="gauge-label">Editorial Quality</span>
        </div>
        <div class="gauge">
          <svg viewBox="0 0 120 70"><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#2a3038" stroke-width="8"/><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#e2604f" stroke-width="8" stroke-dasharray="157" stroke-dashoffset="14.13"/></svg>
          <span class="gauge-value mono">91</span>
          <span class="gauge-label">Industry Impact</span>
        </div>
        <div class="gauge">
          <svg viewBox="0 0 120 70"><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#2a3038" stroke-width="8"/><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#f2a93b" stroke-width="8" stroke-dasharray="157" stroke-dashoffset="9.42"/></svg>
          <span class="gauge-value mono">94</span>
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
          <li><span>BYD</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:85%"></span></span><span class="rank-count">8</span></li>
          <li><span>Hyundai/Kia</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:78%"></span></span><span class="rank-count">7</span></li>
          <li><span>BMW</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:67%"></span></span><span class="rank-count">6</span></li>
          <li><span>Mercedes‑Benz</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:56%"></span></span><span class="rank-count">5</span></li>
          <li><span>Volkswagen</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:44%"></span></span><span class="rank-count">4</span></li>
          <li><span>Rivian</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:33%"></span></span><span class="rank-count">3</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4>Top Brands</h4>
        <ul class="rank-list">
          <li><span>Audi</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:90%"></span></span><span class="rank-count">6</span></li>
          <li><span>Volvo</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:75%"></span></span><span class="rank-count">5</span></li>
          <li><span>Genesis</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:60%"></span></span><span class="rank-count">4</span></li>
          <li><span>Toyota</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:45%"></span></span><span class="rank-count">3</span></li>
          <li><span>DS Automobiles</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:30%"></span></span><span class="rank-count">2</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4>Top Suppliers & Infrastructure</h4>
        <ul class="rank-list">
          <li><span>SK On</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:100%"></span></span><span class="rank-count">3</span></li>
          <li><span>Factorial Energy</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:90%"></span></span><span class="rank-count">3</span></li>
          <li><span>EVgo</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:80%"></span></span><span class="rank-count">2</span></li>
          <li><span>Brixmor</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:70%"></span></span><span class="rank-count">2</span></li>
          <li><span>Allego</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:60%"></span></span><span class="rank-count">2</span></li>
          <li><span>Luminar (former)</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:50%"></span></span><span class="rank-count">1</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4>Most Mentioned Executives</h4>
        <ul class="rank-list">
          <li><span>Elon Musk (Tesla)</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:100%"></span></span><span class="rank-count">5</span></li>
          <li><span>Ola Källenius (Mercedes‑Benz)</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:80%"></span></span><span class="rank-count">4</span></li>
          <li><span>Michael Leiters (Porsche)</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:60%"></span></span><span class="rank-count">3</span></li>
          <li><span>RJ Scaringe (Rivian)</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:60%"></span></span><span class="rank-count">3</span></li>
          <li><span>Jim Baumbick (Ford Europe)</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:40%"></span></span><span class="rank-count">2</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4>Trending Topics</h4>
        <div class="tagcloud">
          <span class="chip lg">Safety probes</span>
          <span class="chip">Robotaxis</span>
          <span class="chip">Solid‑state batteries</span>
          <span class="chip">Charging build‑out</span>
          <span class="chip">China exports</span>
          <span class="chip">Software‑defined vehicles</span>
          <span class="chip">Lidar strategy</span>
          <span class="chip">EV affordability</span>
        </div>
      </div>

      <div class="stat-panel">
        <h4>Emerging Technologies</h4>
        <div class="tagcloud">
          <span class="chip lg">Solid‑state cells</span>
          <span class="chip">Iron‑air storage</span>
          <span class="chip">800V platforms</span>
          <span class="chip">AI in UX</span>
          <span class="chip">V2L/VPP</span>
        </div>
      </div>

      <div class="stat-panel">
        <h4>Government & Policy</h4>
        <ul class="rank-list">
          <li><span>NHTSA Tesla probe</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:100%"></span></span><span class="rank-count">1</span></li>
          <li><span>Denmark EV share 97.6%</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:80%"></span></span><span class="rank-count">1</span></li>
          <li><span>Philippines EV incentives</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:70%"></span></span><span class="rank-count">1</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4>Supplier & Network Activity</h4>
        <ul class="rank-list">
          <li><span>EVgo + Brixmor add 500 DCFC</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:95%"></span></span><span class="rank-count">1</span></li>
          <li><span>Allego invests €100M UK</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:75%"></span></span><span class="rank-count">1</span></li>
          <li><span>SK On + Factorial alliance</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:75%"></span></span><span class="rank-count">1</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4>Financial & Markets</h4>
        <ul class="rank-list">
          <li><span>Rivian Q2 margin gains</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:100%"></span></span><span class="rank-count">1</span></li>
          <li><span>BYD July +22%</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:85%"></span></span><span class="rank-count">1</span></li>
          <li><span>Global EV sales +35% QoQ</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:80%"></span></span><span class="rank-count">1</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4>Global Regions</h4>
        <ul class="rank-list">
          <li><span>United States</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:100%"></span></span><span class="rank-count">12</span></li>
          <li><span>China</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:80%"></span></span><span class="rank-count">9</span></li>
          <li><span>Europe (UK/EU)</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:75%"></span></span><span class="rank-count">8</span></li>
          <li><span>Nordics</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:55%"></span></span><span class="rank-count">4</span></li>
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
        <a href="https://www.autocar.co.uk/car-news/electric-cars/new-mercedes-gla-revealed-audi-q4-rival-408-mile-range" target="_blank" rel="noopener">Mercedes unveils new GLA EV with up to 408 miles of range</a>
        <div class="fp-meta"><span>Score 86</span><span>•</span><span>Autocar • Jul 29, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/hyundai-reveals-ioniq-3-prices-start-30000-interest-surges/" target="_blank" rel="noopener">Hyundai IONIQ 3 targets ~$30k with strong preorder interest</a>
        <div class="fp-meta"><span>Score 80</span><span>•</span><span>Electrek • Jul 29, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">BMW pauses G‑Class rival as strategy resets amid China headwinds</a>
        <div class="fp-meta"><span>Score 82</span><span>•</span><span>Autocar • Aug 4, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/08/03/byd-opens-denza-z9s-pre-orders-record-1100-km-ev-range/" target="_blank" rel="noopener">BYD’s Denza Z9S claims 1,100 km range under $50k</a>
        <div class="fp-meta"><span>Score 78</span><span>•</span><span>Electrek • Aug 3, 2026</span></div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Technology</h3>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">SK On and Factorial team to scale solid‑state batteries</a>
        <div class="fp-meta"><span>Score 84</span><span>•</span><span>Electrek • Jul 29, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/waymo-gemini-ai-ojai-robotaxi-redesigned-interface/" target="_blank" rel="noopener">Waymo integrates Google Gemini AI into Ojai robotaxi UX</a>
        <div class="fp-meta"><span>Score 79</span><span>•</span><span>Electrek • Jul 29, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Volvo ditches lidar on EX90/ES90, compensates owners</a>
        <div class="fp-meta"><span>Score 85</span><span>•</span><span>Electrek • Jul 29, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/08/03/tesla-fsd-v14-lite-hw3-computer-failures/" target="_blank" rel="noopener">Reports tie FSD v14 “Lite” to overheating HW3 computers</a>
        <div class="fp-meta"><span>Score 81</span><span>•</span><span>Electrek • Aug 3, 2026</span></div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Government</h3>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">NHTSA probes 1.2M Teslas over suspension link failures</a>
        <div class="fp-meta"><span>Score 92</span><span>•</span><span>Electrek • Jul 31, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.electrive.com/2026/08/04/denmark-evs-account-for-almost-all-new-car-registrations-in-july/" target="_blank" rel="noopener">Denmark hits 97.6% EV share in July registrations</a>
        <div class="fp-meta"><span>Score 75</span><span>•</span><span>electrive • Aug 4, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.electrive.com/2026/08/04/philippines-launches-e850m-incentive-programme-for-ev-manufacturing/" target="_blank" rel="noopener">Philippines unveils €850m EV manufacturing incentives</a>
        <div class="fp-meta"><span>Score 73</span><span>•</span><span>electrive • Aug 4, 2026</span></div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Suppliers & Charging</h3>
      <div class="fp-row">
        <a href="https://www.electrive.com/2026/08/04/evgo-and-brixmor-to-add-more-than-500-fast-charging-stalls-in-the-us/" target="_blank" rel="noopener">EVgo + Brixmor to deploy 500+ new DC fast stalls</a>
        <div class="fp-meta"><span>Score 76</span><span>•</span><span>electrive • Aug 4, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.electrive.com/2026/08/01/allego-commits-e100-million-to-expand-uk-charging-network/" target="_blank" rel="noopener">Allego invests €100M to expand UK ultra‑rapid network</a>
        <div class="fp-meta"><span>Score 70</span><span>•</span><span>electrive • Aug 1, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.electrive.com/2026/08/04/greenmobility-to-bring-weride-robotaxis-to-denmark/" target="_blank" rel="noopener">WeRide to supply robotaxis for GreenMobility in Denmark</a>
        <div class="fp-meta"><span>Score 69</span><span>•</span><span>electrive • Aug 4, 2026</span></div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Trending Topics</h3>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/477795/" target="_blank" rel="noopener">IEA: Q2 EV sales rebound 35%, records in 50 countries</a>
        <div class="fp-meta"><span>Score 83</span><span>•</span><span>Electrek • Jul 29, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/28/baidu-apollo-go-london-robotaxi-testing-uber-lyft/" target="_blank" rel="noopener">Baidu Apollo Go starts robotaxi testing in London</a>
        <div class="fp-meta"><span>Score 75</span><span>•</span><span>Electrek • Jul 28, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/28/volkswagen-launches-cheaper-id-polo-ev-orders-25000/" target="_blank" rel="noopener">Volkswagen opens cheaper ID. Polo pre‑orders after 25k reservations</a>
        <div class="fp-meta"><span>Score 77</span><span>•</span><span>Electrek • Jul 28, 2026</span></div>
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
        <div class="score-chip high">92</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">NHTSA opens probe into 1.2 million Teslas over suspension failures</a>
          <div class="article-take">A large‑scope safety inquiry on Tesla’s core models could force a costly recall and tighter supplier oversight.</div>
          <div class="article-tags">
            <span class="chip">Safety</span>
            <span class="chip">Government</span>
            <span class="chip">Tesla</span>
            <span class="chip">NHTSA</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek</span>
          <span>Jul 31, 2026</span>
          <a href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip high">86</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/electric-cars/new-mercedes-gla-revealed-audi-q4-rival-408-mile-range" target="_blank" rel="noopener">New Mercedes GLA EV revealed with up to 408‑mile range</a>
          <div class="article-take">Mercedes pushes compact EV efficiency and 800V fast‑charging into a volume crossover segment.</div>
          <div class="article-tags">
            <span class="chip">EV</span>
            <span class="chip">Manufacturing</span>
            <span class="chip">Mercedes‑Benz</span>
            <span class="chip">Battery</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar</span>
          <span>Jul 29, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/electric-cars/new-mercedes-gla-revealed-audi-q4-rival-408-mile-range" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip high">85</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Volvo drops lidar on EX90/ES90, pays owners compensation</a>
          <div class="article-take">A strategic pivot away from lidar tightens Volvo’s cost and complexity—but invites debate on ADAS sensing stacks.</div>
          <div class="article-tags">
            <span class="chip">ADAS</span>
            <span class="chip">Volvo</span>
            <span class="chip">Suppliers</span>
            <span class="chip">Lidar</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek</span>
          <span>Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">79</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/waymo-gemini-ai-ojai-robotaxi-redesigned-interface/" target="_blank" rel="noopener">Waymo adds Google’s Gemini AI and new UI to Ojai robotaxi</a>
          <div class="article-take">Conversational AI becomes a front‑end differentiator as robotaxi UX moves beyond maps and buttons.</div>
          <div class="article-tags">
            <span class="chip">Autonomous</span>
            <span class="chip">Software</span>
            <span class="chip">Waymo</span>
            <span class="chip">AI</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek</span>
          <span>Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/waymo-gemini-ai-ojai-robotaxi-redesigned-interface/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">78</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/28/baidu-apollo-go-london-robotaxi-testing-uber-lyft/" target="_blank" rel="noopener">Baidu’s Apollo Go begins London robotaxi testing</a>
          <div class="article-take">China’s AV leader extends its footprint to a right‑hand‑drive market with ride‑hailing partners in tow.</div>
          <div class="article-tags">
            <span class="chip">Autonomous</span>
            <span class="chip">Baidu</span>
            <span class="chip">International</span>
            <span class="chip">Mobility</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek</span>
          <span>Jul 28, 2026</span>
          <a href="https://electrek.co/2026/07/28/baidu-apollo-go-london-robotaxi-testing-uber-lyft/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip high">83</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/477795/" target="_blank" rel="noopener">IEA: Global EV sales jump 35% in Q2; 50 countries set records</a>
          <div class="article-take">EV demand rebounded broadly, underscoring resilience despite pricing resets and macro uncertainty.</div>
          <div class="article-tags">
            <span class="chip">EV</span>
            <span class="chip">Market</span>
            <span class="chip">IEA</span>
            <span class="chip">Finance</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek</span>
          <span>Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/477795/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">80</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/hyundai-reveals-ioniq-3-prices-start-30000-interest-surges/" target="_blank" rel="noopener">Hyundai’s IONIQ 3 starts around $30,000 with high interest</a>
          <div class="article-take">A value‑priced compact EV with 300+ miles range intensifies mainstream price competition.</div>
          <div class="article-tags">
            <span class="chip">Hyundai</span>
            <span class="chip">EV</span>
            <span class="chip">Retail</span>
            <span class="chip">Production</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek</span>
          <span>Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/hyundai-reveals-ioniq-3-prices-start-30000-interest-surges/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">74</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/28/volkswagen-launches-cheaper-id-polo-ev-orders-25000/" target="_blank" rel="noopener">Volkswagen launches cheaper ID. Polo EV after 25k orders</a>
          <div class="article-take">VW leans into sub‑€30k EVs to meet demand in cost‑sensitive segments.</div>
          <div class="article-tags">
            <span class="chip">Volkswagen</span>
            <span class="chip">EV</span>
            <span class="chip">Europe</span>
            <span class="chip">Retail</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek</span>
          <span>Jul 28, 2026</span>
          <a href="https://electrek.co/2026/07/28/volkswagen-launches-cheaper-id-polo-ev-orders-25000/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">72</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/30/bmw-opens-i3-orders-months-early-demand-surges/" target="_blank" rel="noopener">BMW opens new i3 orders months early amid high demand</a>
          <div class="article-take">Strong early interest accelerates BMW’s compact EV rollout plans.</div>
          <div class="article-tags">
            <span class="chip">BMW</span>
            <span class="chip">Production</span>
            <span class="chip">EV</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek</span>
          <span>Jul 30, 2026</span>
          <a href="https://electrek.co/2026/07/30/bmw-opens-i3-orders-months-early-demand-surges/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">78</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/03/byd-opens-denza-z9s-pre-orders-record-1100-km-ev-range/" target="_blank" rel="noopener">BYD opens Denza Z9S pre‑orders with 1,100 km EV range</a>
          <div class="article-take">Long‑range flagship sharpens BYD’s premium push at aggressive price points.</div>
          <div class="article-tags">
            <span class="chip">BYD</span>
            <span class="chip">EV</span>
            <span class="chip">Battery</span>
            <span class="chip">China</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek</span>
          <span>Aug 3, 2026</span>
          <a href="https://electrek.co/2026/08/03/byd-opens-denza-z9s-pre-orders-record-1100-km-ev-range/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">81</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/28/tesla-sues-cybertruck-supplier-angstrom-tooling/" target="_blank" rel="noopener">Tesla sues Cybertruck supplier to retrieve tooling amid plant closure</a>
          <div class="article-take">A legal standoff over tooling access spotlights risk concentration in low‑volume, unique body programs.</div>
          <div class="article-tags">
            <span class="chip">Tesla</span>
            <span class="chip">Supply Chain</span>
            <span class="chip">Manufacturing</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek</span>
          <span>Jul 28, 2026</span>
          <a href="https://electrek.co/2026/07/28/tesla-sues-cybertruck-supplier-angstrom-tooling/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">81</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/03/tesla-fsd-v14-lite-hw3-computer-failures/" target="_blank" rel="noopener">Owners report HW3 Autopilot computer failures after FSD v14 “Lite”</a>
          <div class="article-take">Thermal load from new software builds may be exposing hardware headroom limits on older ECUs.</div>
          <div class="article-tags">
            <span class="chip">Software</span>
            <span class="chip">ADAS</span>
            <span class="chip">Tesla</span>
            <span class="chip">Safety</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek</span>
          <span>Aug 3, 2026</span>
          <a href="https://electrek.co/2026/08/03/tesla-fsd-v14-lite-hw3-computer-failures/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">80</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/04/tesla-china-sales-crash-exports-surge-h1-2026/" target="_blank" rel="noopener">Tesla’s China sales fall as Shanghai exports surge 127%</a>
          <div class="article-take">Pivot to exports helps utilization but underscores rising competitive pressure in China’s home market.</div>
          <div class="article-tags">
            <span class="chip">Tesla</span>
            <span class="chip">China</span>
            <span class="chip">Trade</span>
            <span class="chip">Market</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek</span>
          <span>Aug 4, 2026</span>
          <a href="https://electrek.co/2026/08/04/tesla-china-sales-crash-exports-surge-h1-2026/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip high">84</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/30/rivian-rivn-q2-2026-earnings-r2-deliveries-revenue-up-27/" target="_blank" rel="noopener">Rivian Q2: revenue up 27%, record gross profit, R2 deliveries begin</a>
          <div class="article-take">Scaling the sub‑$50k R2 with improving unit economics shifts Rivian closer to sustainable growth.</div>
          <div class="article-tags">
            <span class="chip">Rivian</span>
            <span class="chip">Finance</span>
            <span class="chip">EV</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek</span>
          <span>Jul 30, 2026</span>
          <a href="https://electrek.co/2026/07/30/rivian-rivn-q2-2026-earnings-r2-deliveries-revenue-up-27/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">77</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/audi-further-strips-a2-e-tron-of-its-camouflage/" target="_blank" rel="noopener">Audi shares A2 e‑tron technical details ahead of fall debut</a>
          <div class="article-take">Efficiency‑first packaging positions Audi’s compact EV as a premium take on ID.3 class hardware.</div>
          <div class="article-tags">
            <span class="chip">Audi</span>
            <span class="chip">EV</span>
            <span class="chip">Efficiency</span>
          </div>
        </div>
        <div class="article-source">
          <span>electrive</span>
          <span>Aug 4, 2026</span>
          <a href="https://www.electrive.com/2026/08/04/audi-further-strips-a2-e-tron-of-its-camouflage/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip high">84</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">SK On and Factorial join forces to scale “breakthrough” solid‑state tech</a>
          <div class="article-take">A cell‑maker/startup pairing aims to speed industrialization from pilot to automotive volumes.</div>
          <div class="article-tags">
            <span class="chip">Battery</span>
            <span class="chip">Solid‑state</span>
            <span class="chip">Suppliers</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek</span>
          <span>Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">76</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/evgo-and-brixmor-to-add-more-than-500-fast-charging-stalls-in-the-us/" target="_blank" rel="noopener">EVgo and Brixmor to add 500+ fast‑charging stalls at retail centers</a>
          <div class="article-take">Co‑location with shopping trips strengthens utilization economics for public DC fast charging.</div>
          <div class="article-tags">
            <span class="chip">Charging</span>
            <span class="chip">EVgo</span>
            <span class="chip">Retail</span>
          </div>
        </div>
        <div class="article-source">
          <span>electrive</span>
          <span>Aug 4, 2026</span>
          <a href="https://www.electrive.com/2026/08/04/evgo-and-brixmor-to-add-more-than-500-fast-charging-stalls-in-the-us/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">75</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/03/norways-ev-share-rises-to-97-6-in-july/" target="_blank" rel="noopener">Norway’s EV share hits 97.6% in July</a>
          <div class="article-take">The world’s leading EV market shows how incentives, choice and infrastructure sustain adoption.</div>
          <div class="article-tags">
            <span class="chip">International</span>
            <span class="chip">EV adoption</span>
            <span class="chip">Policy</span>
          </div>
        </div>
        <div class="article-source">
          <span>electrive</span>
          <span>Aug 3, 2026</span>
          <a href="https://www.electrive.com/2026/08/03/norways-ev-share-rises-to-97-6-in-july/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">74</div>
        <div class="article-main">
          <a class="headline" href="https://www.caranddriver.com/news/a73337003/hyundai-kia-genesis-record-sales-july-2026/" target="_blank" rel="noopener">Hyundai, Kia and Genesis post record July US sales</a>
          <div class="article-take">Hybrids and new EVs are driving incremental volume despite a mixed macro backdrop.</div>
          <div class="article-tags">
            <span class="chip">Hyundai</span>
            <span class="chip">Kia</span>
            <span class="chip">Sales</span>
            <span class="chip">Hybrid</span>
          </div>
        </div>
        <div class="article-source">
          <span>Car and Driver</span>
          <span>Aug 3, 2026</span>
          <a href="https://www.caranddriver.com/news/a73337003/hyundai-kia-genesis-record-sales-july-2026/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">73</div>
        <div class="article-main">
          <a class="headline" href="https://www.caranddriver.com/news/a73317556/ford-ceo-chinese-automaker-arrival-warning/" target="_blank" rel="noopener">Ford CEO warns Chinese automakers could enter US within 5–10 years</a>
          <div class="article-take">Expect intensified pricing pressure and fresh distribution models if trade barriers ease.</div>
          <div class="article-tags">
            <span class="chip">Trade</span>
            <span class="chip">China</span>
            <span class="chip">Competition</span>
            <span class="chip">Ford</span>
          </div>
        </div>
        <div class="article-source">
          <span>Car and Driver</span>
          <span>Jul 31, 2026</span>
          <a href="https://www.caranddriver.com/news/a73317556/ford-ceo-chinese-automaker-arrival-warning/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip high">82</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">BMW puts G‑Class rival on hold as China headwinds hit</a>
          <div class="article-take">Product planning flexes to regional demand shifts and profit protection amid tariff and FX volatility.</div>
          <div class="article-tags">
            <span class="chip">BMW</span>
            <span class="chip">Strategy</span>
            <span class="chip">China</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar</span>
          <span>Aug 4, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">68</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/new-models-vital-ds-survival-uk-sales-hit-record-low" target="_blank" rel="noopener">New models vital to DS survival as UK sales hit record low</a>
          <div class="article-take">A lineup reset (N°3, N°7) must land to stabilize dealer economics in a shrinking niche.</div>
          <div class="article-tags">
            <span class="chip">DS Automobiles</span>
            <span class="chip">Dealers</span>
            <span class="chip">Sales</span>
            <span class="chip">Europe</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar</span>
          <span>Aug 4, 2026</span>
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
    <h2 class="section-title">Industry News <span class="count">3</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip high">83</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/477795/" target="_blank" rel="noopener">IEA: Global EV sales jump 35% in Q2; 50 countries set records</a>
          <div class="article-take">Momentum returns broadly, setting a higher baseline for H2 planning.</div>
          <div class="article-tags">
            <span class="chip">Market</span><span class="chip">EV</span><span class="chip">IEA</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek</span><span>Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/477795/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip high">82</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">BMW pauses G‑Class rival amid reassessed product strategy</a>
          <div class="article-take">OEMs are tightening investment gates as regional demand diverges.</div>
          <div class="article-tags">
            <span class="chip">BMW</span><span class="chip">Strategy</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar</span><span>Aug 4, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">74</div>
        <div class="article-main">
          <a class="headline" href="https://www.caranddriver.com/news/a73337003/hyundai-kia-genesis-record-sales-july-2026/" target="_blank" rel="noopener">Hyundai, Kia and Genesis notch record July US sales</a>
          <div class="article-take">Hybrid mix buoyed volumes as lineups refreshed across segments.</div>
          <div class="article-tags">
            <span class="chip">Sales</span><span class="chip">Hyundai</span><span class="chip">Kia</span>
          </div>
        </div>
        <div class="article-source">
          <span>Car and Driver</span><span>Aug 3, 2026</span>
          <a href="https://www.caranddriver.com/news/a73337003/hyundai-kia-genesis-record-sales-july-2026/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="electric-vehicles">
    <h2 class="section-title">Electric Vehicles <span class="count">3</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip high">86</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/electric-cars/new-mercedes-gla-revealed-audi-q4-rival-408-mile-range" target="_blank" rel="noopener">Mercedes’ new GLA EV brings 408‑mile range and 800V charging</a>
          <div class="article-take">A strong efficiency play in a critical premium compact segment.</div>
          <div class="article-tags">
            <span class="chip">Mercedes‑Benz</span><span class="chip">EV</span><span class="chip">Battery</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar</span><span>Jul 29, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/electric-cars/new-mercedes-gla-revealed-audi-q4-rival-408-mile-range" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">80</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/hyundai-reveals-ioniq-3-prices-start-30000-interest-surges/" target="_blank" rel="noopener">IONIQ 3 priced near $30k with 300+ miles of range</a>
          <div class="article-take">Hyundai sharpens the value equation in mainstream EVs.</div>
          <div class="article-tags">
            <span class="chip">Hyundai</span><span class="chip">EV</span><span class="chip">Retail</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek</span><span>Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/hyundai-reveals-ioniq-3-prices-start-30000-interest-surges/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">74</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/28/volkswagen-launches-cheaper-id-polo-ev-orders-25000/" target="_blank" rel="noopener">VW opens cheaper ID. Polo EV pre‑orders after strong demand</a>
          <div class="article-take">A sub‑€30k city EV anchors affordability for Europe.</div>
          <div class="article-tags">
            <span class="chip">Volkswagen</span><span class="chip">EV</span><span class="chip">Europe</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek</span><span>Jul 28, 2026</span>
          <a href="https://electrek.co/2026/07/28/volkswagen-launches-cheaper-id-polo-ev-orders-25000/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="manufacturers">
    <h2 class="section-title">Manufacturers <span class="count">3</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip high">84</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/30/rivian-rivn-q2-2026-earnings-r2-deliveries-revenue-up-27/" target="_blank" rel="noopener">Rivian posts record gross profit as R2 deliveries begin</a>
          <div class="article-take">Execution on a lower‑cost platform is moving the P&L in the right direction.</div>
          <div class="article-tags">
            <span class="chip">Rivian</span><span class="chip">Finance</span><span class="chip">Production</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek</span><span>Jul 30, 2026</span>
          <a href="https://electrek.co/2026/07/30/rivian-rivn-q2-2026-earnings-r2-deliveries-revenue-up-27/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">77</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/audi-further-strips-a2-e-tron-of-its-camouflage/" target="_blank" rel="noopener">Audi previews A2 e‑tron efficiency‑focused compact</a>
          <div class="article-take">Aero and new LFP pack target top‑tier range per kWh in the class.</div>
          <div class="article-tags">
            <span class="chip">Audi</span><span class="chip">EV</span><span class="chip">Efficiency</span>
          </div>
        </div>
        <div class="article-source">
          <span>electrive</span><span>Aug 4, 2026</span>
          <a href="https://www.electrive.com/2026/08/04/audi-further-strips-a2-e-tron-of-its-camouflage/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">78</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/03/byd-opens-denza-z9s-pre-orders-record-1100-km-ev-range/" target="_blank" rel="noopener">BYD’s Denza Z9S touts 1,100 km range under $50k</a>
          <div class="article-take">Range headline cements BYD’s tech leadership in premium‑leaning trims.</div>
          <div class="article-tags">
            <span class="chip">BYD</span><span class="chip">Battery</span><span class="chip">China</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek</span><span>Aug 3, 2026</span>
          <a href="https://electrek.co/2026/08/03/byd-opens-denza-z9s-pre-orders-record-1100-km-ev-range/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="dealers">
    <h2 class="section-title">Dealers <span class="count">2</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip">68</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/new-models-vital-ds-survival-uk-sales-hit-record-low" target="_blank" rel="noopener">DS UK sales slump; new N°3 and N°7 models crucial</a>
          <div class="article-take">Showroom traffic and profitability hinge on a fast product pivot.</div>
          <div class="article-tags">
            <span class="chip">DS</span><span class="chip">Dealers</span><span class="chip">Sales</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar</span><span>Aug 4, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/new-models-vital-ds-survival-uk-sales-hit-record-low" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">66</div>
        <div class="article-main">
          <a class="headline" href="https://www.motor1.com/news/803722/costco-infiniti-discount/" target="_blank" rel="noopener">Costco offers new discounts on Infiniti SUVs</a>
          <div class="article-take">Big‑box partnerships continue to drive retail lead‑gen for dealers.</div>
          <div class="article-tags">
            <span class="chip">Retail</span><span class="chip">Infiniti</span><span class="chip">Incentives</span>
          </div>
        </div>
        <div class="article-source">
          <span>Motor1</span><span>Aug 3, 2026</span>
          <a href="https://www.motor1.com/news/803722/costco-infiniti-discount/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="suppliers">
    <h2 class="section-title">Suppliers <span class="count">3</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip high">84</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">SK On and Factorial align on solid‑state EV batteries</a>
          <div class="article-take">Consolidation around a manufacturable chemistry is accelerating.</div>
          <div class="article-tags">
            <span class="chip">Battery</span><span class="chip">SK On</span><span class="chip">Factorial</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek</span><span>Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">76</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/evgo-and-brixmor-to-add-more-than-500-fast-charging-stalls-in-the-us/" target="_blank" rel="noopener">EVgo + Brixmor to install 500+ fast chargers at shopping centers</a>
          <div class="article-take">Retail footprints are becoming anchor tenants for DCFC scale.</div>
          <div class="article-tags">
            <span class="chip">Charging</span><span class="chip">EVgo</span><span class="chip">Brixmor</span>
          </div>
        </div>
        <div class="article-source">
          <span>electrive</span><span>Aug 4, 2026</span>
          <a href="https://www.electrive.com/2026/08/04/evgo-and-brixmor-to-add-more-than-500-fast-charging-stalls-in-the-us/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">70</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/01/allego-commits-e100-million-to-expand-uk-charging-network/" target="_blank" rel="noopener">Allego commits €100M to expand UK ultra‑rapid charging</a>
          <div class="article-take">Capital flows continue into high‑traffic urban and corridor sites.</div>
          <div class="article-tags">
            <span class="chip">Allego</span><span class="chip">Charging</span><span class="chip">UK</span>
          </div>
        </div>
        <div class="article-source">
          <span>electrive</span><span>Aug 1, 2026</span>
          <a href="https://www.electrive.com/2026/08/01/allego-commits-e100-million-to-expand-uk-charging-network/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="government">
    <h2 class="section-title">Government <span class="count">3</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip high">92</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">NHTSA opens probe into 1.2M Teslas over suspension failures</a>
          <div class="article-take">A potential mass recall could reshape service operations and costs.</div>
          <div class="article-tags">
            <span class="chip">Safety</span><span class="chip">NHTSA</span><span class="chip">Tesla</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek</span><span>Jul 31, 2026</span>
          <a href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">75</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/denmark-evs-account-for-almost-all-new-car-registrations-in-july/" target="_blank" rel="noopener">Denmark: 97.6% EV share in July registrations</a>
          <div class="article-take">Policy alignment and accessible charging can push near‑total electrification.</div>
          <div class="article-tags">
            <span class="chip">Policy</span><span class="chip">Europe</span><span class="chip">EV adoption</span>
          </div>
        </div>
        <div class="article-source">
          <span>electrive</span><span>Aug 4, 2026</span>
          <a href="https://www.electrive.com/2026/08/04/denmark-evs-account-for-almost-all-new-car-registrations-in-july/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">73</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/philippines-launches-e850m-incentive-programme-for-ev-manufacturing/" target="_blank" rel="noopener">Philippines launches €850m EV manufacturing incentives</a>
          <div class="article-take">Southeast Asia’s policy race for EV supply chain wins intensifies.</div>
          <div class="article-tags">
            <span class="chip">Incentives</span><span class="chip">Manufacturing</span><span class="chip">Asia</span>
          </div>
        </div>
        <div class="article-source">
          <span>electrive</span><span>Aug 4, 2026</span>
          <a href="https://www.electrive.com/2026/08/04/philippines-launches-e850m-incentive-programme-for-ev-manufacturing/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="technology">
    <h2 class="section-title">Technology <span class="count">3</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip high">85</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Volvo exits lidar program on EX90/ES90, offers payouts</a>
          <div class="article-take">Shifting sensor strategy cuts complexity but raises perception debates.</div>
          <div class="article-tags">
            <span class="chip">Volvo</span><span class="chip">ADAS</span><span class="chip">Lidar</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek</span><span>Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">81</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/03/tesla-fsd-v14-lite-hw3-computer-failures/" target="_blank" rel="noopener">Reports of HW3 failures follow Tesla FSD v14 “Lite” rollout</a>
          <div class="article-take">Software heat loads can reveal latent hardware margin issues at scale.</div>
          <div class="article-tags">
            <span class="chip">Software</span><span class="chip">Tesla</span><span class="chip">Safety</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek</span><span>Aug 3, 2026</span>
          <a href="https://electrek.co/2026/08/03/tesla-fsd-v14-lite-hw3-computer-failures/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">79</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/waymo-gemini-ai-ojai-robotaxi-redesigned-interface/" target="_blank" rel="noopener">Waymo adds Gemini AI and new rider interface</a>
          <div class="article-take">User experience and trust are becoming as critical as AV miles.</div>
          <div class="article-tags">
            <span class="chip">AI</span><span class="chip">Autonomous</span><span class="chip">UX</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek</span><span>Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/waymo-gemini-ai-ojai-robotaxi-redesigned-interface/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="finance">
    <h2 class="section-title">Finance <span class="count">3</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip high">84</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/30/rivian-rivn-q2-2026-earnings-r2-deliveries-revenue-up-27/" target="_blank" rel="noopener">Rivian beats on revenue, prints record gross profit</a>
          <div class="article-take">Operational leverage is improving as new product ramps.</div>
          <div class="article-tags">
            <span class="chip">Earnings</span><span class="chip">Rivian</span><span class="chip">Margins</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek</span><span>Jul 30, 2026</span>
          <a href="https://electrek.co/2026/07/30/rivian-rivn-q2-2026-earnings-r2-deliveries-revenue-up-27/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">80</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/04/tesla-china-sales-crash-exports-surge-h1-2026/" target="_blank" rel="noopener">Tesla China unit: inland sales down, exports up 127%</a>
          <div class="article-take">Mix shift preserves factory load but pressures margins and logistics.</div>
          <div class="article-tags">
            <span class="chip">Tesla</span><span class="chip">China</span><span class="chip">Exports</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek</span><span>Aug 4, 2026</span>
          <a href="https://electrek.co/2026/08/04/tesla-china-sales-crash-exports-surge-h1-2026/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">78</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/03/byd-boosts-sales-by-22-in-july/" target="_blank" rel="noopener">BYD sales rise 22% in July, exports at record share</a>
          <div class="article-take">Overseas momentum offsets softness in the domestic market.</div>
          <div class="article-tags">
            <span class="chip">BYD</span><span class="chip">Sales</span><span class="chip">Exports</span>
          </div>
        </div>
        <div class="article-source">
          <span>electrive</span><span>Aug 3, 2026</span>
          <a href="https://www.electrive.com/2026/08/03/byd-boosts-sales-by-22-in-july/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="international">
    <h2 class="section-title">International <span class="count">3</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip">78</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/28/baidu-apollo-go-london-robotaxi-testing-uber-lyft/" target="_blank" rel="noopener">Baidu Apollo Go starts road testing in London</a>
          <div class="article-take">China’s AV champions are testing the waters in Europe’s capitals.</div>
          <div class="article-tags">
            <span class="chip">Autonomous</span><span class="chip">London</span><span class="chip">Mobility</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek</span><span>Jul 28, 2026</span>
          <a href="https://electrek.co/2026/07/28/baidu-apollo-go-london-robotaxi-testing-uber-lyft/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">75</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/denmark-evs-account-for-almost-all-new-car-registrations-in-july/" target="_blank" rel="noopener">Denmark nears 100% EV share in monthly registrations</a>
          <div class="article-take">Policy clarity and product breadth continue to show compounding effects.</div>
          <div class="article-tags">
            <span class="chip">Europe</span><span class="chip">EV adoption</span><span class="chip">Policy</span>
          </div>
        </div>
        <div class="article-source">
          <span>electrive</span><span>Aug 4, 2026</span>
          <a href="https://www.electrive.com/2026/08/04/denmark-evs-account-for-almost-all-new-car-registrations-in-july/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">74</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/28/volkswagen-launches-cheaper-id-polo-ev-orders-25000/" target="_blank" rel="noopener">Volkswagen opens pre‑orders for entry ID. Polo EV in UK</a>
          <div class="article-take">Lower price points broaden EV access in Europe’s B‑segment.</div>
          <div class="article-tags">
            <span class="chip">UK</span><span class="chip">Volkswagen</span><span class="chip">EV</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek</span><span>Jul 28, 2026</span>
          <a href="https://electrek.co/2026/07/28/volkswagen-launches-cheaper-id-polo-ev-orders-25000/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="opinion">
    <h2 class="section-title">Opinion <span class="count">2</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip">70</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/business-manufacturing/chinese-car-makers-all-share-parts-will-world-follow" target="_blank" rel="noopener">Chinese car makers share parts—will the world follow?</a>
          <div class="article-take">Standardized components slash costs and lead times, challenging Western norms.</div>
          <div class="article-tags">
            <span class="chip">Supply Chain</span><span class="chip">China</span><span class="chip">Strategy</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar</span><span>Aug 4, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/business-manufacturing/chinese-car-makers-all-share-parts-will-world-follow" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">64</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/opinion/new-cars/ignore-jay-leno-your-dream-garage-only-needs-three-cars" target="_blank" rel="noopener">Ignore Jay Leno: your dream garage only needs three cars</a>
          <div class="article-take">A minimalist’s case for maximizing driving joy and practicality.</div>
          <div class="article-tags">
            <span class="chip">Opinion</span><span class="chip">Culture</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar</span><span>Aug 3, 2026</span>
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