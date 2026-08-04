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
        <p class="exec-summary">US auto-safety regulators launched a wide probe into possible front lateral link separations on 2018–2020 Model 3 and 2021–2023 Model Y vehicles. The case tests Tesla’s quality control and service response, and it could trigger a massive repair campaign just as the company navigates margin pressure and regulatory scrutiny across autonomy and safety.</p>

        <div class="takeaways">
          <h3>Key Takeaways</h3>
          <ul>
            <li>156 complaints cite a front suspension link detaching while driving; NHTSA is assessing frequency, severity and root cause.</li>
            <li>Any resulting recall would be one of Tesla’s largest US service actions in recent years and could weigh on delivery timing and costs.</li>
            <li>The probe sharpens the focus on Tesla’s hardware reliability as the company pushes software-led features and Full Self-Driving.</li>
          </ul>
        </div>

        <div class="impact-row">
          <div class="impact-block">
            <h4>Industry Impact</h4>
            <p>Large-scale component probes often ripple through suppliers, service networks and residual values. A mandated fix would add near‑term cost and capacity strain while pulling engineering focus into validation and audit work. It also reinforces a broader regulatory pivot toward mechanical safety even as ADAS dominates headlines, a cue for every EV maker scaling fast to recheck durability and supplier oversight.</p>
          </div>
          <div class="impact-block">
            <h4>Companies Affected</h4>
            <div class="chip-row">
              <span class="chip entity-mfr">Tesla</span>
              <span class="chip entity-mfr">NHTSA</span>
              <span class="chip entity-mfr">Model 3</span>
              <span class="chip entity-mfr">Model Y</span>
            </div>
          </div>
        </div>

        <div class="source-strip">
          <span>Source: <b>Electrek</b></span>
          <span>Reported July 31, 2026</span>
          <a href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">Read original →</a>
        </div>

        <div class="related">
          <h4>Related Coverage</h4>
          <ul>
            <li><a href="https://www.electrive.com/2026/08/03/nhtsa-opens-probe-into-1-2-million-teslas/" target="_blank" rel="noopener">NHTSA opens probe into 1.2 million Teslas (electrive)</a></li>
            <li><a href="https://electrek.co/2026/07/30/tesla-10-millionth-vehicle-ev-growth-stalled/" target="_blank" rel="noopener">Tesla hits 10 million vehicles — growth challenges remain (Electrek)</a></li>
            <li><a href="https://electrek.co/2026/08/03/tesla-fsd-v14-lite-hw3-computer-failures/" target="_blank" rel="noopener">Owners report HW3 overheating with latest FSD build (Electrek)</a></li>
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
          <svg viewBox="0 0 120 70"><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#2a3038" stroke-width="8"/><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#f2a93b" stroke-width="8" stroke-dasharray="157" stroke-dashoffset="7.9"/></svg>
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
    <h2 class="section-title">Industry Snapshot <span class="count">Week of Jul 29 – Aug 4, 2026</span></h2>
    <div class="dash-grid">
      <div class="stat-panel">
        <h4>Top Manufacturers</h4>
        <ul class="rank-list">
          <li><span>Tesla</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:100%"></div></div><span class="rank-count">28</span></li>
          <li><span>BYD</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:86%"></div></div><span class="rank-count">24</span></li>
          <li><span>Hyundai/Kia</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:79%"></div></div><span class="rank-count">22</span></li>
          <li><span>BMW</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:68%"></div></div><span class="rank-count">19</span></li>
          <li><span>Mercedes‑Benz</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:61%"></div></div><span class="rank-count">17</span></li>
        </ul>
      </div>
      <div class="stat-panel">
        <h4>Top Brands</h4>
        <ul class="rank-list">
          <li><span>Audi</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:85%"></div></div><span class="rank-count">23</span></li>
          <li><span>Volkswagen</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:74%"></div></div><span class="rank-count">20</span></li>
          <li><span>Genesis</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:59%"></div></div><span class="rank-count">16</span></li>
          <li><span>Volvo</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:52%"></div></div><span class="rank-count">14</span></li>
          <li><span>Ford</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:44%"></div></div><span class="rank-count">12</span></li>
        </ul>
      </div>
      <div class="stat-panel">
        <h4>Top Suppliers</h4>
        <ul class="rank-list">
          <li><span>SK On</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:100%"></div></div><span class="rank-count">8</span></li>
          <li><span>Factorial Energy</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:88%"></div></div><span class="rank-count">7</span></li>
          <li><span>MAHLE</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:75%"></div></div><span class="rank-count">6</span></li>
          <li><span>AVL</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:63%"></div></div><span class="rank-count">5</span></li>
          <li><span>Beam Global</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:50%"></div></div><span class="rank-count">4</span></li>
        </ul>
      </div>
      <div class="stat-panel">
        <h4>Most Mentioned Executives</h4>
        <ul class="rank-list">
          <li><span>Ola Källenius (Mercedes‑Benz)</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:100%"></div></div><span class="rank-count">6</span></li>
          <li><span>Milan Nedeljković (BMW)</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:83%"></div></div><span class="rank-count">5</span></li>
          <li><span>Jim Baumbick (Ford)</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:67%"></div></div><span class="rank-count">4</span></li>
          <li><span>RJ Scaringe (Rivian)</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:50%"></div></div><span class="rank-count">3</span></li>
        </ul>
      </div>
      <div class="stat-panel">
        <h4>Trending Topics</h4>
        <div class="tagcloud">
          <span class="chip lg">Safety probes</span>
          <span class="chip lg">Solid‑state batteries</span>
          <span class="chip">Ultra‑fast charging</span>
          <span class="chip">Software‑defined vehicles</span>
          <span class="chip">Autonomous ride‑hail</span>
          <span class="chip">China export mix</span>
          <span class="chip">Low‑cost EVs</span>
        </div>
      </div>
      <div class="stat-panel">
        <h4>Emerging Technologies</h4>
        <div class="tagcloud">
          <span class="chip">Iron‑air storage</span>
          <span class="chip">800V platforms</span>
          <span class="chip">Vision‑language AI in UX</span>
          <span class="chip">LFP packs @ 100% SOC</span>
          <span class="chip">Rare‑earth‑free motors</span>
          <span class="chip">V2L & VPPs</span>
        </div>
      </div>
      <div class="stat-panel">
        <h4>Government Activity</h4>
        <ul class="rank-list">
          <li><span>NHTSA Tesla probe</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:100%"></div></div><span class="rank-count">1</span></li>
          <li><span>Philippines EV incentives</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:75%"></div></div><span class="rank-count">1</span></li>
          <li><span>UK/Denmark EV policy</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:58%"></div></div><span class="rank-count">2</span></li>
        </ul>
      </div>
      <div class="stat-panel">
        <h4>Supplier & Charging Moves</h4>
        <ul class="rank-list">
          <li><span>SK On–Factorial alliance</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:100%"></div></div><span class="rank-count">1</span></li>
          <li><span>EVgo + Brixmor rollout</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:83%"></div></div><span class="rank-count">1</span></li>
          <li><span>Beam Global city pilots</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:67%"></div></div><span class="rank-count">2</span></li>
        </ul>
      </div>
      <div class="stat-panel">
        <h4>Financial Pulse</h4>
        <ul class="rank-list">
          <li><span>Rivian Q2 beat</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:100%"></div></div><span class="rank-count">$1.66B</span></li>
          <li><span>BYD July sales</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:78%"></div></div><span class="rank-count">+22%</span></li>
          <li><span>Lucid stake filing</span><div class="rank-bar-wrap"><div class="rank-bar" style="width:62%"></div></div><span class="rank-count">+25%</span></li>
        </ul>
      </div>
      <div class="stat-panel">
        <h4>Global Regions</h4>
        <div class="tagcloud">
          <span class="chip lg">United States</span>
          <span class="chip lg">China</span>
          <span class="chip">EU & UK</span>
          <span class="chip">Nordics</span>
          <span class="chip">Southeast Asia</span>
          <span class="chip">Latin America</span>
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
        <a href="https://www.autocar.co.uk/car-news/new-cars/new-mercedes-gla-revealed-audi-q4-rival-408-mile-range" target="_blank" rel="noopener">Mercedes unveils new GLA EV with up to 408 miles range</a>
        <div class="fp-meta"><span>Score 76</span><span>Autocar — Jul 29, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">BMW hits pause on G‑Class rival amid China headwinds</a>
        <div class="fp-meta"><span>Score 72</span><span>Autocar — Aug 4, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/ferrari-luce-ev-sold-out-2026-allocation/" target="_blank" rel="noopener">Ferrari’s Luce EV sells out 2026 allocation (~500 units)</a>
        <div class="fp-meta"><span>Score 70</span><span>Electrek — Jul 29, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/28/bmw-ramps-up-ix3-output-orders-near-100000/" target="_blank" rel="noopener">BMW ramps iX3 output as orders near 100,000</a>
        <div class="fp-meta"><span>Score 68</span><span>Electrek — Jul 28, 2026</span></div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Technology</h3>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/waymo-gemini-ai-ojai-robotaxi-redesigned-interface/" target="_blank" rel="noopener">Waymo bakes Google Gemini into robotaxi with new UI</a>
        <div class="fp-meta"><span>Score 78</span><span>Electrek — Jul 29, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">SK On and Factorial form solid‑state battery alliance</a>
        <div class="fp-meta"><span>Score 74</span><span>Electrek — Jul 29, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.autocar.co.uk/car-news/new-cars/reborn-audi-a2-driven-electric-comeback-efficiency-king" target="_blank" rel="noopener">Audi previews ultra‑efficient A2 e‑tron</a>
        <div class="fp-meta"><span>Score 69</span><span>Autocar — Aug 1, 2026</span></div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Government & Safety</h3>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">NHTSA opens probe into 1.2M Teslas over suspension</a>
        <div class="fp-meta"><span>Score 92</span><span>Electrek — Jul 31, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.electrive.com/2026/08/04/philippines-launches-e850m-incentive-programme-for-ev-manufacturing/" target="_blank" rel="noopener">Philippines launches €850m EV manufacturing incentives</a>
        <div class="fp-meta"><span>Score 66</span><span>electrive — Aug 4, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.roadandtrack.com/news/a73278061/california-tire-efficiency-program-niche-exemptions-for-enthusiasts/" target="_blank" rel="noopener">California carves tire‑efficiency exemptions for niche uses</a>
        <div class="fp-meta"><span>Score 58</span><span>Road & Track — Jul 29, 2026</span></div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Suppliers & Charging</h3>
      <div class="fp-row">
        <a href="https://chargedevs.com/newswire/mahle-introduces-a-new-range-extender-engine-and-a-rare-earth-free-electric-motor/" target="_blank" rel="noopener">MAHLE unveils truck range‑extender and rare‑earth‑free motor</a>
        <div class="fp-meta"><span>Score 62</span><span>Charged — Jul 31, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.electrive.com/2026/08/04/evgo-and-brixmor-to-add-more-than-500-fast-charging-stalls-in-the-us/" target="_blank" rel="noopener">EVgo, Brixmor plan 500+ new fast‑charging stalls</a>
        <div class="fp-meta"><span>Score 66</span><span>electrive — Aug 4, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://chargedevs.com/newswire/beam-global-supplies-ev-arc-off-grid-charging-systems-for-dallas-municipal-fleet-and-massachusetts-carshare-pilot/" target="_blank" rel="noopener">Cities add off‑grid solar EV chargers for fleets & carshare</a>
        <div class="fp-meta"><span>Score 60</span><span>Charged — Jul 30, 2026</span></div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Trending Topics</h3>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/477795/" target="_blank" rel="noopener">IEA: Global EV sales rebound 35% in Q2; 50 countries set records</a>
        <div class="fp-meta"><span>Score 80</span><span>Electrek — Jul 29, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/28/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Volvo drops lidar on EX90/ES90 and compensates owners</a>
        <div class="fp-meta"><span>Score 85</span><span>Electrek — Jul 29, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.electrive.com/2026/08/04/denmark-evs-account-for-almost-all-new-car-registrations-in-july/" target="_blank" rel="noopener">Denmark logs 97% EV share in July</a>
        <div class="fp-meta"><span>Score 65</span><span>electrive — Aug 4, 2026</span></div>
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
        <div class="score-chip high">92</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">NHTSA probes 1.2M Tesla Model 3/Y for front suspension link failures</a>
          <div class="article-take">A large safety probe puts Tesla’s quality systems and service throughput under the microscope ahead of a possible major fix.</div>
          <div class="article-tags">
            <span class="chip">Safety</span><span class="chip">Government</span><span class="chip">EV</span>
            <span class="chip">Tesla</span><span class="chip">NHTSA</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek</span>
          <span>Jul 31, 2026</span>
          <a href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip high">85</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Volvo drops lidar for EX90/ES90 and compensates owners</a>
          <div class="article-take">The move resets Volvo’s sensor stack and ripples to lidar supplier plans, while managing customer expectations with payouts.</div>
          <div class="article-tags">
            <span class="chip">ADAS</span><span class="chip">Technology</span><span class="chip">Suppliers</span>
            <span class="chip">Volvo</span><span class="chip">Luminar</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek</span>
          <span>Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">78</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/waymo-gemini-ai-ojai-robotaxi-redesigned-interface/" target="_blank" rel="noopener">Waymo adds Gemini AI and new rider interface to Ojai robotaxi</a>
          <div class="article-take">Embedding a general AI assistant signals a shift from pure autonomy demos toward a fuller passenger experience layer.</div>
          <div class="article-tags">
            <span class="chip">Autonomous</span><span class="chip">Software</span><span class="chip">Mobility</span>
            <span class="chip">Waymo</span><span class="chip">Google</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek</span>
          <span>Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/waymo-gemini-ai-ojai-robotaxi-redesigned-interface/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">80</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/477795/" target="_blank" rel="noopener">IEA: Global EV sales jump 35% in Q2; records in 50 countries</a>
          <div class="article-take">After a soft Q1, demand re-accelerated broadly, easing fears of a prolonged EV slowdown.</div>
          <div class="article-tags">
            <span class="chip">EV</span><span class="chip">Finance</span><span class="chip">Global</span>
            <span class="chip">IEA</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek</span>
          <span>Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/477795/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">76</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/electric-cars/new-mercedes-gla-revealed-audi-q4-rival-408-mile-range" target="_blank" rel="noopener">New Mercedes GLA EV revealed with up to 408‑mile range</a>
          <div class="article-take">Mercedes scales its compact EV strategy with MMA platform, 800V charging and a mass‑market footprint.</div>
          <div class="article-tags">
            <span class="chip">EV</span><span class="chip">Products</span><span class="chip">Manufacturing</span>
            <span class="chip">Mercedes‑Benz</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar</span>
          <span>Jul 29, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/electric-cars/new-mercedes-gla-revealed-audi-q4-rival-408-mile-range" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">74</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">SK On, Factorial team up to scale solid‑state EV batteries</a>
          <div class="article-take">A new alliance aims to compress the path from pilot cells to automaker‑grade packs in high volume.</div>
          <div class="article-tags">
            <span class="chip">Battery</span><span class="chip">Suppliers</span><span class="chip">Technology</span>
            <span class="chip">SK On</span><span class="chip">Factorial</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek</span>
          <span>Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">73</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/07/31/tesla-tops-10-million-electric-vehicles-built/" target="_blank" rel="noopener">Tesla passes 10 million cumulative EVs built</a>
          <div class="article-take">A manufacturing milestone underscores scale leadership but comes amid slowing plant utilization.</div>
          <div class="article-tags">
            <span class="chip">Production</span><span class="chip">EV</span><span class="chip">Manufacturing</span>
            <span class="chip">Tesla</span>
          </div>
        </div>
        <div class="article-source">
          <span>electrive</span>
          <span>Jul 31, 2026</span>
          <a href="https://www.electrive.com/2026/07/31/tesla-tops-10-million-electric-vehicles-built/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">72</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/hyundai-reveals-ioniq-3-prices-start-30000-interest-surges/" target="_blank" rel="noopener">Hyundai IONIQ 3 starts around $30k; interest surges</a>
          <div class="article-take">An attainable price, 300‑mile range and updated infotainment target mainstream EV adoption.</div>
          <div class="article-tags">
            <span class="chip">EV</span><span class="chip">Retail</span><span class="chip">Products</span>
            <span class="chip">Hyundai</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek</span>
          <span>Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/hyundai-reveals-ioniq-3-prices-start-30000-interest-surges/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">71</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/28/volkswagen-launches-cheaper-id-polo-ev-orders-25000/" target="_blank" rel="noopener">VW launches cheaper ID. Polo EV; 25,000 orders already</a>
          <div class="article-take">Sub‑$30k variants show legacy makers leaning into compact EV value at scale.</div>
          <div class="article-tags">
            <span class="chip">EV</span><span class="chip">Retail</span><span class="chip">Manufacturing</span>
            <span class="chip">Volkswagen</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek</span>
          <span>Jul 28, 2026</span>
          <a href="https://electrek.co/2026/07/28/volkswagen-launches-cheaper-id-polo-ev-orders-25000/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">70</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/ferrari-luce-ev-sold-out-2026-allocation/" target="_blank" rel="noopener">Ferrari Luce EV hits first‑year sales target</a>
          <div class="article-take">Even at super‑luxury pricing, early EV demand signals brand power and constrained supply.</div>
          <div class="article-tags">
            <span class="chip">EV</span><span class="chip">Luxury</span><span class="chip">Retail</span>
            <span class="chip">Ferrari</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek</span>
          <span>Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/ferrari-luce-ev-sold-out-2026-allocation/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">69</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/03/byd-opens-denza-z9s-pre-orders-record-1100-km-ev-range/" target="_blank" rel="noopener">BYD’s Denza Z9S claims 1,100 km EV range; pre‑orders open</a>
          <div class="article-take">Range one‑upmanship continues as Chinese premium EVs push long‑distance capability.</div>
          <div class="article-tags">
            <span class="chip">EV</span><span class="chip">Products</span><span class="chip">China</span>
            <span class="chip">BYD</span><span class="chip">Denza</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek</span>
          <span>Aug 3, 2026</span>
          <a href="https://electrek.co/2026/08/03/byd-opens-denza-z9s-pre-orders-record-1100-km-ev-range/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">68</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/audi-q9-suv-revealed-huge-%C2%A3100k-a8-successor" target="_blank" rel="noopener">Audi reveals Q9 flagship SUV as indirect A8 successor</a>
          <div class="article-take">A tech‑heavy, high‑margin SUV continues premium brands’ pivot away from large sedans.</div>
          <div class="article-tags">
            <span class="chip">Manufacturers</span><span class="chip">Products</span><span class="chip">ICE/Hybrid</span>
            <span class="chip">Audi</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar</span>
          <span>Jul 30, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/audi-q9-suv-revealed-huge-%C2%A3100k-a8-successor" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">66</div>
        <div class="article-main">
          <a class="headline" href="https://www.greencarreports.com/news/1146051_gm-pilot-ev-charging-network-now-spans-over-25-states" target="_blank" rel="noopener">GM–Pilot fast‑charging network now spans 25+ US states</a>
          <div class="article-take">Multi‑party charging buildouts broaden corridor coverage beyond early coastal hubs.</div>
          <div class="article-tags">
            <span class="chip">Charging</span><span class="chip">Infrastructure</span><span class="chip">US</span>
            <span class="chip">GM</span><span class="chip">EVgo</span>
          </div>
        </div>
        <div class="article-source">
          <span>Green Car Reports</span>
          <span>Aug 4, 2026</span>
          <a href="https://www.greencarreports.com/news/1146051_gm-pilot-ev-charging-network-now-spans-over-25-states" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">65</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/denmark-evs-account-for-almost-all-new-car-registrations-in-july/" target="_blank" rel="noopener">Denmark nears 98% EV share in July private registrations</a>
          <div class="article-take">Another Nordic market shows how policy, product and charging density compound adoption.</div>
          <div class="article-tags">
            <span class="chip">EV</span><span class="chip">International</span><span class="chip">Policy</span>
            <span class="chip">Denmark</span>
          </div>
        </div>
        <div class="article-source">
          <span>electrive</span>
          <span>Aug 4, 2026</span>
          <a href="https://www.electrive.com/2026/08/04/denmark-evs-account-for-almost-all-new-car-registrations-in-july/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">72</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/30/rivian-rivn-q2-2026-earnings-r2-deliveries-revenue-up-27/" target="_blank" rel="noopener">Rivian Q2: revenue +27%, record gross profit, R2 deliveries started</a>
          <div class="article-take">Scaling the lower‑priced R2 shifts Rivian toward volume economics while improving unit costs.</div>
          <div class="article-tags">
            <span class="chip">Finance</span><span class="chip">EV</span><span class="chip">Manufacturers</span>
            <span class="chip">Rivian</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek</span>
          <span>Jul 30, 2026</span>
          <a href="https://electrek.co/2026/07/30/rivian-rivn-q2-2026-earnings-r2-deliveries-revenue-up-27/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">72</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">BMW reevaluates product plan; off‑roader on hold</a>
          <div class="article-take">Demand divergence and tariff risk are forcing tighter model discipline and platform reuse.</div>
          <div class="article-tags">
            <span class="chip">Manufacturers</span><span class="chip">Strategy</span><span class="chip">China</span>
            <span class="chip">BMW</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar</span>
          <span>Aug 4, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">Read original →</a>
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
    <h2 class="section-title">Industry News <span class="count">Market, policy and strategy</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip high">92</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">NHTSA opens probe into 1.2M Teslas over suspension</a>
          <div class="article-take">US regulators escalate scrutiny of a critical hardware reliability issue at scale.</div>
          <div class="article-tags"><span class="chip">Safety</span><span class="chip">Government</span><span class="chip">Tesla</span></div>
        </div>
        <div class="article-source">
          <span>Electrek</span><span>Jul 31, 2026</span>
          <a href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">80</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/477795/" target="_blank" rel="noopener">IEA: Global EV sales jump 35% in Q2</a>
          <div class="article-take">Adoption momentum rebounds broadly after a choppy first quarter.</div>
          <div class="article-tags"><span class="chip">EV</span><span class="chip">Finance</span><span class="chip">Global</span></div>
        </div>
        <div class="article-source">
          <span>Electrek</span><span>Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/477795/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">73</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/07/31/tesla-tops-10-million-electric-vehicles-built/" target="_blank" rel="noopener">Tesla tops 10 million EVs built</a>
          <div class="article-take">Milestone highlights production scale amid utilization and demand mix shifts.</div>
          <div class="article-tags"><span class="chip">Production</span><span class="chip">Manufacturing</span><span class="chip">Tesla</span></div>
        </div>
        <div class="article-source">
          <span>electrive</span><span>Jul 31, 2026</span>
          <a href="https://www.electrive.com/2026/07/31/tesla-tops-10-million-electric-vehicles-built/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">72</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/03/hyundai-kias-record-us-sales-run/" target="_blank" rel="noopener">Hyundai & Kia extend US record sales streak on electrified mix</a>
          <div class="article-take">Hybrid and affordable EV entries continue to propel share gains.</div>
          <div class="article-tags"><span class="chip">Retail</span><span class="chip">Hybrid</span><span class="chip">EV</span></div>
        </div>
        <div class="article-source">
          <span>Electrek</span><span>Aug 3, 2026</span>
          <a href="https://electrek.co/2026/08/03/hyundai-kias-record-us-sales-run/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="electric-vehicles">
    <h2 class="section-title">Electric Vehicles <span class="count">Products and adoption</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip">76</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/electric-cars/new-mercedes-gla-revealed-audi-q4-rival-408-mile-range" target="_blank" rel="noopener">Mercedes GLA EV debuts with up to 408‑mile range, 800V charging</a>
          <div class="article-take">Compact segment gets a long‑range, fast‑charge contender from Stuttgart.</div>
          <div class="article-tags"><span class="chip">EV</span><span class="chip">Products</span><span class="chip">Mercedes‑Benz</span></div>
        </div>
        <div class="article-source">
          <span>Autocar</span><span>Jul 29, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/electric-cars/new-mercedes-gla-revealed-audi-q4-rival-408-mile-range" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">72</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/hyundai-reveals-ioniq-3-prices-start-30000-interest-surges/" target="_blank" rel="noopener">Hyundai IONIQ 3 starts at ~$30k, strong demand at launch</a>
          <div class="article-take">Aggressive pricing and range aim squarely at mainstream buyers.</div>
          <div class="article-tags"><span class="chip">EV</span><span class="chip">Retail</span><span class="chip">Hyundai</span></div>
        </div>
        <div class="article-source">
          <span>Electrek</span><span>Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/hyundai-reveals-ioniq-3-prices-start-30000-interest-surges/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">71</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/28/volkswagen-launches-cheaper-id-polo-ev-orders-25000/" target="_blank" rel="noopener">Volkswagen opens orders for lower‑priced ID. Polo EV</a>
          <div class="article-take">High early order volume validates the compact‑EV value thesis.</div>
          <div class="article-tags"><span class="chip">EV</span><span class="chip">Products</span><span class="chip">Volkswagen</span></div>
        </div>
        <div class="article-source">
          <span>Electrek</span><span>Jul 28, 2026</span>
          <a href="https://electrek.co/2026/07/28/volkswagen-launches-cheaper-id-polo-ev-orders-25000/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">69</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/03/byd-opens-denza-z9s-pre-orders-record-1100-km-ev-range/" target="_blank" rel="noopener">BYD’s Denza Z9S claims 1,100 km range; pre‑orders start</a>
          <div class="article-take">Premium EVs keep stretching range envelopes to differentiate.</div>
          <div class="article-tags"><span class="chip">EV</span><span class="chip">China</span><span class="chip">BYD</span></div>
        </div>
        <div class="article-source">
          <span>Electrek</span><span>Aug 3, 2026</span>
          <a href="https://electrek.co/2026/08/03/byd-opens-denza-z9s-pre-orders-record-1100-km-ev-range/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="manufacturers">
    <h2 class="section-title">Manufacturers <span class="count">Product & strategy moves</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip">72</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">BMW reevaluates lineup; off‑roader paused</a>
          <div class="article-take">Macro shifts drive tougher new‑model gatekeeping.</div>
          <div class="article-tags"><span class="chip">Strategy</span><span class="chip">BMW</span></div>
        </div>
        <div class="article-source">
          <span>Autocar</span><span>Aug 4, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">68</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/audi-q9-suv-revealed-huge-%C2%A3100k-a8-successor" target="_blank" rel="noopener">Audi Q9 arrives as tech‑led flagship SUV</a>
          <div class="article-take">Premium brands keep chasing margins with large SUVs.</div>
          <div class="article-tags"><span class="chip">Products</span><span class="chip">Audi</span></div>
        </div>
        <div class="article-source">
          <span>Autocar</span><span>Jul 30, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/audi-q9-suv-revealed-huge-%C2%A3100k-a8-successor" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">70</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/ferrari-luce-ev-sold-out-2026-allocation/" target="_blank" rel="noopener">Ferrari Luce EV sells out year one</a>
          <div class="article-take">Ultra‑luxury EV demand remains supply‑constrained.</div>
          <div class="article-tags"><span class="chip">Luxury</span><span class="chip">Ferrari</span></div>
        </div>
        <div class="article-source">
          <span>Electrek</span><span>Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/ferrari-luce-ev-sold-out-2026-allocation/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="dealers">
    <h2 class="section-title">Dealers <span class="count">Retail & distribution</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip">60</div>
        <div class="article-main">
          <a class="headline" href="https://www.carscoops.com/2026/08/servicemember-repossession-settlement/" target="_blank" rel="noopener">US DOJ settles with dealer over improper repossessions</a>
          <div class="article-take">Compliance lapses bring penalties and reputational risk to retail networks.</div>
          <div class="article-tags"><span class="chip">Dealers</span><span class="chip">Government</span><span class="chip">Legal</span></div>
        </div>
        <div class="article-source">
          <span>Carscoops</span><span>Aug 4, 2026</span>
          <a href="https://www.carscoops.com/2026/08/servicemember-repossession-settlement/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">58</div>
        <div class="article-main">
          <a class="headline" href="https://www.motor1.com/news/803722/costco-infiniti-discount/" target="_blank" rel="noopener">Costco offers fresh discounts on new Infiniti SUVs</a>
          <div class="article-take">Big‑box partnerships keep fueling traffic and price transparency.</div>
          <div class="article-tags"><span class="chip">Retail</span><span class="chip">Incentives</span><span class="chip">Infiniti</span></div>
        </div>
        <div class="article-source">
          <span>Motor1</span><span>Aug 3, 2026</span>
          <a href="https://www.motor1.com/news/803722/costco-infiniti-discount/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="suppliers">
    <h2 class="section-title">Suppliers <span class="count">Batteries, components & charging</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip">74</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">SK On and Factorial form solid‑state battery alliance</a>
          <div class="article-take">Partnership targets manufacturability and carmaker qualification at scale.</div>
          <div class="article-tags"><span class="chip">Battery</span><span class="chip">Suppliers</span><span class="chip">Solid‑state</span></div>
        </div>
        <div class="article-source">
          <span>Electrek</span><span>Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">62</div>
        <div class="article-main">
          <a class="headline" href="https://chargedevs.com/newswire/mahle-introduces-a-new-range-extender-engine-and-a-rare-earth-free-electric-motor/" target="_blank" rel="noopener">MAHLE debuts truck range‑extender, rare‑earth‑free e‑motor</a>
          <div class="article-take">Suppliers hedge with combustion‑assist solutions while reducing materials risk.</div>
          <div class="article-tags"><span class="chip">Suppliers</span><span class="chip">Powertrain</span><span class="chip">Sustainability</span></div>
        </div>
        <div class="article-source">
          <span>Charged</span><span>Jul 31, 2026</span>
          <a href="https://chargedevs.com/newswire/mahle-introduces-a-new-range-extender-engine-and-a-rare-earth-free-electric-motor/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">60</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/03/blue-solutions-and-avl-test-solid-state-battery-safety/" target="_blank" rel="noopener">Blue Solutions & AVL validate solid‑state safety methods</a>
          <div class="article-take">Thermal propagation work advances industrialization readiness.</div>
          <div class="article-tags"><span class="chip">Battery</span><span class="chip">Safety</span><span class="chip">R&amp;D</span></div>
        </div>
        <div class="article-source">
          <span>electrive</span><span>Aug 3, 2026</span>
          <a href="https://www.electrive.com/2026/08/03/blue-solutions-and-avl-test-solid-state-battery-safety/" target="_blank" rel="noopener">Read original →</a>
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
          <a class="headline" href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">NHTSA investigates Tesla Model 3/Y suspension link failures</a>
          <div class="article-take">Potential large‑scale repair action looms over Tesla’s US fleet.</div>
          <div class="article-tags"><span class="chip">Safety</span><span class="chip">Regulation</span><span class="chip">Tesla</span></div>
        </div>
        <div class="article-source">
          <span>Electrek</span><span>Jul 31, 2026</span>
          <a href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">66</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/philippines-launches-e850m-incentive-programme-for-ev-manufacturing/" target="_blank" rel="noopener">Philippines unveils €850m EV manufacturing incentives</a>
          <div class="article-take">New subsidies court assembly and component investment into ASEAN.</div>
          <div class="article-tags"><span class="chip">Trade</span><span class="chip">Manufacturing</span><span class="chip">Policy</span></div>
        </div>
        <div class="article-source">
          <span>electrive</span><span>Aug 4, 2026</span>
          <a href="https://www.electrive.com/2026/08/04/philippines-launches-e850m-incentive-programme-for-ev-manufacturing/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="technology">
    <h2 class="section-title">Technology <span class="count">Software & hardware</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip">78</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/waymo-gemini-ai-ojai-robotaxi-redesigned-interface/" target="_blank" rel="noopener">Waymo integrates Gemini AI, refreshes robotaxi UX</a>
          <div class="article-take">Conversational AI meets autonomy to smooth rider experience.</div>
          <div class="article-tags"><span class="chip">Autonomous</span><span class="chip">Software</span><span class="chip">UX</span></div>
        </div>
        <div class="article-source">
          <span>Electrek</span><span>Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/waymo-gemini-ai-ojai-robotaxi-redesigned-interface/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">69</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/reborn-audi-a2-driven-electric-comeback-efficiency-king" target="_blank" rel="noopener">Audi A2 e‑tron: aero‑driven efficiency revival</a>
          <div class="article-take">Packaging and LFP updates aim for standout miles/kWh.</div>
          <div class="article-tags"><span class="chip">Efficiency</span><span class="chip">EV</span><span class="chip">Audi</span></div>
        </div>
        <div class="article-source">
          <span>Autocar</span><span>Aug 1, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/reborn-audi-a2-driven-electric-comeback-efficiency-king" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      <div class="article-row">
        <div class="score-chip">62</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/mercedes-big-screens-stay-we-went-too-far-removing-buttons" target="_blank" rel="noopener">Mercedes: big screens stay, some buttons return</a>
          <div class="article-take">Carmaker rebalances UI after customer pushback on touch‑only controls.</div>
          <div class="article-tags"><span class="chip">Software</span><span class="chip">HMI</span><span class="chip">Mercedes‑Benz</span></div>
        </div>
        <div class="article-source">
          <span>Autocar</span><span>Jul 31, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/mercedes-big-screens-stay-we-went-too-far-removing-buttons" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="finance">
    <h2 class="section-title">Finance <span class="count">Earnings & deals</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip">72</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/30/rivian-rivn-q2-2026-earnings-r2-deliveries-revenue-up-27/" target="_blank" rel="noopener">Rivian Q2 revenue up 27% with record gross profit</a>
          <div class="article-take">Mix shift to lower‑priced R2 starts to bend the cost curve.</div>
          <div class="article-tags"><span class="chip">Earnings</span><span class="chip">EV</span><span class="chip">Rivian</span></div>
        </div>
        <div class="article-source">
          <span>Electrek</span><span>Jul 30, 2026</span>
          <a href="https://electrek.co/2026/07/30/rivian-rivn-q2-2026-earnings-r2-deliveries-revenue-up-27/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">68</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/03/byd-boosts-sales-by-22-in-july/" target="_blank" rel="noopener">BYD July sales rise 22% with exports at record share</a>
          <div class="article-take">China’s leader leans harder on overseas markets as domestic growth softens.</div>
          <div class="article-tags"><span class="chip">Sales</span><span class="chip">BYD</span><span class="chip">Exports</span></div>
        </div>
        <div class="article-source">
          <span>electrive</span><span>Aug 3, 2026</span>
          <a href="https://www.electrive.com/2026/08/03/byd-boosts-sales-by-22-in-july/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="international">
    <h2 class="section-title">International <span class="count">Global markets</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip">65</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/denmark-evs-account-for-almost-all-new-car-registrations-in-july/" target="_blank" rel="noopener">Denmark approaches 98% EV share in July private sales</a>
          <div class="article-take">Policy alignment and product breadth drive a near‑full transition snapshot.</div>
          <div class="article-tags"><span class="chip">EV</span><span class="chip">Policy</span><span class="chip">Denmark</span></div>
        </div>
        <div class="article-source">
          <span>electrive</span><span>Aug 4, 2026</span>
          <a href="https://www.electrive.com/2026/08/04/denmark-evs-account-for-almost-all-new-car-registrations-in-july/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">64</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/28/baidu-apollo-go-london-robotaxi-testing-uber-lyft/" target="_blank" rel="noopener">Baidu’s Apollo Go starts London robotaxi testing with Uber & Lyft</a>
          <div class="article-take">Chinese AVs expand west via platform partnerships in RHD markets.</div>
          <div class="article-tags"><span class="chip">Autonomous</span><span class="chip">International</span><span class="chip">Baidu</span></div>
        </div>
        <div class="article-source">
          <span>Electrek</span><span>Jul 28, 2026</span>
          <a href="https://electrek.co/2026/07/28/baidu-apollo-go-london-robotaxi-testing-uber-lyft/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
    </div>
  </div>

  <div class="sec-group reveal" id="opinion">
    <h2 class="section-title">Opinion <span class="count">Analysis & commentary</span></h2>
    <div class="article-table">
      <div class="article-row">
        <div class="score-chip">60</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/opinion/business-manufacturing/chinese-car-makers-all-share-parts-will-world-follow" target="_blank" rel="noopener">China’s shared‑parts playbook: can the rest of the world follow?</a>
          <div class="article-take">Industrial standardization is a key lever behind China’s speed and cost edge.</div>
          <div class="article-tags"><span class="chip">Supply Chain</span><span class="chip">China</span><span class="chip">Opinion</span></div>
        </div>
        <div class="article-source">
          <span>Autocar</span><span>Aug 2, 2026</span>
          <a href="https://www.autocar.co.uk/opinion/business-manufacturing/chinese-car-makers-all-share-parts-will-world-follow" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">54</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/opinion/new-cars/ignore-jay-leno-your-dream-garage-only-needs-three-cars" target="_blank" rel="noopener">Your dream garage only needs three cars</a>
          <div class="article-take">A practical case for focus over volume in enthusiast ownership.</div>
          <div class="article-tags"><span class="chip">Opinion</span><span class="chip">Culture</span></div>
        </div>
        <div class="article-source">
          <span>Autocar</span><span>Aug 1, 2026</span>
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