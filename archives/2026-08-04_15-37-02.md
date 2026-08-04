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
        <h1>NHTSA opens probe into 1.2 million Teslas over front suspension failures</h1>
        <p class="exec-summary">US safety regulators launched a preliminary evaluation into Model 3 (2018–2020) and Model Y (2021–2023) after 150+ complaints of a lower control arm separation while driving. A potential steering-loss defect puts the country’s best-selling EV lineup under a microscope just as Tesla leans more heavily on exports and software-led value. Beyond recall risk, the probe could ripple through warranty costs, residual values, and dealer service bays that depend on Tesla-adjacent work. It also tests the company’s ability to juggle cost-down pressure with durability at scale—especially as new NACS-compatible entrants give consumers more choice.</p>

        <div class="takeaways">
          <h3>Key Takeaways</h3>
          <ul>
            <li>Preliminary evaluation targets lower lateral link separation causing possible steering loss.</li>
            <li>Scope covers ~1.2M US vehicles across Tesla’s highest-volume model years.</li>
            <li>Outcome could include recall, supplier changes, or tightened inspection procedures.</li>
            <li>Probe timing intersects with rising complaints of suspension creak and premature wear.</li>
          </ul>
        </div>

        <div class="impact-row">
          <div class="impact-block">
            <h4>Industry Impact</h4>
            <p>High-visibility safety actions on the largest EV fleet influence consumer trust, used values, and insurer assumptions across the category—not just Tesla. If parts redesigns or inspections are mandated, suppliers of control arms, bushings and fasteners face volume and cost swings. Dealers and independents can see short-term service spikes for inspections and post-repair alignments. Competitively, legacy OEMs may amplify durability messaging as EV adoption broadens to mainstream buyers.</p>
          </div>
          <div class="impact-block">
            <h4>Companies Affected</h4>
            <div class="chip-row">
              <span class="chip entity-mfr">Tesla</span>
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
            <li><a href="https://www.carscoops.com/2026/08/tesla-suspension-investigation/" target="_blank" rel="noopener">Over 150 complaints of Teslas losing front suspension put 1.2M under probe</a></li>
            <li><a href="https://electrek.co/2026/08/04/tesla-china-sales-crash-exports-surge-h1-2026/" target="_blank" rel="noopener">Tesla China sales slump as exports surge out of Shanghai</a></li>
            <li><a href="https://electrek.co/2026/07/30/tesla-10-millionth-vehicle-ev-growth-stalled/" target="_blank" rel="noopener">Tesla hits 10M vehicles built—amid slower utilization of existing capacity</a></li>
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
          <svg viewBox="0 0 120 70"><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#2a3038" stroke-width="8"/><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#f2a93b" stroke-width="8" stroke-dasharray="157" stroke-dashoffset="7.85"/></svg>
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
    <h2 class="section-title">Industry Snapshot <span class="count">Last 7 days through Aug 4, 2026</span></h2>
    <div class="dash-grid">
      
      <div class="stat-panel">
        <h4>Top OEMs in the News</h4>
        <ul class="rank-list">
          <li><span>Tesla</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:92%"></span></span><span class="rank-count">92</span></li>
          <li><span>BMW</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:78%"></span></span><span class="rank-count">78</span></li>
          <li><span>BYD</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:74%"></span></span><span class="rank-count">74</span></li>
          <li><span>Hyundai/Kia</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:70%"></span></span><span class="rank-count">70</span></li>
          <li><span>Volkswagen Group</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:63%"></span></span><span class="rank-count">63</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4>Trending Themes</h4>
        <div class="tagcloud">
          <span class="chip lg">Safety probes</span>
          <span class="chip">Lidar strategy shifts</span>
          <span class="chip">Solid‑state batteries</span>
          <span class="chip lg">Affordable EVs</span>
          <span class="chip">Charging build‑out</span>
          <span class="chip">China exports</span>
          <span class="chip">OEM cost resets</span>
        </div>
      </div>

      <div class="stat-panel">
        <h4>Markets to Watch</h4>
        <ul class="rank-list">
          <li><span>United States</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:85%"></span></span><span class="rank-count">85</span></li>
          <li><span>China</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:80%"></span></span><span class="rank-count">80</span></li>
          <li><span>Nordics</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:68%"></span></span><span class="rank-count">68</span></li>
          <li><span>UK/EU</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:66%"></span></span><span class="rank-count">66</span></li>
        </ul>
      </div>

      <div class="stat-panel">
        <h4>Powertrain Mix (news share)</h4>
        <ul class="rank-list">
          <li><span>BEV</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:64%"></span></span><span class="rank-count">64%</span></li>
          <li><span>Hybrid/PHEV</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:22%"></span></span><span class="rank-count">22%</span></li>
          <li><span>ICE/Other</span><span class="rank-bar-wrap"><span class="rank-bar" style="width:14%"></span></span><span class="rank-count">14%</span></li>
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
        <a href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">BMW pauses G‑Class rival as China headwinds bite</a>
        <div class="fp-meta"><span>Score 82</span><span>•</span><span>Aug 4, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/08/04/tesla-china-sales-crash-exports-surge-h1-2026/" target="_blank" rel="noopener">Tesla’s China sales slide while exports surge</a>
        <div class="fp-meta"><span>Score 80</span><span>•</span><span>Aug 4, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/08/03/hyundai-kias-record-us-sales-run/" target="_blank" rel="noopener">Hyundai and Kia extend record US sales streak</a>
        <div class="fp-meta"><span>Score 76</span><span>•</span><span>Aug 3, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/ferrari-luce-ev-sold-out-2026-allocation/" target="_blank" rel="noopener">Ferrari’s Luce EV sells out 2026 allocation</a>
        <div class="fp-meta"><span>Score 74</span><span>•</span><span>Jul 29, 2026</span></div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Technology</h3>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Volvo ditches lidar on EX90/ES90, pays owners</a>
        <div class="fp-meta"><span>Score 84</span><span>•</span><span>Jul 29, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">SK On and Factorial form solid‑state alliance</a>
        <div class="fp-meta"><span>Score 78</span><span>•</span><span>Jul 29, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.autocar.co.uk/car-news/new-cars/reborn-audi-a2-driven-electric-comeback-efficiency-king" target="_blank" rel="noopener">Audi A2 e‑tron leans into extreme efficiency</a>
        <div class="fp-meta"><span>Score 72</span><span>•</span><span>Aug 1, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/waymo-gemini-ai-ojai-robotaxi-redesigned-interface/" target="_blank" rel="noopener">Waymo bakes Gemini AI into robotaxi UX</a>
        <div class="fp-meta"><span>Score 70</span><span>•</span><span>Jul 29, 2026</span></div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Government & Policy</h3>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">NHTSA probe targets 1.2M Teslas for suspension</a>
        <div class="fp-meta"><span>Score 92</span><span>•</span><span>Jul 31, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.greencarreports.com/news/1146051_gm-pilot-ev-charging-network-now-spans-over-25-states" target="_blank" rel="noopener">GM–Pilot DC fast‑charge buildout tops 25 states</a>
        <div class="fp-meta"><span>Score 75</span><span>•</span><span>Aug 3, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.electrive.com/2026/08/04/denmark-evs-account-for-almost-all-new-car-registrations-in-july/" target="_blank" rel="noopener">Denmark nears 100% EV share for private buyers</a>
        <div class="fp-meta"><span>Score 71</span><span>•</span><span>Aug 4, 2026</span></div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Suppliers & Infrastructure</h3>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/28/tesla-sues-cybertruck-supplier-angstrom-tooling/" target="_blank" rel="noopener">Tesla sues supplier to access Cybertruck tooling</a>
        <div class="fp-meta"><span>Score 73</span><span>•</span><span>Jul 28, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.electrive.com/2026/08/03/edenred-completes-acquisition-of-the-mobility-house-solutions/" target="_blank" rel="noopener">Edenred buys The Mobility House Solutions</a>
        <div class="fp-meta"><span>Score 67</span><span>•</span><span>Aug 3, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://www.electrive.com/2026/08/03/blue-solutions-and-avl-test-solid-state-battery-safety/" target="_blank" rel="noopener">AVL, Blue Solutions test solid‑state safety</a>
        <div class="fp-meta"><span>Score 65</span><span>•</span><span>Aug 3, 2026</span></div>
      </div>
    </div>

    <div class="feature-panel">
      <h3>Trending Topics</h3>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/29/hyundai-reveals-ioniq-3-prices-start-30000-interest-surges/" target="_blank" rel="noopener">Affordable EV wave: Hyundai IONIQ 3 from ~$30k</a>
        <div class="fp-meta"><span>Score 79</span><span>•</span><span>Jul 29, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/07/28/volkswagen-launches-cheaper-id-polo-ev-orders-25000/" target="_blank" rel="noopener">VW opens cheaper ID. Polo after 25k orders</a>
        <div class="fp-meta"><span>Score 72</span><span>•</span><span>Jul 28, 2026</span></div>
      </div>
      <div class="fp-row">
        <a href="https://electrek.co/2026/08/03/byd-opens-denza-z9s-pre-orders-record-1100-km-ev-range/" target="_blank" rel="noopener">BYD Denza Z9S touts 1,100‑km EV range</a>
        <div class="fp-meta"><span>Score 70</span><span>•</span><span>Aug 3, 2026</span></div>
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
    <h2 class="section-title">Latest Articles <span class="count">14 analyzed today</span></h2>
    <div class="article-table">
      
      <div class="article-row">
        <div class="score-chip high">92</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">NHTSA opens probe into 1.2M Tesla Model 3/Y over suspension failures</a>
          <div class="article-take">A potential control‑arm defect puts the nation’s largest EV fleet under immediate safety and cost scrutiny.</div>
          <div class="article-tags">
            <span class="chip">Tesla</span><span class="chip">Safety</span><span class="chip">Regulation</span>
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
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">BMW puts G‑Class rival on hold as China headwinds hit home</a>
          <div class="article-take">Program triage underscores how uneven regional demand is forcing OEMs to revisit capital plans.</div>
          <div class="article-tags">
            <span class="chip">BMW</span><span class="chip">Strategy</span><span class="chip">China</span>
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
          <a class="headline" href="https://electrek.co/2026/08/04/tesla-china-sales-crash-exports-surge-h1-2026/" target="_blank" rel="noopener">Tesla’s China sales drop as exports from Shanghai surge</a>
          <div class="article-take">Pivot to exports keeps lines busy but risks ceding brand momentum in the world’s largest EV market.</div>
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
        <div class="score-chip">84</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Volvo drops lidar on EX90/ES90, pays owner compensation</a>
          <div class="article-take">Strategic sensor shift trims complexity and cost while pressuring lidar suppliers to prove near‑term ROI.</div>
          <div class="article-tags">
            <span class="chip">Volvo</span><span class="chip">ADAS</span><span class="chip">Lidar</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">78</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">SK On and Factorial team up to scale solid‑state batteries</a>
          <div class="article-take">Partnership accelerates path from pilot cells to auto‑grade volumes as OEMs demand clearer timelines.</div>
          <div class="article-tags">
            <span class="chip">SK On</span><span class="chip">Factorial</span><span class="chip">Batteries</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">79</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/hyundai-reveals-ioniq-3-prices-start-30000-interest-surges/" target="_blank" rel="noopener">Hyundai IONIQ 3 starts around $30,000 as demand surges</a>
          <div class="article-take">Lean pricing and 300‑mile range reset expectations for mainstream EV value in 2027 model year.</div>
          <div class="article-tags">
            <span class="chip">Hyundai</span><span class="chip">Pricing</span><span class="chip">EV Adoption</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/hyundai-reveals-ioniq-3-prices-start-30000-interest-surges/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">75</div>
        <div class="article-main">
          <a class="headline" href="https://www.greencarreports.com/news/1146051_gm-pilot-ev-charging-network-now-spans-over-25-states" target="_blank" rel="noopener">GM–Pilot EVgo highway network now spans 25+ states</a>
          <div class="article-take">Planned coast‑to‑coast coverage strengthens NACS transition narrative and road‑trip confidence.</div>
          <div class="article-tags">
            <span class="chip">GM</span><span class="chip">EVgo</span><span class="chip">Charging</span>
          </div>
        </div>
        <div class="article-source">
          <span>Green Car Reports — Aug 3, 2026</span>
          <a href="https://www.greencarreports.com/news/1146051_gm-pilot-ev-charging-network-now-spans-over-25-states" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">70</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/waymo-gemini-ai-ojai-robotaxi-redesigned-interface/" target="_blank" rel="noopener">Waymo integrates Google Gemini and a new rider UI</a>
          <div class="article-take">Sharper guidance and conversational assistance target rider trust as ODD expands.</div>
          <div class="article-tags">
            <span class="chip">Waymo</span><span class="chip">Autonomy</span><span class="chip">UX</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/waymo-gemini-ai-ojai-robotaxi-redesigned-interface/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">77</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/30/rivian-rivn-q2-2026-earnings-r2-deliveries-revenue-up-27/" target="_blank" rel="noopener">Rivian Q2: revenue +27%, record gross profit with R2 launch</a>
          <div class="article-take">Scaling a sub‑$50k model while lifting margins signals credible path off cash burn.</div>
          <div class="article-tags">
            <span class="chip">Rivian</span><span class="chip">Earnings</span><span class="chip">R2</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 30, 2026</span>
          <a href="https://electrek.co/2026/07/30/rivian-rivn-q2-2026-earnings-r2-deliveries-revenue-up-27/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">72</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/reborn-audi-a2-driven-electric-comeback-efficiency-king" target="_blank" rel="noopener">Reborn Audi A2 driven: aero-first EV comeback</a>
          <div class="article-take">VW Group’s compact EV strategy leans on efficiency to deliver range without oversized packs.</div>
          <div class="article-tags">
            <span class="chip">Audi</span><span class="chip">Efficiency</span><span class="chip">Compact EVs</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 1, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/reborn-audi-a2-driven-electric-comeback-efficiency-king" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">73</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/28/tesla-sues-cybertruck-supplier-angstrom-tooling/" target="_blank" rel="noopener">Tesla sues Cybertruck supplier to retrieve critical tooling</a>
          <div class="article-take">Tooling access fight highlights supply risk concentration in low‑volume stainless body panels.</div>
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
          <a class="headline" href="https://electrek.co/2026/08/03/byd-opens-denza-z9s-pre-orders-record-1100-km-ev-range/" target="_blank" rel="noopener">BYD opens Denza Z9S pre‑orders, touts 1,100‑km range</a>
          <div class="article-take">Ultra‑long‑range specs intensify China’s range race and premium push into export markets.</div>
          <div class="article-tags">
            <span class="chip">BYD</span><span class="chip">Premium EV</span><span class="chip">Range</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 3, 2026</span>
          <a href="https://electrek.co/2026/08/03/byd-opens-denza-z9s-pre-orders-record-1100-km-ev-range/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">71</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/denmark-evs-account-for-almost-all-new-car-registrations-in-july/" target="_blank" rel="noopener">Denmark: EVs make up 97% of private new registrations in July</a>
          <div class="article-take">Nordic momentum shows incentives and charging density can flip markets rapidly.</div>
          <div class="article-tags">
            <span class="chip">Denmark</span><span class="chip">Policy</span><span class="chip">Adoption</span>
          </div>
        </div>
        <div class="article-source">
          <span>electrive — Aug 4, 2026</span>
          <a href="https://www.electrive.com/2026/08/04/denmark-evs-account-for-almost-all-new-car-registrations-in-july/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">72</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/28/volkswagen-launches-cheaper-id-polo-ev-orders-25000/" target="_blank" rel="noopener">Volkswagen launches cheaper ID. Polo EV after 25k orders</a>
          <div class="article-take">Smaller pack variant broadens entry pricing and defends share against new low‑cost rivals.</div>
          <div class="article-tags">
            <span class="chip">Volkswagen</span><span class="chip">Pricing</span><span class="chip">Small EVs</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 28, 2026</span>
          <a href="https://electrek.co/2026/07/28/volkswagen-launches-cheaper-id-polo-ev-orders-25000/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">76</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/03/hyundai-kias-record-us-sales-run/" target="_blank" rel="noopener">Hyundai and Kia’s record US sales run shows no signs of slowing</a>
          <div class="article-take">Hybrid‑heavy mix sustains growth while EVs build brand equity and showroom traffic.</div>
          <div class="article-tags">
            <span class="chip">Hyundai</span><span class="chip">Kia</span><span class="chip">Sales</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 3, 2026</span>
          <a href="https://electrek.co/2026/08/03/hyundai-kias-record-us-sales-run/" target="_blank" rel="noopener">Read original →</a>
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
  
  <div class="sec-group" id="manufacturers">
    <h2 class="section-title">OEM Spotlight <span class="count">5 stories</span></h2>
    <div class="article-table">
      
      <div class="article-row">
        <div class="score-chip">82</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home" target="_blank" rel="noopener">BMW pauses hardcore off‑roader amid shifting global demand</a>
          <div class="article-take">Capital discipline trumps halo projects when core markets wobble.</div>
          <div class="article-tags">
            <span class="chip">BMW</span><span class="chip">Strategy</span>
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
          <a class="headline" href="https://electrek.co/2026/08/04/tesla-china-sales-crash-exports-surge-h1-2026/" target="_blank" rel="noopener">Tesla leans on exports as Chinese retail weakens</a>
          <div class="article-take">Protecting factory utilization can cost you home‑market mindshare.</div>
          <div class="article-tags">
            <span class="chip">Tesla</span><span class="chip">China</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 4, 2026</span>
          <a href="https://electrek.co/2026/08/04/tesla-china-sales-crash-exports-surge-h1-2026/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">76</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/03/hyundai-kias-record-us-sales-run/" target="_blank" rel="noopener">Hyundai/Kia notch another record month in US</a>
          <div class="article-take">Balanced powertrain mix cushions consumer uncertainty.</div>
          <div class="article-tags">
            <span class="chip">Hyundai</span><span class="chip">Kia</span><span class="chip">Sales</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 3, 2026</span>
          <a href="https://electrek.co/2026/08/03/hyundai-kias-record-us-sales-run/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">74</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/ferrari-luce-ev-sold-out-2026-allocation/" target="_blank" rel="noopener">Ferrari’s first EV sells out 2026 run in weeks</a>
          <div class="article-take">Ultra‑luxury demand stays price‑inelastic—even for a polarizing design.</div>
          <div class="article-tags">
            <span class="chip">Ferrari</span><span class="chip">Demand</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/ferrari-luce-ev-sold-out-2026-allocation/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">77</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/30/rivian-rivn-q2-2026-earnings-r2-deliveries-revenue-up-27/" target="_blank" rel="noopener">Rivian posts record gross profit on R2 deliveries</a>
          <div class="article-take">Cost‑down curve finally meets volume ambitions.</div>
          <div class="article-tags">
            <span class="chip">Rivian</span><span class="chip">Financials</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 30, 2026</span>
          <a href="https://electrek.co/2026/07/30/rivian-rivn-q2-2026-earnings-r2-deliveries-revenue-up-27/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

    </div>
  </div>

  <div class="sec-group" id="technology">
    <h2 class="section-title">EV &amp; Technology <span class="count">5 stories</span></h2>
    <div class="article-table">
      
      <div class="article-row">
        <div class="score-chip">84</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Volvo axes lidar on two flagships, compensates buyers</a>
          <div class="article-take">A rare public reversal raises questions about near‑term sensor stacks.</div>
          <div class="article-tags">
            <span class="chip">Volvo</span><span class="chip">ADAS</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      
      <div class="article-row">
        <div class="score-chip">78</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">SK On + Factorial push solid‑state scaling</a>
          <div class="article-take">Consortia are replacing moonshots as timetables tighten.</div>
          <div class="article-tags">
            <span class="chip">Batteries</span><span class="chip">Solid‑state</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      
      <div class="article-row">
        <div class="score-chip">72</div>
        <div class="article-main">
          <a class="headline" href="https://www.autocar.co.uk/car-news/new-cars/reborn-audi-a2-driven-electric-comeback-efficiency-king" target="_blank" rel="noopener">Audi’s A2 e‑tron prioritizes aero over battery size</a>
          <div class="article-take">Efficiency becomes the new luxury in compact EV packaging.</div>
          <div class="article-tags">
            <span class="chip">Audi</span><span class="chip">Efficiency</span>
          </div>
        </div>
        <div class="article-source">
          <span>Autocar — Aug 1, 2026</span>
          <a href="https://www.autocar.co.uk/car-news/new-cars/reborn-audi-a2-driven-electric-comeback-efficiency-king" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      
      <div class="article-row">
        <div class="score-chip">70</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/waymo-gemini-ai-ojai-robotaxi-redesigned-interface/" target="_blank" rel="noopener">Waymo debuts Gemini‑powered robotaxi interface</a>
          <div class="article-take">Better explanations and guidance aim to boost AV rider confidence.</div>
          <div class="article-tags">
            <span class="chip">Waymo</span><span class="chip">AI</span><span class="chip">UX</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/waymo-gemini-ai-ojai-robotaxi-redesigned-interface/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      
      <div class="article-row">
        <div class="score-chip">67</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/03/blue-solutions-and-avl-test-solid-state-battery-safety/" target="_blank" rel="noopener">AVL and Blue Solutions validate solid‑state safety</a>
          <div class="article-take">Thermal propagation work readies next‑gen chemistries for series programs.</div>
          <div class="article-tags">
            <span class="chip">AVL</span><span class="chip">Solid‑state</span><span class="chip">Safety</span>
          </div>
        </div>
        <div class="article-source">
          <span>electrive — Aug 3, 2026</span>
          <a href="https://www.electrive.com/2026/08/03/blue-solutions-and-avl-test-solid-state-battery-safety/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

    </div>
  </div>

  <div class="sec-group" id="government">
    <h2 class="section-title">Government &amp; Infrastructure <span class="count">3 stories</span></h2>
    <div class="article-table">
      
      <div class="article-row">
        <div class="score-chip high">92</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">US safety probe into Tesla suspension failures</a>
          <div class="article-take">Regulators escalate scrutiny on the largest EV cohort on US roads.</div>
          <div class="article-tags">
            <span class="chip">NHTSA</span><span class="chip">Tesla</span><span class="chip">Safety</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 31, 2026</span>
          <a href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      
      <div class="article-row">
        <div class="score-chip">75</div>
        <div class="article-main">
          <a class="headline" href="https://www.greencarreports.com/news/1146051_gm-pilot-ev-charging-network-now-spans-over-25-states" target="_blank" rel="noopener">GM–Pilot EVgo buildout crosses half the nation</a>
          <div class="article-take">Highway coverage is the make‑or‑break for EV road trips and fleet routing.</div>
          <div class="article-tags">
            <span class="chip">Charging</span><span class="chip">Infrastructure</span>
          </div>
        </div>
        <div class="article-source">
          <span>Green Car Reports — Aug 3, 2026</span>
          <a href="https://www.greencarreports.com/news/1146051_gm-pilot-ev-charging-network-now-spans-over-25-states" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      
      <div class="article-row">
        <div class="score-chip">71</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/04/denmark-evs-account-for-almost-all-new-car-registrations-in-july/" target="_blank" rel="noopener">Denmark hits 97% EV share among private buyers in July</a>
          <div class="article-take">A preview of policy + product alignment when friction is removed.</div>
          <div class="article-tags">
            <span class="chip">Policy</span><span class="chip">Adoption</span>
          </div>
        </div>
        <div class="article-source">
          <span>electrive — Aug 4, 2026</span>
          <a href="https://www.electrive.com/2026/08/04/denmark-evs-account-for-almost-all-new-car-registrations-in-july/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

    </div>
  </div>

  <div class="sec-group" id="electric-vehicles">
    <h2 class="section-title">EV &amp; Market Intelligence <span class="count">4 stories</span></h2>
    <div class="article-table">
      
      <div class="article-row">
        <div class="score-chip">79</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/hyundai-reveals-ioniq-3-prices-start-30000-interest-surges/" target="_blank" rel="noopener">IONIQ 3 targets $30k buyers with 300‑mile range</a>
          <div class="article-take">Pricing discipline broadens EV addressable market beyond early adopters.</div>
          <div class="article-tags">
            <span class="chip">Hyundai</span><span class="chip">Value EV</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 29, 2026</span>
          <a href="https://electrek.co/2026/07/29/hyundai-reveals-ioniq-3-prices-start-30000-interest-surges/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      
      <div class="article-row">
        <div class="score-chip">72</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/28/volkswagen-launches-cheaper-id-polo-ev-orders-25000/" target="_blank" rel="noopener">VW introduces lower‑priced ID. Polo variant</a>
          <div class="article-take">Small batteries, big volumes: the new European playbook.</div>
          <div class="article-tags">
            <span class="chip">Volkswagen</span><span class="chip">Small EVs</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 28, 2026</span>
          <a href="https://electrek.co/2026/07/28/volkswagen-launches-cheaper-id-polo-ev-orders-25000/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      
      <div class="article-row">
        <div class="score-chip">70</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/08/03/byd-opens-denza-z9s-pre-orders-record-1100-km-ev-range/" target="_blank" rel="noopener">BYD’s Denza raises the ultra‑range stakes</a>
          <div class="article-take">Flagship specs set the tone for premium EV one‑upmanship.</div>
          <div class="article-tags">
            <span class="chip">BYD</span><span class="chip">Premium</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Aug 3, 2026</span>
          <a href="https://electrek.co/2026/08/03/byd-opens-denza-z9s-pre-orders-record-1100-km-ev-range/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      
      <div class="article-row">
        <div class="score-chip">77</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/30/rivian-rivn-q2-2026-earnings-r2-deliveries-revenue-up-27/" target="_blank" rel="noopener">Rivian’s improving unit economics with R2</a>
          <div class="article-take">Mid‑priced EVs can be margin‑accretive with the right scale curve.</div>
          <div class="article-tags">
            <span class="chip">Rivian</span><span class="chip">Margins</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 30, 2026</span>
          <a href="https://electrek.co/2026/07/30/rivian-rivn-q2-2026-earnings-r2-deliveries-revenue-up-27/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

    </div>
  </div>

  <div class="sec-group" id="suppliers">
    <h2 class="section-title">Suppliers <span class="count">3 stories</span></h2>
    <div class="article-table">
      
      <div class="article-row">
        <div class="score-chip">78</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/29/solid-state-ev-battery-leaders-team-up/" target="_blank" rel="noopener">SK On &amp; Factorial ally on solid‑state scaling</a>
          <div class="article-take">Cell makers consolidate to hit OEM timelines and yield targets.</div>
          <div class="article-tags">
            <span class="chip">SK On</span><span class="chip">Factorial</span>
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
          <a class="headline" href="https://electrek.co/2026/07/28/tesla-sues-cybertruck-supplier-angstrom-tooling/" target="_blank" rel="noopener">Tooling standoff exposes fragility in specialized parts</a>
          <div class="article-take">Niche dies can bottleneck entire model lines when suppliers exit.</div>
          <div class="article-tags">
            <span class="chip">Tesla</span><span class="chip">Suppliers</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 28, 2026</span>
          <a href="https://electrek.co/2026/07/28/tesla-sues-cybertruck-supplier-angstrom-tooling/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">67</div>
        <div class="article-main">
          <a class="headline" href="https://www.electrive.com/2026/08/03/edenred-completes-acquisition-of-the-mobility-house-solutions/" target="_blank" rel="noopener">Edenred acquires The Mobility House Solutions</a>
          <div class="article-take">Fleet electrification consolidates around turnkey charging + energy services.</div>
          <div class="article-tags">
            <span class="chip">Edenred</span><span class="chip">Charging</span>
          </div>
        </div>
        <div class="article-source">
          <span>electrive — Aug 3, 2026</span>
          <a href="https://www.electrive.com/2026/08/03/edenred-completes-acquisition-of-the-mobility-house-solutions/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

    </div>
  </div>

  <div class="sec-group" id="finance">
    <h2 class="section-title">Industry News <span class="count">3 stories</span></h2>
    <div class="article-table">
      
      <div class="article-row">
        <div class="score-chip high">92</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">US safety probe hits Tesla’s core volumes</a>
          <div class="article-take">Potential recall liabilities can ripple through warranty reserves and resale values.</div>
          <div class="article-tags">
            <span class="chip">Safety</span><span class="chip">Regulatory</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 31, 2026</span>
          <a href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>
      
      <div class="article-row">
        <div class="score-chip">77</div>
        <div class="article-main">
          <a class="headline" href="https://electrek.co/2026/07/30/rivian-rivn-q2-2026-earnings-r2-deliveries-revenue-up-27/" target="_blank" rel="noopener">Rivian reports stronger Q2 and margin trajectory</a>
          <div class="article-take">Investors reward proof of scalable, mid‑price EV economics.</div>
          <div class="article-tags">
            <span class="chip">Earnings</span><span class="chip">EV Economics</span>
          </div>
        </div>
        <div class="article-source">
          <span>Electrek — Jul 30, 2026</span>
          <a href="https://electrek.co/2026/07/30/rivian-rivn-q2-2026-earnings-r2-deliveries-revenue-up-27/" target="_blank" rel="noopener">Read original →</a>
        </div>
      </div>

      <div class="article-row">
        <div class="score-chip">75</div>
        <div class="article-main">
          <a class="headline" href="https://www.greencarreports.com/news/1146051_gm-pilot-ev-charging-network-now-spans-over-25-states" target="_blank" rel="noopener">GM–Pilot–EVgo push accelerates DCFC availability</a>
          <div class="article-take">Network density is becoming a competitive pillar alongside product.</div>
          <div class="article-tags">
            <span class="chip">Infrastructure</span><span class="chip">Charging</span>
          </div>
        </div>
        <div class="article-source">
          <span>Green Car Reports — Aug 3, 2026</span>
          <a href="https://www.greencarreports.com/news/1146051_gm-pilot-ev-charging-network-now-spans-over-25-states" target="_blank" rel="noopener">Read original →</a>
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