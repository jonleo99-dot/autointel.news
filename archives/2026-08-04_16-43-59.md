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
    <span class="ticker-item"><b>Tesla</b> NHTSA probe <span class="ticker-down">▼</span></span>
    <span class="ticker-item"><b>Mercedes-Benz</b> GLA EV launch <span class="ticker-up">▲</span></span>
    <span class="ticker-item"><b>Hyundai</b> IONIQ 3 demand <span class="ticker-up">▲</span></span>
    <span class="ticker-item"><b>BMW</b> product review <span class="ticker-flat">■</span></span>
    <span class="ticker-item"><b>Waymo</b> Gemini UI <span class="ticker-up">▲</span></span>
    <span class="ticker-item"><b>BYD</b> 1,100 km claim <span class="ticker-up">▲</span></span>
    <span class="ticker-item"><b>Volvo</b> drops lidar <span class="ticker-down">▼</span></span>
    <span class="ticker-item"><b>Rivian</b> revenue up <span class="ticker-up">▲</span></span>
    <span class="ticker-item"><b>Audi</b> Q9 flagship <span class="ticker-up">▲</span></span>
    <span class="ticker-item"><b>Philippines</b> EV incentives <span class="ticker-up">▲</span></span>
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
        <h1>NHTSA opens probe into 1.2M Teslas over front‑suspension failures</h1>
        <p class="exec-summary">US regulators launched a preliminary investigation into 2018–2020 Model 3 and 2021–2023 Model Y vehicles after 150+ complaints of lower control‑arm separations while driving. The probe zeroes in on the front lower lateral link detaching, a failure mode that can sharply compromise steering control. For Tesla, the timing collides with ongoing cost and quality resets and expanding exports from Shanghai. For the industry, it’s a reminder that aggressive time‑to‑market and supplier turmoil can boomerang into expensive rework, warranty hits, and brand risk when component margins are shaved too thin.</p>

        <div class="takeaways">
          <h3>Key Takeaways</h3>
          <ul>
            
          </ul>
        </div>

        <div class="impact-row">
          <div class="impact-block">
            <h4>Industry Impact</h4>
            <p>Potential outcomes range from an engineering service campaign to a full recall. Either path would elevate supply risk for chassis components, push warranty reserves higher across EV programs, and could invite broader scrutiny of lightweight suspension designs used to chase range. Dealers should prepare for inspection volume surges and educate owners about warning signs (steering noise/feel) while OEMs reassess validation gates for fast‑cycle platforms.</p>
          </div>
          <div class="impact-block">
            <h4>Companies Affected</h4>
            <div class="chip-row">
              <span class="chip entity-mfr">Tesla</span>
              <span class="chip entity-mfr">NHTSA</span>
              <span class="chip">Model 3</span>
              <span class="chip">Model Y</span>
              <span class="chip">Suspension Suppliers</span>
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
            <li><a href="https://electrek.co/2026/07/28/tesla-sues-cybertruck-supplier-angstrom-tooling/" target="_blank" rel="noopener">Tesla sues Cybertruck supplier amid tooling standoff</a></li>
            <li><a href="https://www.electrive.com/2026/07/31/tesla-tops-10-million-electric-vehicles-built/" target="_blank" rel="noopener">Tesla tops 10 million EVs produced</a></li>
            <li><a href="https://electrek.co/2026/08/04/tesla-china-sales-crash-exports-surge-h1-2026/" target="_blank" rel="noopener">Tesla China sales fall as exports surge</a></li>
          </ul>
        </div>
      </div>

      <div class="hero-gauges">
        <div class="gauge">
          <svg viewBox="0 0 120 70"><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#2a3038" stroke-width="8"/><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#f2a93b" stroke-width="8" stroke-dasharray="157" stroke-dashoffset="12.9"/></svg>
          <span class="gauge-value mono">92</span>
          <span class="gauge-label">Importance</span>
        </div>
        <div class="gauge">
          <svg viewBox="0 0 120 70"><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#2a3038" stroke-width="8"/><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#3ecf8e" stroke-width="8" stroke-dasharray="157" stroke-dashoffset="18.8"/></svg>
          <span class="gauge-value mono">88</span>
          <span class="gauge-label">Editorial Quality</span>
        </div>
        <div class="gauge">
          <svg viewBox="0 0 120 70"><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#2a3038" stroke-width="8"/><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#e2604f" stroke-width="8" stroke-dasharray="157" stroke-dashoffset="23.6"/></svg>
          <span class="gauge-value mono">85</span>
          <span class="gauge-label">Industry Impact</span>
        </div>
        <div class="gauge">
          <svg viewBox="0 0 120 70"><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#2a3038" stroke-width="8"/><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#f2a93b" stroke-width="8" stroke-dasharray="157" stroke-dashoffset="26.7"/></svg>
          <span class="gauge-value mono">83</span>
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
    <h2 class="section-title">Industry Snapshot <span class="count">Last 7 days • through Aug 4, 2026</span></h2>
    <div class="dash-grid">
      
      <div class="stat-panel">
        <h4>OEMs by headline momentum</h4>
        <ul class="rank-list">
          <li><span>Tesla</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:100%"></span></span><span class="rank-count">18</span></li>
          <li><span>Mercedes‑Benz</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:78%"></span></span><span class="rank-count">14</span></li>
          <li><span>BMW</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:61%"></span></span><span class="rank-count">11</span></li>
          <li><span>BYD</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:56%"></span></span><span class="rank-count">10</span></li>
          <li><span>Hyundai/Kia</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:50%"></span></span><span class="rank-count">9</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4>Regulatory & safety themes</h4>
        <ul class="rank-list">
          <li><span>NHTSA investigations/recalls</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:100%"></span></span><span class="rank-count">5</span></li>
          <li><span>Incentives & grants</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:60%"></span></span><span class="rank-count">3</span></li>
          <li><span>Charging policy & rollouts</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:80%"></span></span><span class="rank-count">4</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4>Technology signals</h4>
        <div class="tagcloud">
          <span class="chip lg">Solid‑state batteries</span>
          <span class="chip">Lidar strategy</span>
          <span class="chip">AI in HMI</span>
          <span class="chip">Fast charging (seconds)</span>
          <span class="chip">Safety compute</span>
          <span class="chip">Long‑range chemistries</span>
          <span class="chip">V2L/VPP</span>
        </div>
      </div>

      <div class="stat-panel">
        <h4>Retail & demand cues</h4>
        <ul class="rank-list">
          <li><span>Affordable EV launches</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:90%"></span></span><span class="rank-count">7</span></li>
          <li><span>Hybrid mix gains</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:70%"></span></span><span class="rank-count">5</span></li>
          <li><span>Premium EV sell‑outs</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:50%"></span></span><span class="rank-count">4</span></li>
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
        <a href="https://www.autocar.co.uk/car-news/electric-cars/new-mercedes-gla-revealed-audi-q4-rival-408-mile-range" target="_blank" rel="noopener">Mercedes reveals new GLA EV with up to 408‑mile range</a>
        <div class="fp-meta"><span>Score 80</span><span>•</span><span>Autocar</span><span>•</span><span>Aug 4</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.autocar.co.uk/car-news/new-cars/audi-q9-suv-revealed-huge-%C2%A3100k-a8-successor" target="_blank" rel="noopener">Audi debuts Q9 flagship SUV as A8 successor</a>
        <div class="fp-meta"><span>Score 78</span><span>•</span><span>Autocar</span><span>•</span><span>Aug 4</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/28/bmw-ramps-up-ix3-output-orders-near-100000/" target="_blank" rel="noopener">BMW ramps iX3 output as orders near 100k</a>
        <div class="fp-meta"><span>Score 72</span><span>•</span><span>Electrek</span><span>•</span><span>Aug 3</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/08/03/volvos-next-electric-suv-will-start-in-the-upper-40000-range/" target="_blank" rel="noopener">Volvo’s next electric SUV to start under $50k</a>
        <div class="fp-meta"><span>Score 70</span><span>•</span><span>Electrek</span><span>•</span><span>Aug 4</span></div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Technology</h3>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">SK On and Factorial ally to scale solid‑state batteries</a>
        <div class="fp-meta"><span>Score 76</span><span>•</span><span>Electrek</span><span>•</span><span>Jul 29</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/waymo-gemini-ai-ojai-robotaxi-redesigned-interface/" target="_blank" rel="noopener">Waymo integrates Gemini AI and new rider UI</a>
        <div class="fp-meta"><span>Score 75</span><span>•</span><span>Electrek</span><span>•</span><span>Jul 29</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Volvo drops lidar on EX90/ES90, compensates owners</a>
        <div class="fp-meta"><span>Score 82</span><span>•</span><span>Electrek</span><span>•</span><span>Jul 29</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.greencarreports.com/news/1146039_ev-battery-recycling-breakthrough-recovers-99-99-of-lithium" target="_blank" rel="noopener">Researchers claim 99.99% lithium recovery in recycling</a>
        <div class="fp-meta"><span>Score 68</span><span>•</span><span>Green Car Reports</span><span>•</span><span>Aug 3</span></div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Government & Regulation</h3>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">NHTSA probes 1.2M Teslas over suspension failures</a>
        <div class="fp-meta"><span>Score 92</span><span>•</span><span>Electrek</span><span>•</span><span>Jul 31</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.electrive.com/2026/08/04/philippines-launches-e850m-incentive-programme-for-ev-manufacturing/" target="_blank" rel="noopener">Philippines unveils €850m EV manufacturing incentives</a>
        <div class="fp-meta"><span>Score 71</span><span>•</span><span>Electrive</span><span>•</span><span>Aug 4</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.electrive.com/2026/08/03/devon-and-torbay-commission-nearly-3000-public-ev-charging-points/" target="_blank" rel="noopener">Devon & Torbay commission ~3,000 public chargers</a>
        <div class="fp-meta"><span>Score 69</span><span>•</span><span>Electrive</span><span>•</span><span>Aug 3</span></div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Suppliers & Infrastructure</h3>
      <div class="fp-row">
        <a href="https://chargedevs.com/newswire/beam-global-supplies-ev-arc-off-grid-charging-systems-for-dallas-municipal-fleet-and-massachusetts-carshare-pilot/" target="_blank" rel="noopener">Beam Global delivers off‑grid EV ARC systems</a>
        <div class="fp-meta"><span>Score 66</span><span>•</span><span>Charged</span><span>•</span><span>Aug 1</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.electrive.com/2026/08/04/evgo-and-brixmor-to-add-more-than-500-fast-charging-stalls-in-the-us/" target="_blank" rel="noopener">EVgo, Brixmor to add 500+ DC fast stalls</a>
        <div class="fp-meta"><span>Score 70</span><span>•</span><span>Electrive</span><span>•</span><span>Aug 4</span></div>
      </div>
      <div class="fp-row">
        <a href="https://chargedevs.com/newswire/mahle-introduces-a-new-range-extender-engine-and-a-rare-earth-free-electric-motor/" target="_blank" rel="noopener">MAHLE debuts truck range‑extender and rare‑earth‑free motor</a>
        <div class="fp-meta"><span>Score 64</span><span>•</span><span>Charged</span><span>•</span><span>Aug 3</span></div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Trending Topics</h3>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/30/tesla-10-millionth-vehicle-ev-growth-stalled/" target="_blank" rel="noopener">Tesla hits 10M EVs as growth stalls vs capacity</a>
        <div class="fp-meta"><span>Score 73</span><span>•</span><span>Electrek</span><span>•</span><span>Jul 30</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.caranddriver.com/news/a73317897/california-registrations-hybrids-evs-2026/" target="_blank" rel="noopener">California registers more hybrids than EVs in H1</a>
        <div class="fp-meta"><span>Score 67</span><span>•</span><span>Car and Driver</span><span>•</span><span>Aug 1</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/27/rivian-r2-tesla-model-y-real-world-efficiency-test/" target="_blank" rel="noopener">Real‑world test: Rivian R2 uses more energy than Model Y</a>
        <div class="fp-meta"><span>Score 69</span><span>•</span><span>Electrek</span><span>•</span><span>Jul 27</span></div>
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
        <div class="score-chip high">92</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">NHTSA opens probe into 1.2M Teslas over suspension failures</a>
          <div class="article-take">Safety scrutiny on a high‑volume EV platform could translate into costly rework and broad supplier ripples.</div>
          <div class="article-tags">
            <span class="chip">Tesla</span><span class="chip">NHTSA</span><span class="chip">Quality</span><span class="chip">Recall risk</span>
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
          <a class="headline" href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Volvo drops lidar on EX90/ES90 and compensates owners</a>
          <div class="article-take">Backing away from lidar trims cost and complexity but raises questions on long‑term ADAS roadmaps.</div>
          <div class="article-tags">
            <span class="chip">Volvo</span><span class="chip">ADAS</span><span class="chip">Lidar</span><span class="chip">Cost</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">80</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/electric-cars/new-mercedes-gla-revealed-audi-q4-rival-408-mile-range" target="_blank" rel="noopener">New Mercedes GLA revealed with up to 408‑mile EV range</a>
          <div class="article-take">Mercedes pushes compact EV efficiency and charging speed to defend premium C‑SUV share.</div>
          <div class="article-tags">
            <span class="chip">Mercedes‑Benz</span><span class="chip">GLA EV</span><span class="chip">Launch</span><span class="chip">Compact SUV</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 4, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/electric-cars/new-mercedes-gla-revealed-audi-q4-rival-408-mile-range" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">78</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/audi-q9-suv-revealed-huge-%C2%A3100k-a8-successor" target="_blank" rel="noopener">Audi Q9 revealed as “unapologetically high‑status” SUV</a>
          <div class="article-take">Audi doubles down on profit‑rich full‑size SUVs to offset EV transition costs.</div>
          <div class="article-tags">
            <span class="chip">Audi</span><span class="chip">Q9</span><span class="chip">Luxury SUV</span><span class="chip">Profit mix</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 4, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/audi-q9-suv-revealed-huge-%C2%A3100k-a8-successor" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">77</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/hyundai-reveals-ioniq-3-prices-start-30000-interest-surges/" target="_blank" rel="noopener">Hyundai IONIQ 3 pricing around $30k as interest surges</a>
          <div class="article-take">Affordable range and fresh UX give Hyundai a high‑volume EV foothold with mainstream buyers.</div>
          <div class="article-tags">
            <span class="chip">Hyundai</span><span class="chip">IONIQ 3</span><span class="chip">Pricing</span><span class="chip">Demand</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/hyundai-reveals-ioniq-3-prices-start-30000-interest-surges/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">76</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">SK On and Factorial join forces to scale solid‑state</a>
          <div class="article-take">Partnerships are consolidating the path to pilot lines and early‑decade production commitments.</div>
          <div class="article-tags">
            <span class="chip">SK On</span><span class="chip">Factorial</span><span class="chip">Solid‑state</span><span class="chip">Batteries</span>
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
          <a class="headline" href="https://electrek.co/2026/07/29/waymo-gemini-ai-ojai-robotaxi-redesigned-interface/" target="_blank" rel="noopener">Waymo adds Gemini AI assistant and new rider interface</a>
          <div class="article-take">Human‑machine experience becomes a competitive moat as AV services scale beyond pilots.</div>
          <div class="article-tags">
            <span class="chip">Waymo</span><span class="chip">Autonomy</span><span class="chip">AI UX</span><span class="chip">Robotaxi</span>
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
          <a class="headline" href="https://electrek.co/2026/07/30/tesla-10-millionth-vehicle-ev-growth-stalled/" target="_blank" rel="noopener">Tesla builds 10 millionth vehicle as growth lags capacity</a>
          <div class="article-take">Scale milestone collides with utilization pressure, pushing margin defense and new product timing.</div>
          <div class="article-tags">
            <span class="chip">Tesla</span><span class="chip">Production</span><span class="chip">Capacity</span><span class="chip">Margins</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 30, 2026</span>
          <a href="https://electrek.co/2026/07/30/tesla-10-millionth-vehicle-ev-growth-stalled/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">72</div>
        <div class="article-main">
          <a class="headline" href="https://www.greencarreports.com/news/1146051_gm-pilot-ev-charging-network-now-spans-over-25-states" target="_blank" rel="noopener">GM‑Pilot EVgo highway charging now in 25+ states</a>
          <div class="article-take">Ultrafast coverage at travel centers anchors road‑trip confidence as NACS transition accelerates.</div>
          <div class="article-tags">
            <span class="chip">GM</span><span class="chip">EVgo</span><span class="chip">Charging</span><span class="chip">Network</span>
          </div>
        </div>
        <div class="article-source">
          <span>Green Car Reports — Aug 2, 2026</span>
          <a href="https://www.greencarreports.com/news/1146051_gm-pilot-ev-charging-network-now-spans-over-25-states" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">71</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/philippines-launches-e850m-incentive-programme-for-ev-manufacturing/" target="_blank" rel="noopener">Philippines launches €850m EV manufacturing incentive</a>
          <div class="article-take">New money targets assembly and parts localization to pull supply chains beyond China.</div>
          <div class="article-tags">
            <span class="chip">Philippines</span><span class="chip">Incentives</span><span class="chip">Manufacturing</span><span class="chip">Supply chain</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrive — Aug 4, 2026</span>
          <a href="https://www.electrive.com/2026/08/04/philippines-launches-e850m-incentive-programme-for-ev-manufacturing/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">70</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/ferrari-luce-ev-sold-out-2026-allocation/" target="_blank" rel="noopener">Ferrari’s $640k Luce EV sells out 2026 allocation</a>
          <div class="article-take">Ultra‑luxury demand remains price‑inelastic, signaling headroom for halo EV pricing.</div>
          <div class="article-tags">
            <span class="chip">Ferrari</span><span class="chip">EV</span><span class="chip">Demand</span><span class="chip">Luxury</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/ferrari-luce-ev-sold-out-2026-allocation/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">69</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/27/rivian-r2-tesla-model-y-real-world-efficiency-test/" target="_blank" rel="noopener">Test: Rivian R2 uses more energy than Model Y at every speed</a>
          <div class="article-take">EPA parity masks aero and rolling‑loss penalties that show up in real‑world highway use.</div>
          <div class="article-tags">
            <span class="chip">Rivian</span><span class="chip">Tesla</span><span class="chip">Efficiency</span><span class="chip">Range</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 27, 2026</span>
          <a href="https://electrek.co/2026/07/27/rivian-r2-tesla-model-y-real-world-efficiency-test/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">69</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/03/devon-and-torbay-commission-nearly-3000-public-ev-charging-points/" target="_blank" rel="noopener">Devon & Torbay commission nearly 3,000 public EV chargers</a>
          <div class="article-take">Local LEVI capital plus private funds accelerate UK’s curbside and destination coverage.</div>
          <div class="article-tags">
            <span class="chip">UK</span><span class="chip">Charging</span><span class="chip">Infrastructure</span><span class="chip">LEVI</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrive — Aug 3, 2026</span>
          <a href="https://www.electrive.com/2026/08/03/devon-and-torbay-commission-nearly-3000-public-ev-charging-points/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">68</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/07/31/volkswagen-opens-uk-order-books-for-the-id-polo/" target="_blank" rel="noopener">Volkswagen opens UK orders for sub‑£24k ID. Polo</a>
          <div class="article-take">Entry EV pricing inches lower, pressuring value brands to respond on spec and finance.</div>
          <div class="article-tags">
            <span class="chip">Volkswagen</span><span class="chip">ID. Polo</span><span class="chip">Pricing</span><span class="chip">UK</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrive — Jul 31, 2026</span>
          <a href="https://www.electrive.com/2026/07/31/volkswagen-opens-uk-order-books-for-the-id-polo/" target="_blank" rel="noopener">Read original →</a>
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
    <h2 class="section-title">Industry News <span class="count">4 stories</span></h2>
    <div class="article-table">
      
      <div class="article-row">
        <div class="score-chip high">92</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">NHTSA opens probe into 1.2M Teslas over suspension failures</a>
          <div class="article-take">A potential recall could reshape warranty reserves and validation standards across fast‑cycle EVs.</div>
          <div class="article-tags"><span class="chip">Regulation</span><span class="chip">Tesla</span><span class="chip">Safety</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 31, 2026</span>
          <a href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">79</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">BMW rethinks product plan; G‑Class rival put on hold</a>
          <div class="article-take">Shifting demand and China headwinds force tighter capital targeting on future nameplates.</div>
          <div class="article-tags"><span class="chip">BMW</span><span class="chip">Strategy</span><span class="chip">Portfolio</span></div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 4, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">73</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/30/tesla-10-millionth-vehicle-ev-growth-stalled/" target="_blank" rel="noopener">Tesla hits 10M EVs but runs below installed capacity</a>
          <div class="article-take">Scale brings leverage—until it doesn’t; product cadence and pricing discipline become decisive.</div>
          <div class="article-tags"><span class="chip">Tesla</span><span class="chip">Production</span><span class="chip">Utilization</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 30, 2026</span>
          <a href="https://electrek.co/2026/07/30/tesla-10-millionth-vehicle-ev-growth-stalled/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      
      <div class="article-row">
        <div class="score-chip">67</div>
        <div class="article-main">
          <a class="headline" href="https://www.caranddriver.com/news/a73317897/california-registrations-hybrids-evs-2026/" target="_blank" rel="noopener">California buys more hybrids than EVs in H1 2026</a>
          <div class="article-take">Powertrain pragmatism persists; expect hybrid‑heavy trims to anchor showroom traffic.</div>
          <div class="article-tags"><span class="chip">Hybrids</span><span class="chip">Demand</span><span class="chip">Mix</span></div>
        </div>
        <div class="article-source">
          <span>Car and Driver — Aug 1, 2026</span>
          <a href="https://www.caranddriver.com/news/a73317897/california-registrations-hybrids-evs-2026/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

    </div>
  </div>

  <div class="sec-group reveal" id="electric-vehicles">
    <h2 class="section-title">Electric Vehicles <span class="count">4 stories</span></h2>
    <div class="article-table">

      <div class="article-row">
        <div class="score-chip">80</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/electric-cars/new-mercedes-gla-revealed-audi-q4-rival-408-mile-range" target="_blank" rel="noopener">Mercedes GLA EV debuts with long range and 320kW charging</a>
          <div class="article-take">Luxury compacts lean on efficiency and charging speed to widen appeal beyond early adopters.</div>
          <div class="article-tags"><span class="chip">Mercedes‑Benz</span><span class="chip">GLA</span><span class="chip">Launch</span></div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 4, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/electric-cars/new-mercedes-gla-revealed-audi-q4-rival-408-mile-range" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      
      <div class="article-row">
        <div class="score-chip">77</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/hyundai-reveals-ioniq-3-prices-start-30000-interest-surges/" target="_blank" rel="noopener">IONIQ 3 hits $30k price point with 300+ miles of range</a>
          <div class="article-take">Price‑spec balance is set to pull fence‑sitters into EV consideration lists.</div>
          <div class="article-tags"><span class="chip">Hyundai</span><span class="chip">IONIQ 3</span><span class="chip">Value EV</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/hyundai-reveals-ioniq-3-prices-start-30000-interest-surges/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      
      <div class="article-row">
        <div class="score-chip">68</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/07/31/volkswagen-opens-uk-order-books-for-the-id-polo/" target="_blank" rel="noopener">Volkswagen opens orders for budget ID. Polo in UK</a>
          <div class="article-take">Mainstream EVs creep below £24k MSRP, pressuring used‑ICE economics.</div>
          <div class="article-tags"><span class="chip">Volkswagen</span><span class="chip">ID. Polo</span><span class="chip">UK Market</span></div>
        </div>
        <div class="article-source">
          <span>Electrive — Jul 31, 2026</span>
          <a href="https://www.electrive.com/2026/07/31/volkswagen-opens-uk-order-books-for-the-id-polo/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      
      <div class="article-row">
        <div class="score-chip">70</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/ferrari-luce-ev-sold-out-2026-allocation/" target="_blank" rel="noopener">Ferrari’s Luce EV sells out 2026 in under two months</a>
          <div class="article-take">Proof that brand equity can outrun EV price resistance at the top of the market.</div>
          <div class="article-tags"><span class="chip">Ferrari</span><span class="chip">EV</span><span class="chip">Demand</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/ferrari-luce-ev-sold-out-2026-allocation/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

    </div>
  </div>

  <div class="sec-group reveal" id="manufacturers">
    <h2 class="section-title">Manufacturers <span class="count">3 stories</span></h2>
    <div class="article-table">
      
      <div class="article-row">
        <div class="score-chip">78</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/audi-q9-suv-revealed-huge-%C2%A3100k-a8-successor" target="_blank" rel="noopener">Audi Q9 targets US and Middle East luxury SUV buyers</a>
          <div class="article-take">Bigger body, bigger margins—Audi leans on SUVs to bankroll EV pivots.</div>
          <div class="article-tags"><span class="chip">Audi</span><span class="chip">Q9</span><span class="chip">Luxury</span></div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 4, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/audi-q9-suv-revealed-huge-%C2%A3100k-a8-successor" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      
      <div class="article-row">
        <div class="score-chip">72</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/28/bmw-ramps-up-ix3-output-orders-near-100000/" target="_blank" rel="noopener">BMW boosts iX3 output as orders approach 100k</a>
          <div class="article-take">A fast ramp in Hungary underlines BMW’s modular plant playbook for EVs.</div>
          <div class="article-tags"><span class="chip">BMW</span><span class="chip">iX3</span><span class="chip">Production</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 28, 2026</span>
          <a href="https://electrek.co/2026/07/28/bmw-ramps-up-ix3-output-orders-near-100000/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      

      <div class="article-row">
        <div class="score-chip">70</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/03/volvos-next-electric-suv-will-start-in-the-upper-40000-range/" target="_blank" rel="noopener">Volvo aims sub‑$50k entry with upcoming EX50</a>
          <div class="article-take">Competitive MSRP targets Model Y shoppers with Scandinavian UX and safety cred.</div>
          <div class="article-tags"><span class="chip">Volvo</span><span class="chip">Pricing</span><span class="chip">EX50</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 3, 2026</span>
          <a href="https://electrek.co/2026/08/03/volvos-next-electric-suv-will-start-in-the-upper-40000-range/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

    </div>
  </div>

  <div class="sec-group reveal" id="dealers">
    <h2 class="section-title">Dealers <span class="count">2 stories</span></h2>
    <div class="article-table">

      <div class="article-row">
        <div class="score-chip">69</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/03/devon-and-torbay-commission-nearly-3000-public-ev-charging-points/" target="_blank" rel="noopener">Devon & Torbay greenlight nearly 3,000 public chargers</a>
          <div class="article-take">More local plugs reduce test‑drive friction and improve EV readiness around showrooms.</div>
          <div class="article-tags"><span class="chip">Dealers</span><span class="chip">Charging</span><span class="chip">UK</span></div>
        </div>
        <div class="article-source">
          <span>Electrive — Aug 3, 2026</span>
          <a href="https://www.electrive.com/2026/08/03/devon-and-torbay-commission-nearly-3000-public-ev-charging-points/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      

      <div class="article-row">
        <div class="score-chip">67</div>
        <div class="article-main">
          <a class="headline" href="https://www.caranddriver.com/news/a73317897/california-registrations-hybrids-evs-2026/" target="_blank" rel="noopener">Hybrids outpace EVs in California registrations</a>
          <div class="article-take">Stores should recalibrate inventory and F&I for hybrid demand surges.</div>
          <div class="article-tags"><span class="chip">Retail</span><span class="chip">Hybrids</span><span class="chip">Mix</span></div>
        </div>
        <div class="article-source">
          <span>Car and Driver — Aug 1, 2026</span>
          <a href="https://www.caranddriver.com/news/a73317897/california-registrations-hybrids-evs-2026/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

    </div>
  </div>

  <div class="sec-group reveal" id="suppliers">
    <h2 class="section-title">Suppliers <span class="count">3 stories</span></h2>
    <div class="article-table">

      <div class="article-row">
        <div class="score-chip">70</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/evgo-and-brixmor-to-add-more-than-500-fast-charging-stalls-in-the-us/" target="_blank" rel="noopener">EVgo and Brixmor add 500+ fast chargers at shopping centers</a>
          <div class="article-take">Retail real estate becomes charging real estate—anchoring dwell‑time monetization.</div>
          <div class="article-tags"><span class="chip">EVgo</span><span class="chip">Retail</span><span class="chip">DC Fast</span></div>
        </div>
        <div class="article-source">
          <span>Electrive — Aug 4, 2026</span>
          <a href="https://www.electrive.com/2026/08/04/evgo-and-brixmor-to-add-more-than-500-fast-charging-stalls-in-the-us/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      
      <div class="article-row">
        <div class="score-chip">66</div>
        <div class="article-main">
          <a class="headline" href="https://chargedevs.com/newswire/beam-global-supplies-ev-arc-off-grid-charging-systems-for-dallas-municipal-fleet-and-massachusetts-carshare-pilot/" target="_blank" rel="noopener">Beam Global supplies off‑grid EV ARC systems for fleets</a>
          <div class="article-take">No‑trench deployments keep municipal electrification projects on schedule.</div>
          <div class="article-tags"><span class="chip">Beam Global</span><span class="chip">Fleets</span><span class="chip">Off‑grid</span></div>
        </div>
        <div class="article-source">
          <span>Charged — Aug 1, 2026</span>
          <a href="https://chargedevs.com/newswire/beam-global-supplies-ev-arc-off-grid-charging-systems-for-dallas-municipal-fleet-and-massachusetts-carshare-pilot/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      

      <div class="article-row">
        <div class="score-chip">64</div>
        <div class="article-main">
          <a class="headline" href="https://chargedevs.com/newswire/mahle-introduces-a-new-range-extender-engine-and-a-rare-earth-free-electric-motor/" target="_blank" rel="noopener">MAHLE reveals truck range‑extender and rare‑earth‑free e‑motor</a>
          <div class="article-take">Bridging tech targets uptime and cost while de‑risking magnet supply chains.</div>
          <div class="article-tags"><span class="chip">MAHLE</span><span class="chip">Powertrain</span><span class="chip">Supply chain</span></div>
        </div>
        <div class="article-source">
          <span>Charged — Aug 3, 2026</span>
          <a href="https://chargedevs.com/newswire/mahle-introduces-a-new-range-extender-engine-and-a-rare-earth-free-electric-motor/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

    </div>
  </div>

  <div class="sec-group reveal" id="government">
    <h2 class="section-title">Government <span class="count">3 stories</span></h2>
    <div class="article-table">

      <div class="article-row">
        <div class="score-chip high">92</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">US safety probe targets Tesla front suspension failures</a>
          <div class="article-take">Potential recall could trigger cross‑program audits of similar control‑arm designs.</div>
          <div class="article-tags"><span class="chip">NHTSA</span><span class="chip">Tesla</span><span class="chip">Safety</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 31, 2026</span>
          <a href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      

      <div class="article-row">
        <div class="score-chip">71</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/philippines-launches-e850m-incentive-programme-for-ev-manufacturing/" target="_blank" rel="noopener">Philippines announces €850m EV manufacturing plan</a>
          <div class="article-take">A new hub for ASEAN EV assembly is taking shape with fresh state support.</div>
          <div class="article-tags"><span class="chip">Policy</span><span class="chip">Manufacturing</span><span class="chip">APAC</span></div>
        </div>
        <div class="article-source">
          <span>Electrive — Aug 4, 2026</span>
          <a href="https://www.electrive.com/2026/08/04/philippines-launches-e850m-incentive-programme-for-ev-manufacturing/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      

      <div class="article-row">
        <div class="score-chip">69</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/03/devon-and-torbay-commission-nearly-3000-public-ev-charging-points/" target="_blank" rel="noopener">UK councils commission nearly 3,000 public charge points</a>
          <div class="article-take">Public‑private models accelerate rollout where curbside access is critical.</div>
          <div class="article-tags"><span class="chip">UK</span><span class="chip">Charging</span><span class="chip">Policy</span></div>
        </div>
        <div class="article-source">
          <span>Electrive — Aug 3, 2026</span>
          <a href="https://www.electrive.com/2026/08/03/devon-and-torbay-commission-nearly-3000-public-ev-charging-points/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

    </div>
  </div>

  <div class="sec-group reveal" id="technology">
    <h2 class="section-title">Technology <span class="count">3 stories</span></h2>
    <div class="article-table">

      <div class="article-row">
        <div class="score-chip">82</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Volvo ditches lidar on EX90/ES90 and pays out to buyers</a>
          <div class="article-take">Automated‑safety roadmaps are normalizing around vision‑centric stacks to cut BOM cost.</div>
          <div class="article-tags"><span class="chip">Volvo</span><span class="chip">ADAS</span><span class="chip">Lidar</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      

      <div class="article-row">
        <div class="score-chip">76</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">SK On, Factorial team to speed solid‑state to market</a>
          <div class="article-take">Alliances are the shortcut from lab cells to qualified automotive packs.</div>
          <div class="article-tags"><span class="chip">Batteries</span><span class="chip">Solid‑state</span><span class="chip">Partnerships</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      

      <div class="article-row">
        <div class="score-chip">75</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/waymo-gemini-ai-ojai-robotaxi-redesigned-interface/" target="_blank" rel="noopener">Waymo integrates Gemini assistant and revamped rider UI</a>
          <div class="article-take">Service differentiation shifts from pure autonomy to the total ride experience.</div>
          <div class="article-tags"><span class="chip">Waymo</span><span class="chip">AI</span><span class="chip">UX</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/waymo-gemini-ai-ojai-robotaxi-redesigned-interface/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

    </div>
  </div>

  <div class="sec-group reveal" id="finance">
    <h2 class="section-title">Finance <span class="count">2 stories</span></h2>
    <div class="article-table">

      <div class="article-row">
        <div class="score-chip">72</div>
        <div class="article-main">
          <a class="headline" href="https://www.greencarreports.com/news/1146051_gm-pilot-ev-charging-network-now-spans-over-25-states" target="_blank" rel="noopener">GM‑Pilot with EVgo expands; capex pivots to plazas</a>
          <div class="article-take">High‑traffic travel centers concentrate ROI versus scattered urban fast‑charging.</div>
          <div class="article-tags"><span class="chip">Capex</span><span class="chip">Charging</span><span class="chip">Partnerships</span></div>
        </div>
        <div class="article-source">
          <span>Green Car Reports — Aug 2, 2026</span>
          <a href="https://www.greencarreports.com/news/1146051_gm-pilot-ev-charging-network-now-spans-over-25-states" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      

      <div class="article-row">
        <div class="score-chip">69</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/30/rivian-rivn-q2-2026-earnings-r2-deliveries-revenue-up-27/" target="_blank" rel="noopener">Rivian Q2: revenue up 27% and record gross profit</a>
          <div class="article-take">R2 deliveries begin to bend the cost curve; watch cash burn vs. ramp stability.</div>
          <div class="article-tags"><span class="chip">Rivian</span><span class="chip">Earnings</span><span class="chip">Margins</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 30, 2026</span>
          <a href="https://electrek.co/2026/07/30/rivian-rivn-q2-2026-earnings-r2-deliveries-revenue-up-27/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

    </div>
  </div>

  <div class="sec-group reveal" id="international">
    <h2 class="section-title">International <span class="count">3 stories</span></h2>
    <div class="article-table">

      <div class="article-row">
        <div class="score-chip">71</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/philippines-launches-e850m-incentive-programme-for-ev-manufacturing/" target="_blank" rel="noopener">Philippines courts EV makers with €850m package</a>
          <div class="article-take">New regional manufacturing nodes compete for final assembly and battery pack lines.</div>
          <div class="article-tags"><span class="chip">APAC</span><span class="chip">Policy</span><span class="chip">Manufacturing</span></div>
        </div>
        <div class="article-source">
          <span>Electrive — Aug 4, 2026</span>
          <a href="https://www.electrive.com/2026/08/04/philippines-launches-e850m-incentive-programme-for-ev-manufacturing/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      

      <div class="article-row">
        <div class="score-chip">70</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/04/tesla-china-sales-crash-exports-surge-h1-2026/" target="_blank" rel="noopener">Tesla’s China sales slide as exports surge 127%</a>
          <div class="article-take">Shanghai pivots to export hub role amid intensifying domestic competition.</div>
          <div class="article-tags"><span class="chip">China</span><span class="chip">Exports</span><span class="chip">Competition</span></div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 4, 2026</span>
          <a href="https://electrek.co/2026/08/04/tesla-china-sales-crash-exports-surge-h1-2026/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>      

      <div class="article-row">
        <div class="score-chip">68</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/03/norways-ev-share-rises-to-97-6-in-july/" target="_blank" rel="noopener">Norway’s EV share hits 97.6% in July</a>
          <div class="article-take">Market maturity offers a preview of charging, aftersales, and residual trends elsewhere.</div>
          <div class="article-tags"><span class="chip">Norway</span><span class="chip">EV share</span><span class="chip">Policy outcomes</span></div>
        </div>
        <div class="article-source">
          <span>Electrive — Aug 3, 2026</span>
          <a href="https://www.electrive.com/2026/08/03/norways-ev-share-rises-to-97-6-in-july/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

    </div>
  </div>

  <div class="sec-group reveal" id="opinion">
    <h2 class="section-title">Opinion <span class="count">1 story</span></h2>
    <div class="article-table">

      <div class="article-row">
        <div class="score-chip">60</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/opinion/new-cars/ignore-jay-leno-your-dream-garage-only-needs-three-cars" target="_blank" rel="noopener">Ignore Jay Leno: your dream garage only needs three cars</a>
          <div class="article-take">A focused fleet beats sprawling collections—practical thinking for today’s owners.</div>
          <div class="article-tags"><span class="chip">Opinion</span><span class="chip">Ownership</span></div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 4, 2026</span>
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