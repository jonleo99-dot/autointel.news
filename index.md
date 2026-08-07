<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width,initial-scale=1">
<meta name="description" content="AutoIntel Intelligence is being upgraded. Check back soon for scored, structured automotive industry intelligence.">
<meta property="og:title" content="AutoIntel Intelligence — Under Construction">
<meta property="og:description" content="We're upgrading the signal. Back shortly.">
<meta property="og:type" content="website">
<meta property="og:url" content="https://autointel.news">
<meta name="twitter:card" content="summary_large_image">
<title>AutoIntel Intelligence — Under Construction</title>
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
html,body{margin:0;height:100%}
body{
  background:var(--bg);
  color:var(--ink);
  font-family:'IBM Plex Sans',Arial,sans-serif;
  font-size:15px;
  line-height:1.6;
  min-height:100%;
  display:flex;
  flex-direction:column;
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
  flex:none;
}
.ticker-track{
  display:inline-flex;
  gap:36px;
  padding-left:36px;
  animation:tickerScroll 30s linear infinite;
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
.ticker-item b{color:var(--amber);font-weight:500}
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
  flex:none;
}
.masthead-row{
  max-width:1320px;
  margin:0 auto;
  padding:18px 24px;
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

/* ---------------- Main construction panel ---------------- */
main{
  flex:1;
  display:flex;
  align-items:center;
  justify-content:center;
  padding:48px 24px;
}
.construct-card{
  width:100%;
  max-width:640px;
  background:var(--panel);
  border:1px solid var(--line);
  border-radius:14px;
  padding:44px 40px 40px;
  text-align:center;
}
.eyebrow{
  font-family:'IBM Plex Mono',monospace;
  font-size:11px;
  letter-spacing:0.14em;
  color:var(--amber);
  display:inline-flex;
  align-items:center;
  gap:8px;
  margin-bottom:20px;
}
.eyebrow .dot{
  width:7px;height:7px;border-radius:50%;
  background:var(--amber);
  display:inline-block;
  animation:pulse 1.6s ease-in-out infinite;
}
@keyframes pulse{
  0%,100%{opacity:1}
  50%{opacity:.3}
}

.gauge-wrap{margin:0 auto 28px;width:150px}
.gauge{
  background:var(--panel-2);
  border:1px solid var(--line);
  border-radius:10px;
  padding:16px 12px 12px;
}
.gauge svg{width:100%;max-width:110px;height:auto;display:block;margin:0 auto}
.gauge-value{
  font-family:'IBM Plex Mono',monospace;
  font-size:20px;
  font-weight:600;
  margin-top:-30px;
  display:block;
  color:#fff;
}
.gauge-label{
  font-family:'IBM Plex Mono',monospace;
  font-size:9.5px;
  letter-spacing:0.08em;
  color:var(--ink-dim);
  text-transform:uppercase;
  display:block;
  margin-top:4px;
}

h1{
  font-size:28px;
  line-height:1.3;
  margin-bottom:14px;
}
.dek{
  color:var(--ink-dim);
  font-size:14.5px;
  max-width:44ch;
  margin:0 auto 28px;
}

.chip-row{display:flex;flex-wrap:wrap;gap:8px;justify-content:center;margin-bottom:32px}
.chip{
  font-family:'IBM Plex Mono',monospace;
  font-size:11px;
  padding:6px 12px;
  border-radius:999px;
  background:var(--panel-2);
  border:1px solid var(--line);
  color:var(--ink-dim);
  white-space:nowrap;
}
.chip.entity-mfr{border-color:#3a4a3f;color:var(--teal)}

.notify-row{
  display:flex;
  gap:10px;
  max-width:380px;
  margin:0 auto;
  flex-wrap:wrap;
  justify-content:center;
}
.notify-row input{
  flex:1;
  min-width:180px;
  background:var(--panel-2);
  border:1px solid var(--line);
  color:var(--ink);
  border-radius:8px;
  padding:11px 14px;
  font-family:'IBM Plex Sans',sans-serif;
  font-size:13.5px;
}
.notify-row input::placeholder{color:var(--slate)}
.notify-row input:focus{outline:none;border-color:var(--amber)}
.notify-row button{
  background:var(--amber);
  color:#14171c;
  border:none;
  border-radius:8px;
  padding:11px 20px;
  font-family:'IBM Plex Mono',monospace;
  font-size:12.5px;
  font-weight:600;
  letter-spacing:0.03em;
  cursor:pointer;
  transition:background .15s ease;
}
.notify-row button:hover{background:#ffb84f}

.progress-line{
  margin-top:32px;
  padding-top:24px;
  border-top:1px solid var(--line);
  display:flex;
  align-items:center;
  justify-content:center;
  gap:10px;
  font-family:'IBM Plex Mono',monospace;
  font-size:11px;
  color:var(--ink-dim);
  letter-spacing:0.04em;
}
.progress-track{
  width:140px;
  height:4px;
  background:var(--panel-2);
  border-radius:3px;
  overflow:hidden;
  border:1px solid var(--line);
}
.progress-fill{
  width:64%;
  height:100%;
  background:var(--teal);
  border-radius:3px;
}

footer{
  flex:none;
  text-align:center;
  padding:20px 24px 28px;
  font-family:'IBM Plex Mono',monospace;
  font-size:11px;
  color:var(--slate);
  letter-spacing:0.03em;
}

@media(max-width:480px){
  .construct-card{padding:32px 22px 28px}
  h1{font-size:22px}
}
</style>
</head>
<body>

<div class="ticker" aria-label="Status">
  <div class="ticker-track" id="tickerTrack">
    <span class="ticker-item"><b>STATUS</b> Scheduled maintenance in progress</span>
    <span class="ticker-item"><b>ETA</b> Back online shortly</span>
    <span class="ticker-item"><b>DATA</b> No signal lost — feeds resume on restore</span>
  </div>
</div>

<header class="masthead">
  <div class="masthead-row">
    <div class="wordmark">AutoIntel<span class="wordmark-sub">INTELLIGENCE</span></div>
    <div class="masthead-date mono" id="publishDate"></div>
  </div>
</header>

<main>
  <div class="construct-card">
    <span class="eyebrow"><span class="dot"></span>UNDER CONSTRUCTION</span>

    <div class="gauge-wrap">
      <div class="gauge">
        <svg viewBox="0 0 120 70"><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#2a3038" stroke-width="8"/><path d="M10,65 A50,50 0 0 1 110,65" fill="none" stroke="#f2a93b" stroke-width="8" stroke-dasharray="157" stroke-dashoffset="55"/></svg>
        <span class="gauge-value mono">64%</span>
        <span class="gauge-label">Build Progress</span>
      </div>
    </div>

    <h1>We're upgrading the signal.</h1>
    <p class="dek">AutoIntel Intelligence is offline for scheduled improvements. We'll be back with sharper data and a faster read shortly.</p>

    <div class="chip-row">
      <span class="chip entity-mfr">Entity Data</span>
      <span class="chip">Scoring Engine</span>
      <span class="chip">Source Attribution</span>
    </div>

    <form class="notify-row" onsubmit="return false;">
      <input type="email" placeholder="you@email.com" aria-label="Email address">
      <button type="submit">Notify Me</button>
    </form>

    <div class="progress-line">
      <span>REBUILDING</span>
      <span class="progress-track"><span class="progress-fill"></span></span>
    </div>
  </div>
</main>

<footer>
  &copy; <span id="year"></span> AutoIntel Intelligence — automotive industry signal, daily.
</footer>

<script>
document.getElementById('publishDate').textContent = new Date().toLocaleDateString('en-US',{weekday:'long',year:'numeric',month:'long',day:'numeric'}).toUpperCase();
document.getElementById('year').textContent = new Date().getFullYear();

(function(){
  var track = document.getElementById('tickerTrack');
  if (track) track.innerHTML += track.innerHTML;
})();
</script>

</body>
</html>
