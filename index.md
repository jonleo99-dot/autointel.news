<!doctype html>
<html lang="en">
<head>
<meta charset='utf-8'>
<meta name='viewport' content='width=device-width,initial-scale=1'>
<meta name='description' content='AutoIntel.News delivers daily automotive industry intelligence, revealing market contradictions and tensions that shape the future of cars, trucks, and mobility.'>
<meta name='keywords' content='automotive news, EV market, car industry, dealership intelligence, OEM strategy, market analysis'>
<meta property='og:title' content='AutoIntel.News - Automotive Intelligence. Curated Daily.'>
<meta property='og:description' content='Revealing market contradictions behind automotive headlines. B2B focused intelligence for dealership GMs, OEMs, and fleet operators.'>
<meta property='og:type' content='website'>
<meta property='og:url' content='https://autointel.news'>
<meta name='twitter:card' content='summary_large_image'>
<meta name='twitter:title' content='AutoIntel.News - Automotive Intelligence. Curated Daily.'>
<meta name='twitter:description' content='Revealing market contradictions behind automotive headlines.'>
<title>AutoIntel.News - Automotive Intelligence. Curated Daily.</title>
<style>
body{
  margin:0;
  background:#0f0f10;
  color:#eee;
  font-family:Arial,sans-serif;
  font-size:16px;
  line-height:1.6
}
header{
  padding:40px;
  text-align:center;
  background:#171717;
  border-bottom:4px solid #f60
}
.scroll-top-bar{
  position:fixed;
  top:0;
  left:0;
  right:0;
  z-index:1000;
  background:#171717;
  border-bottom:2px solid #f60;
  padding:10px 16px;
  display:flex;
  align-items:center;
  justify-content:center;
  gap:8px;
  cursor:pointer;
  transform:translateY(-100%);
  transition:transform 0.25s ease;
  font-size:13px;
  letter-spacing:1px;
  color:#eee
}
.scroll-top-bar.is-visible{
  transform:translateY(0)
}
.scroll-top-bar .car-symbol{
  font-family:Times,'Times New Roman',serif;
  color:#f60;
  font-style:italic;
  font-size:15px
}
.scroll-top-bar span:last-child{
  font-weight:bold
}
@media(prefers-reduced-motion:reduce){
  .scroll-top-bar{
    transition:none
  }
}
.date-field{
  color:#aaa;
  font-size:12px;
  letter-spacing:1px;
  text-transform:uppercase;
  margin-bottom:15px
}
header h1{
  margin:0 0 10px 0;
  font-size:45px;
  letter-spacing:2px;
  font-weight:700;
  font-family:'Noticia Text',serif;
  font-style:normal
}
header h1 .car-symbol{
  font-style:italic
}
header p{
  margin:10px 0 0 0;
  font-size:14px;
  color:#ccc;
  max-width:900px;
  margin-left:auto;
  margin-right:auto;
  line-height:1.6
}
.tagline{
  color:#aaa;
  font-size:14px;
  margin:15px 0 20px 0
}
.stats-bar{
  text-align:center;
  padding:20px;
  margin:0 0 20px 0;
  border-bottom:1px solid #2a2a2a;
  background:#0f0f10
}
.stat{
  display:inline-block;
  margin:0 20px;
  font-weight:bold;
  color:#f60;
  font-size:14px
}
.wrap{
  max-width:1400px;
  margin:auto;
  padding:24px
}
.hero{
  overflow:hidden;
  border-radius:14px;
  background:#1b1b1b;
  margin-bottom:40px;
  box-shadow:0 4px 12px rgba(0,0,0,0.3)
}
.hero img{
  width:100%;
  height:420px;
  object-fit:cover;
  display:block
}
.hero-content{
  padding:32px
}
.hero-content h2{
  margin:0 0 15px 0;
  font-size:32px;
  line-height:1.3;
  color:#fff
}
.hero-content h2 a:hover{
  text-decoration:underline
}
.hero-content p{
  margin:0 0 12px 0;
  font-size:16px;
  color:#ccc;
  line-height:1.6
}
.hero-tension{
  margin:15px 0 0 0;
  padding-top:15px;
  border-top:1px solid #f60;
  font-size:13px;
  color:#f60;
  font-style:italic;
  line-height:1.5
}
.badge{
  background:#f60;
  color:#fff;
  padding:6px 12px;
  border-radius:999px;
  font-size:11px;
  font-weight:bold;
  display:inline-block;
  margin-bottom:15px;
  letter-spacing:0.5px
}
.sec{
  margin:48px 0 32px 0;
  padding:24px;
  background:#1b1b1b;
  border-left:5px solid #f60;
  border-radius:8px
}
.sec h2{
  margin:0 0 8px 0;
  font-size:22px;
  color:#fff
}
.sec small{
  color:#aaa;
  font-size:13px
}
.grid{
  display:grid;
  grid-template-columns:repeat(auto-fit,minmax(280px,1fr));
  gap:20px;
  margin-bottom:40px
}
.card{
  background:#1b1b1b;
  border-radius:12px;
  overflow:hidden;
  transition:all 0.3s ease;
  border:1px solid #2a2a2a;
  display:flex;
  flex-direction:column;
  height:100%
}
.card:hover{
  transform:translateY(-5px);
  border-color:#f60;
  box-shadow:0 8px 24px rgba(255,102,0,0.2)
}
.card img{
  width:100%;
  height:200px;
  object-fit:cover;
  display:block
}
.card-content{
  padding:18px;
  flex-grow:1;
  display:flex;
  flex-direction:column
}
.card-content .badge{
  margin:0 0 12px 0;
  font-size:10px;
  width:110px;
  padding:6px 4px;
  box-sizing:border-box;
  text-align:center;
  white-space:nowrap;
  overflow:hidden;
  text-overflow:ellipsis
}
.card-content h3{
  margin:0 0 10px 0;
  font-size:15px;
  line-height:1.4;
  color:#fff
}
.card-content p{
  margin:0 0 10px 0;
  font-size:13px;
  color:#aaa;
  line-height:1.5
}
.card-tension{
  font-size:12px;
  color:#f60;
  font-style:italic;
  line-height:1.4;
  padding-top:8px;
  border-top:1px solid #2a2a2a
}
.card-content small{
  display:block;
  margin-top:auto;
  padding-top:8px;
  font-size:11px;
  color:#666;
  border-top:1px solid #2a2a2a
}
.toc-filter-row{
  display:flex;
  justify-content:space-between;
  align-items:center;
  flex-wrap:wrap;
  gap:12px 20px;
  padding:14px 20px;
  border-bottom:1px solid #2a2a2a;
  background:#0f0f10;
  font-size:13px
}
.toc-links{
  color:#ccc;
  line-height:1.8
}
.toc-links a{
  margin:0 2px
}
.filter-bar{
  display:flex;
  align-items:center;
  flex-wrap:wrap;
  gap:8px
}
.filter-label{
  color:#888;
  font-size:12px;
  text-transform:uppercase;
  letter-spacing:0.5px;
  margin-right:10px
}
.filter-select{
  background:#1b1b1b;
  border:1px solid #2a2a2a;
  color:#eee;
  padding:8px 32px 8px 14px;
  border-radius:8px;
  font-size:13px;
  font-family:Arial,sans-serif;
  cursor:pointer;
  appearance:none;
  -webkit-appearance:none;
  -moz-appearance:none;
  background-image:url("data:image/svg+xml;utf8,<svg xmlns='http://www.w3.org/2000/svg' width='10' height='6'><path d='M0 0l5 6 5-6z' fill='%23f60'/></svg>");
  background-repeat:no-repeat;
  background-position:right 12px center
}
.filter-select:hover{
  border-color:#f60
}
.filter-select:focus{
  outline:none;
  border-color:#f60
}
.sec-group.is-hidden,
.hero.is-hidden,
.card.is-hidden{
  display:none
}
a{
  text-decoration:none;
  color:inherit
}
.card a{
  display:flex;
  flex-direction:column;
  height:100%
}
footer{
  text-align:center;
  padding:40px;
  border-top:1px solid #2a2a2a;
  color:#666;
  font-size:13px;
  margin-top:60px
}
footer p{
  margin:10px 0
}
@media(max-width:768px){
  header{padding:20px}
  header h1{font-size:32px}
  .hero img{height:280px}
  .hero-content{padding:20px}
  .grid{grid-template-columns:1fr}
  .stat{display:block;margin:10px 0}
  .toc-filter-row{flex-direction:column;align-items:flex-start}
}
.reveal{
  opacity:0;
  transform:translateY(24px);
  transition:opacity 0.6s ease, transform 0.6s ease
}
.reveal.is-visible{
  opacity:1;
  transform:translateY(0)
}
@media(prefers-reduced-motion:reduce){
  .reveal{
    opacity:1;
    transform:none;
    transition:none
  }
}
</style>
<!-- Google tag (gtag.js) -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-GFL6J09QZV"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-GFL6J09QZV');
</script>
</head>
<body>
<div class="scroll-top-bar" id="scrollTopBar" role="button" tabindex="0" aria-label="Scroll back to top">
  <span>AutoIntel.News</span>
  <span class="car-symbol">ō͡≡o˞̶</span>
</div>

<header>
  <div class='date-field' id='publishDate'></div>
  <h1>AutoIntel.News <span class='car-symbol' style="color:#f60;font-family:Times,'Times New Roman',serif">ō͡≡o˞̶</span></h1>
  <p class='tagline'>Automotive Intelligence. Curated Daily.</p>
</header>

<div class='stats-bar'>
  <span class='stat'><span class="stat-num" data-target="37">0</span> Stories</span>
  <span class='stat'><span class="stat-num" data-target="4">0</span> Publishers</span>
  <span class='stat'>~<span class="stat-num" data-target="14">0</span> min read</span>
</div>

<div class="toc-filter-row" id="tocFilterRow">
  <div class="toc-links"><span style='color:#888'>Jump to: </span><a href="#oem-spotlight">OEM Spotlight</a> &nbsp;|&nbsp; <a href="#market-intelligence">Market Intelligence</a> &nbsp;|&nbsp; <a href="#ev-technology">EV & Technology</a> &nbsp;|&nbsp; <a href="#motorsports">Motorsports</a> &nbsp;|&nbsp; <a href="#performance-builds">Performance Builds</a> &nbsp;|&nbsp; <a href="#suppliers">Suppliers</a> &nbsp;|&nbsp; <a href="#dealer-news">Dealer News</a> &nbsp;|&nbsp; <a href="#industry-news">Industry News</a></div>
  <div class="filter-bar" id="mfrFilterBar">
    <label class="filter-label" for="mfrFilterSelect">Filter by manufacturer:</label>
    <select class="filter-select" id="mfrFilterSelect">
      <option value="__all__">All Manufacturers</option>
      <option value="Alfa Romeo">Alfa Romeo</option>
      <option value="Audi">Audi</option>
      <option value="BMW">BMW</option>
      <option value="BYD">BYD</option>
      <option value="Cadillac">Cadillac</option>
      <option value="DS">DS</option>
      <option value="Ferrari">Ferrari</option>
      <option value="Geely">Geely</option>
      <option value="Genesis">Genesis</option>
      <option value="Hennessey">Hennessey</option>
      <option value="Hyundai">Hyundai</option>
      <option value="Infiniti">Infiniti</option>
      <option value="Jaguar Land Rover">Jaguar Land Rover</option>
      <option value="Kia">Kia</option>
      <option value="Lamborghini">Lamborghini</option>
      <option value="Land Rover">Land Rover</option>
      <option value="Mercedes-Benz">Mercedes-Benz</option>
      <option value="Rivian">Rivian</option>
      <option value="Tesla">Tesla</option>
      <option value="Toyota">Toyota</option>
      <option value="Volvo">Volvo</option>
      <option value="Waymo">Waymo</option>
    </select>
  </div>
</div>

<div class='wrap'>

<p><b>Today's Drive:</b> China's slowdown is reshaping product roadmaps at BMW and beyond, hybrids keep outperforming pure EVs on the sales floor at Hyundai and Toyota, and a wave of flagship launches from Genesis, Audi and Mercedes shows the large-luxury-SUV fight is far from settled.</p>

<!-- Hero Story -->
<div class='hero reveal' data-mfr='BMW'>
  <img src='https://placehold.co/800x450/1b1b1b/f60?text=AutoIntel.News' alt="Hero Story">
  <div class='hero-content'>
    <span class='badge'>FEATURE STORY</span>
    <h2><a href='https://www.autocar.co.uk/car-news/new-cars/bmw-puts-g-class-rival-hold-china-headwinds-hit-home' target='_blank' rel='noopener'>BMW Puts Its G-Class Rival On Hold As China Headwinds Hit Home</a></h2>
    <p>BMW has shelved its G74 off-roader, the long-planned rival to the Mercedes-Benz G-Class, as new CEO Milan Nedeljkovic reworks the company's product roadmap in response to what he calls a "dramatic shift" in global demand. The review follows a weaker-than-expected second quarter, with China's rapid slowdown cited as the main reason BMW cut its full-year guidance in June. Nedeljkovic says BMW is reassessing which technologies, model variants and drivetrains it will actually need, rather than assuming every planned program still fits a market that has moved. The company is still touting strong demand for the iX3 and i3, and remains committed to selling combustion, hybrid, electric and hydrogen models side by side rather than picking one path.</p>
    <div class='hero-tension'><b>The Tension:</b> BMW keeps talking up strong iX3 and i3 order books, but the same leadership team that trumpets that momentum has just quietly shelved a fully developed flagship program — proof that even well-funded product bets aren't safe from China's slowdown.</div>
  </div>
</div>

<!-- Sections will be populated here. Each section's header+grid must be wrapped in a -->
<!-- <div class="sec-group" id="{slug}"> matching the TOC anchor. Each <div class="card"> -->
<!-- must carry data-mfr="Manufacturer1|Manufacturer2" (pipe-separated, empty string if none) -->
<!-- so the manufacturer filter script below can show/hide it. -->
<div class="sec-group" id="oem-spotlight">
  <div class="sec">
    <h2>OEM Spotlight</h2>
    <small>6 stories</small>
  </div>
  <div class="grid">
      <div class="card reveal" data-mfr="Genesis">
        <a href="https://www.motor1.com/news/803622/genesis-gv90-debut-in-august/" target="_blank" rel="noopener">
          <img src="https://placehold.co/800x450/1b1b1b/f60?text=AutoIntel.News" alt="Genesis' New Flagship SUV Could Show Up This Month">
          <div class="card-content">
            <span class="badge">OEM SPOTLIGHT</span>
            <h3>Genesis' New Flagship SUV Could Show Up This Month</h3>
            <p>Genesis is expected to unveil the GV90, its new full-size flagship SUV, as soon as this month. The GV90 is positioned to sit above the existing GV80 and push the brand further into the large-luxury-SUV segment currently dominated by established German and American nameplates.</p>
            <div class="card-tension"><b>The Tension:</b> A flagship SUV launch is exactly the kind of halo product dealers want on the lot — the open question is whether Genesis can build brand pull at the price point large luxury SUVs command.</div>
            <small>motor1.com</small>
          </div>
        </a>
      </div>
      <div class="card reveal" data-mfr="Hyundai">
        <a href="https://electrek.co/2026/08/03/hyundai-40000-ioniq-3-evs-2027/" target="_blank" rel="noopener">
          <img src="https://placehold.co/800x450/1b1b1b/f60?text=AutoIntel.News" alt="Hyundai Plans To Sell Over 40,000 IONIQ 3 Units In 2027">
          <div class="card-content">
            <span class="badge">OEM SPOTLIGHT</span>
            <h3>Hyundai Plans To Sell Over 40,000 IONIQ 3 Units In 2027</h3>
            <p>Hyundai is preparing to open orders on the IONIQ 3 through the second half of 2026, with mass production set to begin in mid-August. The company is targeting more than 40,000 units sold in 2027, a volume goal that puts the IONIQ 3 squarely in Hyundai's mainstream EV lineup rather than a low-volume halo model.</p>
            <div class="card-tension"><b>The Tension:</b> 40,000 units is a mainstream-volume bet on a segment where EV demand has been uneven — Hyundai is wagering price and availability can do what range and tech alone haven't.</div>
            <small>electrek.co</small>
          </div>
        </a>
      </div>
      <div class="card reveal" data-mfr="Mercedes-Benz">
        <a href="https://electrek.co/2026/07/28/mercedes-new-gla-ev-leaks-day-ahead-of-debut/" target="_blank" rel="noopener">
          <img src="https://placehold.co/800x450/1b1b1b/f60?text=AutoIntel.News" alt="Mercedes' New GLA EV Leaks A Day Ahead Of Its Official Debut">
          <div class="card-content">
            <span class="badge">OEM SPOTLIGHT</span>
            <h3>Mercedes' New GLA EV Leaks A Day Ahead Of Its Official Debut</h3>
            <p>The first image of the all-new, electric GLA — Mercedes-Benz's smallest and most affordable SUV — leaked online a day before its scheduled official debut on July 29. The GLA EV is central to Mercedes' push into the compact electric segment where it faces growing pressure from cheaper Chinese entrants.</p>
            <div class="card-tension"><b>The Tension:</b> Losing control of your own reveal narrative a day early is a small thing on its own, but it's a reminder of how little margin OEMs have left to manage the story on flagship affordable-EV launches.</div>
            <small>electrek.co</small>
          </div>
        </a>
      </div>
      <div class="card reveal" data-mfr="Audi">
        <a href="https://www.autocar.co.uk/car-news/new-cars/audi-q9-suv-revealed-huge-%C2%A3100k-a8-successor" target="_blank" rel="noopener">
          <img src="https://placehold.co/800x450/1b1b1b/f60?text=AutoIntel.News" alt="Audi Reveals The Q9, A Huge £100k Rival To The X7 And GLS">
          <div class="card-content">
            <span class="badge">OEM SPOTLIGHT</span>
            <h3>Audi Reveals The Q9, A Huge £100k Rival To The X7 And GLS</h3>
            <p>Audi has revealed the Q9, a massive SUV the brand describes as "unapologetically high-status" and positions as an indirect successor to the A8 saloon. At 5.3m long, 2.2m wide and 1.8m tall, the Q9 is larger than both the BMW X7 and Mercedes GLS it's built to rival, and was developed primarily for the North American and Middle Eastern markets.</p>
            <div class="card-tension"><b>The Tension:</b> Audi is betting its flagship-SUV future on markets outside its European home turf — a tacit admission that the segment that matters most now sits in North America and the Gulf, not Ingolstadt.</div>
            <small>autocar.co.uk</small>
          </div>
        </a>
      </div>
      <div class="card reveal" data-mfr="BMW">
        <a href="https://electrek.co/2026/07/27/bmw-ix5-lwb-debuts-620-miles-range-huge-screens-images/" target="_blank" rel="noopener">
          <img src="https://placehold.co/800x450/1b1b1b/f60?text=AutoIntel.News" alt="BMW's iX5 Long Wheelbase Debuts In China With 620+ Mile Range">
          <div class="card-content">
            <span class="badge">OEM SPOTLIGHT</span>
            <h3>BMW's iX5 Long Wheelbase Debuts In China With 620+ Mile Range</h3>
            <p>BMW introduced the iX5 Long Wheelbase in China, rated at over 620 miles (1,000 km) of CLTC range and built around a cabin dominated by digital screens, including a large "Theater Screen." The China-first, long-wheelbase treatment signals how central that market remains to BMW's EV strategy even as the company pulls back elsewhere.</p>
            <div class="card-tension"><b>The Tension:</b> BMW is simultaneously shelving future SUV programs over China weakness and building this market-specific flagship EV for China first — the same market is both the problem and where the newest metal is landing.</div>
            <small>electrek.co</small>
          </div>
        </a>
      </div>
      <div class="card reveal" data-mfr="Kia|Hyundai">
        <a href="https://electrek.co/2026/07/28/kias-vehicles-smart-upgrade-2027/" target="_blank" rel="noopener">
          <img src="https://placehold.co/800x450/1b1b1b/f60?text=AutoIntel.News" alt="Kia's Vehicles Get A Hyundai-Developed Smart Upgrade Starting 2027">
          <div class="card-content">
            <span class="badge">OEM SPOTLIGHT</span>
            <h3>Kia's Vehicles Get A Hyundai-Developed Smart Upgrade Starting 2027</h3>
            <p>Starting next year, Kia will begin launching vehicles equipped with Hyundai's new high-tech infotainment system, sharing software architecture across the Hyundai Motor Group rather than developing separate systems for each brand.</p>
            <div class="card-tension"><b>The Tension:</b> Shared software cuts R&D cost, but it also narrows one of the few remaining ways Kia can differentiate itself from its corporate sibling in the cabin.</div>
            <small>electrek.co</small>
          </div>
        </a>
      </div>
  </div>
</div>

<div class="sec-group" id="market-intelligence">
  <div class="sec">
    <h2>Market Intelligence</h2>
    <small>6 stories</small>
  </div>
  <div class="grid">
      <div class="card reveal" data-mfr="Hyundai">
        <a href="https://www.motor1.com/news/803621/hyundai-july-2026-record-sales-results/" target="_blank" rel="noopener">
          <img src="https://placehold.co/800x450/1b1b1b/f60?text=AutoIntel.News" alt="Hyundai Posts Another Record Sales Month On Hybrid Strength">
          <div class="card-content">
            <span class="badge">MARKET INTELLIGENCE</span>
            <h3>Hyundai Posts Another Record Sales Month On Hybrid Strength</h3>
            <p>Hyundai's hybrid sales surged 35 percent in July, led by the Tucson and Sonata, driving another record sales month for the brand. The results reinforce hybrids as Hyundai's most reliable growth lever in a market where pure-EV demand has been inconsistent.</p>
            <div class="card-tension"><b>The Tension:</b> While much of the industry chases EV volume targets, Hyundai's best numbers are coming from hybrids — a reminder that the transition plan on paper and the transition actually happening on lots aren't the same thing.</div>
            <small>motor1.com</small>
          </div>
        </a>
      </div>
      <div class="card reveal" data-mfr="Rivian">
        <a href="https://electrek.co/2026/07/30/rivian-rivn-q2-2026-earnings-r2-deliveries-revenue-up-27/" target="_blank" rel="noopener">
          <img src="https://placehold.co/800x450/1b1b1b/f60?text=AutoIntel.News" alt="Rivian's Q2 2026 Revenue Jumps 27% As R2 Deliveries Begin">
          <div class="card-content">
            <span class="badge">MARKET INTELLIGENCE</span>
            <h3>Rivian's Q2 2026 Revenue Jumps 27% As R2 Deliveries Begin</h3>
            <p>Rivian's second-quarter 2026 results showed revenue of $1.658 billion, up 27% year-over-year, alongside a record $179 million gross profit, beating Wall Street on revenue, earnings and adjusted EBITDA. The quarter also marked the start of deliveries for the R2, Rivian's first vehicle priced under $50,000, which began reaching customers on June 9.</p>
            <div class="card-tension"><b>The Tension:</b> Rivian's first profitable-margin quarter arrives on the back of its cheapest vehicle yet — evidence that the path to sustainable EV economics runs through lower price points, not higher ones.</div>
            <small>electrek.co</small>
          </div>
        </a>
      </div>
      <div class="card reveal" data-mfr="">
        <a href="https://electrek.co/2026/07/29/477795/" target="_blank" rel="noopener">
          <img src="https://placehold.co/800x450/1b1b1b/f60?text=AutoIntel.News" alt="Global EV Sales Jump 35% In Q2, With Records In 50 Countries">
          <div class="card-content">
            <span class="badge">MARKET INTELLIGENCE</span>
            <h3>Global EV Sales Jump 35% In Q2, With Records In 50 Countries</h3>
            <p>Global EV sales rebounded sharply in the second quarter, up 35% from a soft start to the year, with 50 countries setting quarterly sales records according to IEA data. The rebound suggests the early-2026 slowdown was more of a pause than a reversal in the broader EV growth trend.</p>
            <div class="card-tension"><b>The Tension:</b> A single quarter's rebound is being read by some as proof the EV transition is back on track, but the record-setting countries and the ones still stalling out are rarely the same ones — global averages can mask very uneven regional reality.</div>
            <small>electrek.co</small>
          </div>
        </a>
      </div>
      <div class="card reveal" data-mfr="Toyota">
        <a href="https://www.carscoops.com/2026/08/toyota-tacoma-tundra-airbag-recall/" target="_blank" rel="noopener">
          <img src="https://placehold.co/800x450/1b1b1b/f60?text=AutoIntel.News" alt="Toyota Recalls Airbags That Were Never Even In Its Trucks">
          <div class="card-content">
            <span class="badge">MARKET INTELLIGENCE</span>
            <h3>Toyota Recalls Airbags That Were Never Even In Its Trucks</h3>
            <p>Toyota has issued a recall covering over 4,000 airbags that were never originally installed in its Tacoma and Tundra trucks. The affected parts were installed as replacements during collision repairs, meaning any Tacoma or Tundra that went through post-crash repair work could be carrying the faulty component.</p>
            <div class="card-tension"><b>The Tension:</b> A recall that traces back to the aftermarket repair supply chain rather than the factory line is a sharper problem for dealers and body shops than for engineering — it's a quality issue nobody at Toyota actually built.</div>
            <small>carscoops.com</small>
          </div>
        </a>
      </div>
      <div class="card reveal" data-mfr="DS">
        <a href="https://www.autocar.co.uk/car-news/new-cars/new-models-vital-ds-survival-uk-sales-hit-record-low" target="_blank" rel="noopener">
          <img src="https://placehold.co/800x450/1b1b1b/f60?text=AutoIntel.News" alt="DS Bets On Two New Models After UK Sales Hit A Record Low">
          <div class="card-content">
            <span class="badge">MARKET INTELLIGENCE</span>
            <h3>DS Bets On Two New Models After UK Sales Hit A Record Low</h3>
            <p>DS sold just 112 cars in the UK during the first half of 2026, an 88% decline from the 948 units it registered over the same period a year earlier. The brand is now pinning its UK recovery on two new models, the N3 supermini and N7 crossover, as it begins what the company frames as a fightback.</p>
            <div class="card-tension"><b>The Tension:</b> An 88% year-on-year collapse is the kind of number that makes "new models are coming" sound less like a strategy and more like the only card left to play.</div>
            <small>autocar.co.uk</small>
          </div>
        </a>
      </div>
      <div class="card reveal" data-mfr="Land Rover">
        <a href="https://www.carscoops.com/2026/08/freelander-8-sales-target/" target="_blank" rel="noopener">
          <img src="https://placehold.co/800x450/1b1b1b/f60?text=AutoIntel.News" alt="China's Reborn Land Rover Freelander Chases 150,000 Global Sales">
          <div class="card-content">
            <span class="badge">MARKET INTELLIGENCE</span>
            <h3>China's Reborn Land Rover Freelander Chases 150,000 Global Sales</h3>
            <p>Freelander has been relaunched as a standalone, Chinese-built joint-venture brand, and it's already targeting 150,000 yearly sales, with half of that volume expected to come from markets outside China.</p>
            <div class="card-tension"><b>The Tension:</b> A historically British nameplate is being rebuilt in China with export ambitions back into Land Rover's traditional home markets — a case study in how brand equity now travels in directions it never used to.</div>
            <small>carscoops.com</small>
          </div>
        </a>
      </div>
  </div>
</div>

<div class="sec-group" id="ev-technology">
  <div class="sec">
    <h2>EV & Technology</h2>
    <small>6 stories</small>
  </div>
  <div class="grid">
      <div class="card reveal" data-mfr="Toyota">
        <a href="https://www.motor1.com/news/803660/toyota-next-gen-batteries-hybrids/" target="_blank" rel="noopener">
          <img src="https://placehold.co/800x450/1b1b1b/f60?text=AutoIntel.News" alt="Toyota's Next-Gen Hybrid Batteries Arrive In 2027">
          <div class="card-content">
            <span class="badge">EV & TECHNOLOGY</span>
            <h3>Toyota's Next-Gen Hybrid Batteries Arrive In 2027</h3>
            <p>Toyota is preparing a new generation of hybrid batteries set to arrive in 2027, promising greater efficiency at a lower manufacturing cost than the current generation. Toyota has leaned on hybrid technology as its core electrification strategy while it takes a more gradual approach to full BEVs.</p>
            <div class="card-tension"><b>The Tension:</b> Cheaper, more efficient hybrid batteries strengthen exactly the technology Toyota bet on instead of an aggressive EV pivot — a bet that's looking increasingly vindicated as hybrid demand outpaces EVs in several major markets.</div>
            <small>motor1.com</small>
          </div>
        </a>
      </div>
      <div class="card reveal" data-mfr="Audi">
        <a href="https://www.motor1.com/news/803644/2027-audi-a2-official-details/" target="_blank" rel="noopener">
          <img src="https://placehold.co/800x450/1b1b1b/f60?text=AutoIntel.News" alt="Audi Calls The Returning A2 E-Tron Its Most Efficient Car Ever">
          <div class="card-content">
            <span class="badge">EV & TECHNOLOGY</span>
            <h3>Audi Calls The Returning A2 E-Tron Its Most Efficient Car Ever</h3>
            <p>The Audi A2 nameplate returns this fall as an all-electric model, described by Audi as its most efficient car to date. The new A2 E-Tron shares little beyond the name with its original early-2000s predecessor, arriving instead as a purpose-built EV aimed at efficiency-focused buyers.</p>
            <div class="card-tension"><b>The Tension:</b> Reviving a beloved nameplate on an entirely different platform is a bet that heritage still sells even when the product underneath has nothing in common with what earned that heritage.</div>
            <small>motor1.com</small>
          </div>
        </a>
      </div>
      <div class="card reveal" data-mfr="BYD">
        <a href="https://electrek.co/2026/08/03/byd-opens-denza-z9s-pre-orders-record-1100-km-ev-range/" target="_blank" rel="noopener">
          <img src="https://placehold.co/800x450/1b1b1b/f60?text=AutoIntel.News" alt="BYD Opens Denza Z9S Pre-Orders, Claims World's Longest EV Range">
          <div class="card-content">
            <span class="badge">EV & TECHNOLOGY</span>
            <h3>BYD Opens Denza Z9S Pre-Orders, Claims World's Longest EV Range</h3>
            <p>BYD has opened pre-orders in China for the new Denza Z9S, claiming what it calls the world's longest pure-electric range at 1,100 km (683 miles), with prices starting under $50,000. The claim, if it holds up under real-world testing, would put meaningful distance between BYD and Western EV range leaders at a comparable price.</p>
            <div class="card-tension"><b>The Tension:</b> A sub-$50,000 EV claiming a range figure well beyond what premium Western EVs offer at two or three times the price is the kind of number that should worry any OEM still pricing range as a luxury feature.</div>
            <small>electrek.co</small>
          </div>
        </a>
      </div>
      <div class="card reveal" data-mfr="">
        <a href="https://electrek.co/2026/08/03/base-power-raises-1b-to-roll-out-its-giant-new-home-battery/" target="_blank" rel="noopener">
          <img src="https://placehold.co/800x450/1b1b1b/f60?text=AutoIntel.News" alt="Base Power Raises $1B To Scale Its Giant Home Battery">
          <div class="card-content">
            <span class="badge">EV & TECHNOLOGY</span>
            <h3>Base Power Raises $1B To Scale Its Giant Home Battery</h3>
            <p>Base Power has unveiled Core, a 39.2-kWh home battery it says can keep a house running for up to 36 hours and can be installed in under an hour, backed by a fresh $1 billion raise to scale production. The product sits at the intersection of home energy storage and the broader EV charging and grid infrastructure buildout.</p>
            <div class="card-tension"><b>The Tension:</b> A billion-dollar bet on home batteries is really a bet that grid reliability, not vehicle range, becomes the next bottleneck for EV adoption at scale.</div>
            <small>electrek.co</small>
          </div>
        </a>
      </div>
      <div class="card reveal" data-mfr="Waymo">
        <a href="https://electrek.co/2026/07/29/waymo-gemini-ai-ojai-robotaxi-redesigned-interface/" target="_blank" rel="noopener">
          <img src="https://placehold.co/800x450/1b1b1b/f60?text=AutoIntel.News" alt="Waymo Adds Google's Gemini AI Assistant To Its Ojai Robotaxi">
          <div class="card-content">
            <span class="badge">EV & TECHNOLOGY</span>
            <h3>Waymo Adds Google's Gemini AI Assistant To Its Ojai Robotaxi</h3>
            <p>Waymo is integrating Google's Gemini AI assistant into its robotaxis for the first time, paired with the first major redesign of its rider interface in years. Both changes are launching on the Ojai, Waymo's purpose-built robotaxi vehicle, as the company prepares to open it up to more public riders.</p>
            <div class="card-tension"><b>The Tension:</b> Layering a conversational AI assistant onto a driverless vehicle raises the bar for what riders expect the car to understand — and for what happens when it doesn't.</div>
            <small>electrek.co</small>
          </div>
        </a>
      </div>
      <div class="card reveal" data-mfr="Tesla">
        <a href="https://electrek.co/2026/07/28/tesla-self-driving-manager-rolling-hazards-lawsuit/" target="_blank" rel="noopener">
          <img src="https://placehold.co/800x450/1b1b1b/f60?text=AutoIntel.News" alt="Ex-Tesla Manager Describes Understaffed, "Scary" Robotaxi Testing">
          <div class="card-content">
            <span class="badge">EV & TECHNOLOGY</span>
            <h3>Ex-Tesla Manager Describes Understaffed, "Scary" Robotaxi Testing</h3>
            <p>A former Tesla manager who ran the company's Full Self-Driving test fleet in Houston alleges in a wrongful-termination lawsuit that the operation was so understaffed its vehicles became "rolling hazards on public streets." He oversaw the fleet before Tesla launched its driverless Robotaxi service in the city.</p>
            <div class="card-tension"><b>The Tension:</b> A safety-culture allegation from inside the exact team that ran pre-launch testing lands right as Tesla is trying to convince regulators and riders that Robotaxi is ready for wider rollout.</div>
            <small>electrek.co</small>
          </div>
        </a>
      </div>
  </div>
</div>

<div class="sec-group" id="motorsports">
  <div class="sec">
    <h2>Motorsports</h2>
    <small>3 stories</small>
  </div>
  <div class="grid">
      <div class="card reveal" data-mfr="Ferrari">
        <a href="https://www.carscoops.com/2026/08/novitec-ferrari-12cilindri-spider/" target="_blank" rel="noopener">
          <img src="https://placehold.co/800x450/1b1b1b/f60?text=AutoIntel.News" alt="Novitec's Ferrari 12Cilindri Spider Brings Back The Manual Itch">
          <div class="card-content">
            <span class="badge">MOTORSPORTS</span>
            <h3>Novitec's Ferrari 12Cilindri Spider Brings Back The Manual Itch</h3>
            <p>Tuner Novitec has dressed the open-top, V12-powered Ferrari 12Cilindri Spider with subtle carbon-fiber aero, staggered Vossen forged wheels, lowered suspension and a gold-plated exhaust — a build aimed squarely at enthusiasts nostalgic for naturally aspirated, manual-adjacent driving character.</p>
            <div class="card-tension"><b>The Tension:</b> The aftermarket keeps finding demand for analog-feeling V12 builds even as the factory roadmap moves toward hybrid and electrified powertrains.</div>
            <small>carscoops.com</small>
          </div>
        </a>
      </div>
      <div class="card reveal" data-mfr="">
        <a href="https://www.autocar.co.uk/car-news/features/243mph-public-roads-meet-worlds-maddest-motorsport-event" target="_blank" rel="noopener">
          <img src="https://placehold.co/800x450/1b1b1b/f60?text=AutoIntel.News" alt="Inside The Silver State Challenge: 243mph, No Barriers">
          <div class="card-content">
            <span class="badge">MOTORSPORTS</span>
            <h3>Inside The Silver State Challenge: 243mph, No Barriers</h3>
            <p>Twice a year, the Silver State Classic Challenge closes a long stretch of Nevada's Route 318 and turns it into one of the only places left where competitors can legally exceed 200mph on a public road — with no barriers, no run-off and no catch fencing.</p>
            <div class="card-tension"><b>The Tension:</b> An event this extreme surviving largely unchanged is a reminder of how much motorsport culture still runs on grassroots tolerance for risk that modern racing series have engineered almost entirely out.</div>
            <small>autocar.co.uk</small>
          </div>
        </a>
      </div>
      <div class="card reveal" data-mfr="">
        <a href="https://www.autocar.co.uk/car-news/from-the-archive/why-women-were-blocked-le-mans-decades" target="_blank" rel="noopener">
          <img src="https://placehold.co/800x450/1b1b1b/f60?text=AutoIntel.News" alt="Why Women Were Blocked From Le Mans For Decades">
          <div class="card-content">
            <span class="badge">MOTORSPORTS</span>
            <h3>Why Women Were Blocked From Le Mans For Decades</h3>
            <p>Jamie Chadwick recently became the first woman to drive a hypercar at Le Mans, a milestone that would have been barred outright just decades ago. Women who fought to compete in earlier eras of the race, including in cars like the Mini Marcos, faced formal and informal barriers that have only gradually lifted.</p>
            <div class="card-tension"><b>The Tension:</b> A genuine milestone this year sits against how recently the sport actively excluded the drivers now making history in it.</div>
            <small>autocar.co.uk</small>
          </div>
        </a>
      </div>
  </div>
</div>

<div class="sec-group" id="performance-builds">
  <div class="sec">
    <h2>Performance Builds</h2>
    <small>6 stories</small>
  </div>
  <div class="grid">
      <div class="card reveal" data-mfr="Lamborghini">
        <a href="https://www.motor1.com/news/803585/lamborghini-revuelto-miura-homage-package/" target="_blank" rel="noopener">
          <img src="https://placehold.co/800x450/1b1b1b/f60?text=AutoIntel.News" alt="Lamborghini Honors The Miura With A Limited Revuelto Homage">
          <div class="card-content">
            <span class="badge">PERFORMANCE BUILDS</span>
            <h3>Lamborghini Honors The Miura With A Limited Revuelto Homage</h3>
            <p>The Lamborghini Revuelto Miura 60° Homage marks the Miura's 60th anniversary with exclusive exterior color choices and two dedicated livery options, tying Lamborghini's current hybrid flagship back to the car widely credited with inventing the modern supercar layout.</p>
            <div class="card-tension"><b>The Tension:</b> A tribute package on a hybrid flagship is Lamborghini leaning on 1960s heritage to sell a very 2020s powertrain.</div>
            <small>motor1.com</small>
          </div>
        </a>
      </div>
      <div class="card reveal" data-mfr="">
        <a href="https://www.motor1.com/news/803555/brabus-carbon-catamaran-debut/" target="_blank" rel="noopener">
          <img src="https://placehold.co/800x450/1b1b1b/f60?text=AutoIntel.News" alt="Brabus Builds A 1,450hp Luxury Catamaran With Hydrofoils">
          <div class="card-content">
            <span class="badge">PERFORMANCE BUILDS</span>
            <h3>Brabus Builds A 1,450hp Luxury Catamaran With Hydrofoils</h3>
            <p>Brabus has expanded beyond cars into marine performance with the Ultima 55, a 56-foot luxury catamaran combining carbon construction, hydrofoils and twin six-cylinder engines producing a combined 1,450 horsepower.</p>
            <div class="card-tension"><b>The Tension:</b> A performance tuner best known for cars branching into hydrofoil yachts says as much about where high-margin performance-brand money is chasing customers as it does about boats.</div>
            <small>motor1.com</small>
          </div>
        </a>
      </div>
      <div class="card reveal" data-mfr="Hennessey">
        <a href="https://www.motor1.com/news/803525/hennessey-blackbird-specs-photos-details/" target="_blank" rel="noopener">
          <img src="https://placehold.co/800x450/1b1b1b/f60?text=AutoIntel.News" alt="Hennessey's New Blackbird Skips Turbos, Hybrids And Screens">
          <div class="card-content">
            <span class="badge">PERFORMANCE BUILDS</span>
            <h3>Hennessey's New Blackbird Skips Turbos, Hybrids And Screens</h3>
            <p>Hennessey's new Blackbird, its third all-new model and successor to the Venom F5, is built around "maximum man-machine connection" rather than outright spec-chasing: no turbos, no hybrid assist, no digital screens, and a gated manual gearbox. Targeted figures still put it near the top of the supercar class, at 800-850bhp and a sub-3.0-second 0-60mph time.</p>
            <div class="card-tension"><b>The Tension:</b> Building a screenless, naturally aspirated manual supercar in 2026 is a direct bet that a shrinking niche of buyers will pay a premium for exactly the tech the rest of the industry is racing to add.</div>
            <small>motor1.com</small>
          </div>
        </a>
      </div>
      <div class="card reveal" data-mfr="Geely">
        <a href="https://electrek.co/2026/08/03/geely-galaxy-battleship-700-tri-motor-stuffs-1113-hp-in-a-high-luxe-boxy-package/" target="_blank" rel="noopener">
          <img src="https://placehold.co/800x450/1b1b1b/f60?text=AutoIntel.News" alt="Geely's Galaxy Battleship 700 Packs 1,113hp Into A Boxy SUV">
          <div class="card-content">
            <span class="badge">PERFORMANCE BUILDS</span>
            <h3>Geely's Galaxy Battleship 700 Packs 1,113hp Into A Boxy SUV</h3>
            <p>The Geely Galaxy Battleship 700, initially expected to target the Range Rover and Land Cruiser, arrives instead with a tri-motor setup producing 1,113 horsepower — putting it closer in output to Italian exotics than to the rugged-luxury SUVs it was originally pitched against.</p>
            <div class="card-tension"><b>The Tension:</b> A Chinese SUV outgunning European hypercars on horsepower alone is a sharp signal of how fast the performance ceiling in that market is rising.</div>
            <small>electrek.co</small>
          </div>
        </a>
      </div>
      <div class="card reveal" data-mfr="Hennessey">
        <a href="https://www.autocar.co.uk/car-news/new-cars/hennessey-blackbird-brings-850bhp-manual-box-and-no-screens" target="_blank" rel="noopener">
          <img src="https://placehold.co/800x450/1b1b1b/f60?text=AutoIntel.News" alt="Hennessey Blackbird: 850bhp, A Manual, And No Screens">
          <div class="card-content">
            <span class="badge">PERFORMANCE BUILDS</span>
            <h3>Hennessey Blackbird: 850bhp, A Manual, And No Screens</h3>
            <p>Hennessey's Blackbird pitches itself against the screen-heavy, hybrid-assisted supercar mainstream with an atmospheric V8, a gated manual gearbox, and a stated target of 800-850bhp with a sub-3.0-second 0-60mph run and a 220mph top speed.</p>
            <div class="card-tension"><b>The Tension:</b> Hennessey is making the same bet twice in one launch cycle: that driver engagement, not spec-sheet tech, is what will actually move six-figure supercar buyers.</div>
            <small>autocar.co.uk</small>
          </div>
        </a>
      </div>
      <div class="card reveal" data-mfr="Alfa Romeo">
        <a href="https://www.autocar.co.uk/opinion/tester%27s-notes/alfa-romeo-only-brand-can-sell-cars-%C2%A330k-and-%C2%A314m" target="_blank" rel="noopener">
          <img src="https://placehold.co/800x450/1b1b1b/f60?text=AutoIntel.News" alt="Is Alfa Romeo The Only Brand Selling Cars At Both £30k And £1.4m?">
          <div class="card-content">
            <span class="badge">PERFORMANCE BUILDS</span>
            <h3>Is Alfa Romeo The Only Brand Selling Cars At Both £30k And £1.4m?</h3>
            <p>Alfa Romeo's current range spans from the sub-£30,000 Junior up to the limited-run 33 Stradale hypercar, with build slots for the latter advertised as high as £3.5 million — a pricing spread few, if any, other brands currently match across a single lineup.</p>
            <div class="card-tension"><b>The Tension:</b> Spanning that price range under one badge is either brilliant brand elasticity or a sign the mainstream and halo ends of the lineup are being built for two completely different customers who happen to share a logo.</div>
            <small>autocar.co.uk</small>
          </div>
        </a>
      </div>
  </div>
</div>

<div class="sec-group" id="suppliers">
  <div class="sec">
    <h2>Suppliers</h2>
    <small>2 stories</small>
  </div>
  <div class="grid">
      <div class="card reveal" data-mfr="Volvo">
        <a href="https://electrek.co/2026/07/29/volvo-drops-lidar-ex90-es90-compensation/" target="_blank" rel="noopener">
          <img src="https://placehold.co/800x450/1b1b1b/f60?text=AutoIntel.News" alt="Volvo Drops Lidar For Good On EX90 And ES90, Pays Owners Back">
          <div class="card-content">
            <span class="badge">SUPPLIERS</span>
            <h3>Volvo Drops Lidar For Good On EX90 And ES90, Pays Owners Back</h3>
            <p>Volvo has confirmed it is permanently dropping lidar from the EX90 and ES90 after cutting ties with supplier Luminar, and is compensating owners for a feature they were promised but will never receive — including a payout of roughly $1,900 per car in Norway, one of several market-specific settlements.</p>
            <div class="card-tension"><b>The Tension:</b> Paying owners to walk back a headline safety feature is an unusually direct admission that a supplier relationship broke down badly enough to change what the car actually is.</div>
            <small>electrek.co</small>
          </div>
        </a>
      </div>
      <div class="card reveal" data-mfr="Tesla">
        <a href="https://electrek.co/2026/07/28/tesla-sues-cybertruck-supplier-angstrom-tooling/" target="_blank" rel="noopener">
          <img src="https://placehold.co/800x450/1b1b1b/f60?text=AutoIntel.News" alt="Tesla Sues Cybertruck Supplier Over Tooling Access">
          <div class="card-content">
            <span class="badge">SUPPLIERS</span>
            <h3>Tesla Sues Cybertruck Supplier Over Tooling Access</h3>
            <p>Tesla is seeking emergency court access to a plant in Troy, Texas, operated by supplier Angstrom Automotive Group, to retrieve tooling needed to keep building the Cybertruck. Angstrom is closing the plant and has denied Tesla access; Tesla says thousands of already-committed Cybertrucks can't be completed without the dies inside.</p>
            <div class="card-tension"><b>The Tension:</b> A single supplier standoff holding up thousands of already sold trucks is a reminder of how little slack exists anywhere in modern production chains.</div>
            <small>electrek.co</small>
          </div>
        </a>
      </div>
  </div>
</div>

<div class="sec-group" id="dealer-news">
  <div class="sec">
    <h2>Dealer News</h2>
    <small>1 stories</small>
  </div>
  <div class="grid">
      <div class="card reveal" data-mfr="Genesis|Hyundai">
        <a href="https://electrek.co/2026/07/30/genesis-gv60-magma-costs-10k-more-than-hyundai-ioniq-5-n/" target="_blank" rel="noopener">
          <img src="https://placehold.co/800x450/1b1b1b/f60?text=AutoIntel.News" alt="Genesis GV60 Magma Prices $10,000 Above The IONIQ 5 N">
          <div class="card-content">
            <span class="badge">DEALER NEWS</span>
            <h3>Genesis GV60 Magma Prices $10,000 Above The IONIQ 5 N</h3>
            <p>The performance-focused Genesis GV60 Magma is set to begin arriving at dealerships priced roughly $10,000 above its closest corporate sibling, the Hyundai IONIQ 5 N, putting the two head-to-head on the same showroom lots at a meaningfully different price.</p>
            <div class="card-tension"><b>The Tension:</b> Dealers now have to sell buyers on a $10,000 premium between two vehicles from the same corporate parent that share more engineering than either brand likes to advertise.</div>
            <small>electrek.co</small>
          </div>
        </a>
      </div>
  </div>
</div>

<div class="sec-group" id="industry-news">
  <div class="sec">
    <h2>Industry News</h2>
    <small>6 stories</small>
  </div>
  <div class="grid">
      <div class="card reveal" data-mfr="Tesla">
        <a href="https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/" target="_blank" rel="noopener">
          <img src="https://placehold.co/800x450/1b1b1b/f60?text=AutoIntel.News" alt="NHTSA Opens Probe Into 1.2M Teslas Over Suspension Failures">
          <div class="card-content">
            <span class="badge">INDUSTRY NEWS</span>
            <h3>NHTSA Opens Probe Into 1.2M Teslas Over Suspension Failures</h3>
            <p>The NHTSA has opened an investigation into roughly 1.2 million Tesla vehicles after receiving 156 complaints of a front suspension component detaching while driving. The probe covers 2018-2020 Model 3 and 2021-2023 Model Y vehicles and centers on the front lower lateral link separating from the car.</p>
            <div class="card-tension"><b>The Tension:</b> A federal safety probe at this scale lands directly on service departments and resale confidence, regardless of how the investigation itself resolves.</div>
            <small>electrek.co</small>
          </div>
        </a>
      </div>
      <div class="card reveal" data-mfr="Tesla">
        <a href="https://electrek.co/2026/07/30/tesla-weighs-selling-china-business-spacex-merger/" target="_blank" rel="noopener">
          <img src="https://placehold.co/800x450/1b1b1b/f60?text=AutoIntel.News" alt="Report: Tesla Weighs Selling China Business Ahead Of SpaceX Merger">
          <div class="card-content">
            <span class="badge">INDUSTRY NEWS</span>
            <h3>Report: Tesla Weighs Selling China Business Ahead Of SpaceX Merger</h3>
            <p>Tesla is reportedly examining a sale of its China business to clear the way for a merger with SpaceX, according to a Wall Street Journal report. Tesla's Shanghai factory builds more than half of all Tesla vehicles, meaning any separation would carve out the single largest piece of the company's car operations. Elon Musk has denied the report.</p>
            <div class="card-tension"><b>The Tension:</b> Even a denied report about spinning off the factory that builds most of your cars is the kind of headline that unsettles suppliers and dealers well before anything is confirmed.</div>
            <small>electrek.co</small>
          </div>
        </a>
      </div>
      <div class="card reveal" data-mfr="Jaguar Land Rover">
        <a href="https://www.motor1.com/news/803393/jlr-new-north-american-ceo-appointed/" target="_blank" rel="noopener">
          <img src="https://placehold.co/800x450/1b1b1b/f60?text=AutoIntel.News" alt="JLR's New North American CEO Inherits A Full Plate">
          <div class="card-content">
            <span class="badge">INDUSTRY NEWS</span>
            <h3>JLR's New North American CEO Inherits A Full Plate</h3>
            <p>Jaguar Land Rover's incoming North American CEO takes over with ambitious plans already in motion, including new model introductions and an expanded range of powertrain options aimed at rebuilding the brand's position in its largest market.</p>
            <div class="card-tension"><b>The Tension:</b> A leadership change landing in the middle of a major product push puts execution risk squarely on one new executive's shoulders.</div>
            <small>motor1.com</small>
          </div>
        </a>
      </div>
      <div class="card reveal" data-mfr="Cadillac">
        <a href="https://www.motor1.com/news/803510/gm-cadillac-infotainment-updates/" target="_blank" rel="noopener">
          <img src="https://placehold.co/800x450/1b1b1b/f60?text=AutoIntel.News" alt="Cadillac Rolls Out A Major Infotainment Fix Across Its EV Lineup">
          <div class="card-content">
            <span class="badge">INDUSTRY NEWS</span>
            <h3>Cadillac Rolls Out A Major Infotainment Fix Across Its EV Lineup</h3>
            <p>Cadillac is rolling out a significant infotainment update across the Lyriq, Optiq, Vistiq and CT5, adding a smarter media queue, profile-linked seat settings, sharper head-up-display graphics and a redesigned home screen layout.</p>
            <div class="card-tension"><b>The Tension:</b> Software fixes rolling out well after these vehicles reached dealer lots underscore how much of the modern ownership experience now gets finished after the sale, not before it.</div>
            <small>motor1.com</small>
          </div>
        </a>
      </div>
      <div class="card reveal" data-mfr="Mercedes-Benz">
        <a href="https://www.motor1.com/news/803387/mercedes-went-too-far-on-touchscreens/" target="_blank" rel="noopener">
          <img src="https://placehold.co/800x450/1b1b1b/f60?text=AutoIntel.News" alt="Mercedes Admits It Went "Too Far" Cutting Physical Buttons">
          <div class="card-content">
            <span class="badge">INDUSTRY NEWS</span>
            <h3>Mercedes Admits It Went "Too Far" Cutting Physical Buttons</h3>
            <p>Mercedes says customer research shows buyers still love its large in-cabin displays, but the company is walking back part of its screen-only push, confirming future models will reintroduce more physical controls for key functions.</p>
            <div class="card-tension"><b>The Tension:</b> Reversing a design philosophy this publicly is a rare, direct admission that a well-funded interior strategy misjudged what buyers actually wanted to touch.</div>
            <small>motor1.com</small>
          </div>
        </a>
      </div>
      <div class="card reveal" data-mfr="Infiniti">
        <a href="https://www.carscoops.com/2026/08/costco-infiniti-discount/" target="_blank" rel="noopener">
          <img src="https://placehold.co/800x450/1b1b1b/f60?text=AutoIntel.News" alt="Infiniti's New QX65 Launches With A Costco Discount Already Attached">
          <div class="card-content">
            <span class="badge">INDUSTRY NEWS</span>
            <h3>Infiniti's New QX65 Launches With A Costco Discount Already Attached</h3>
            <p>Infiniti's new 2027 QX65 qualifies for a Costco member discount from launch, one of three Infiniti SUVs — spanning the QX65 up to the six-figure QX80 — currently enrolled in the program.</p>
            <div class="card-tension"><b>The Tension:</b> Attaching a warehouse-club discount to a brand-new model on day one is an early signal about how much pricing confidence Infiniti actually has in it.</div>
            <small>carscoops.com</small>
          </div>
        </a>
      </div>
  </div>
</div>

<footer>
  <p style="color:#555;margin-top:20px">AutoIntel.News reveals market contradictions behind automotive headlines. We highlight tensions between announcements and reality, strategy and execution, OEM plans and buyer behavior. All links open in new tabs.</p>
</footer>

</div>

<script>
document.getElementById('publishDate').textContent = new Date().toLocaleDateString('en-US', {weekday:'long',year:'numeric',month:'long',day:'numeric'}).toUpperCase();

(function(){
  var select = document.getElementById('mfrFilterSelect');
  if (!select) return;
  var cards = Array.prototype.slice.call(document.querySelectorAll('.card, .hero'));
  var groups = Array.prototype.slice.call(document.querySelectorAll('.sec-group'));

  function applyFilter(selected) {
    cards.forEach(function(card){
      var mfrs = (card.getAttribute('data-mfr') || '').split('|').filter(Boolean);
      var match = selected === '__all__' || mfrs.indexOf(selected) !== -1;
      card.classList.toggle('is-hidden', !match);
    });
    groups.forEach(function(group){
      var visible = group.querySelectorAll('.card:not(.is-hidden)').length > 0;
      group.classList.toggle('is-hidden', !visible);
    });
  }

  select.addEventListener('change', function(){
    applyFilter(select.value);
  });
})();

(function(){
  var counters = Array.prototype.slice.call(document.querySelectorAll('.stat-num'));
  if (!counters.length) return;
  var reduceMotion = window.matchMedia && window.matchMedia('(prefers-reduced-motion: reduce)').matches;
  counters.forEach(function(el){
    var target = parseInt(el.getAttribute('data-target'), 10) || 0;
    if (reduceMotion) { el.textContent = target; return; }
    var duration = 1500;
    var start = null;
    function step(ts){
      if (start === null) start = ts;
      var progress = Math.min((ts - start) / duration, 1);
      var eased = 1 - Math.pow(1 - progress, 3);
      el.textContent = Math.floor(eased * target);
      if (progress < 1) {
        requestAnimationFrame(step);
      } else {
        el.textContent = target;
      }
    }
    requestAnimationFrame(step);
  });
})();

(function(){
  var reveals = Array.prototype.slice.call(document.querySelectorAll('.reveal'));
  if (!reveals.length) return;
  if (!('IntersectionObserver' in window)) {
    reveals.forEach(function(el){ el.classList.add('is-visible'); });
    return;
  }
  document.querySelectorAll('.grid').forEach(function(grid){
    var items = grid.querySelectorAll('.reveal');
    items.forEach(function(el, i){
      el.style.transitionDelay = (Math.min(i, 5) * 80) + 'ms';
    });
  });
  var observer = new IntersectionObserver(function(entries){
    entries.forEach(function(entry){
      if (entry.isIntersecting) {
        entry.target.classList.add('is-visible');
        observer.unobserve(entry.target);
      }
    });
  }, { threshold: 0.15, rootMargin: '0px 0px -40px 0px' });
  reveals.forEach(function(el){ observer.observe(el); });
})();

(function(){
  var bar = document.getElementById('scrollTopBar');
  if (!bar) return;
  var threshold = 220;
  function onScroll(){
    if (window.scrollY > threshold) {
      bar.classList.add('is-visible');
    } else {
      bar.classList.remove('is-visible');
    }
  }
  window.addEventListener('scroll', onScroll, { passive: true });
  onScroll();
  function goTop(){
    window.scrollTo({ top: 0, behavior: 'smooth' });
  }
  bar.addEventListener('click', goTop);
  bar.addEventListener('keydown', function(e){
    if (e.key === 'Enter' || e.key === ' ') {
      e.preventDefault();
      goTop();
    }
  });
})();
</script>

</body>
</html>
