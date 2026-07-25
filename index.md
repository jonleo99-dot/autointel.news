<html>
<head>
<meta charset='utf-8'>
<meta name='viewport' content='width=device-width,initial-scale=1'>
<title>AutoIntel.News - Issue 002</title>
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
header h3{
  margin:5px 0 15px 0;
  font-size:16px;
  font-weight:normal;
  color:#aaa
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
  font-size:10px
}
.card-content h3{
  margin:0 0 10px 0;
  font-size:15px;
  line-height:1.4;
  color:#fff;
  flex-grow:1
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
.stat{
  display:inline-block;
  margin:0 20px;
  font-weight:bold;
  color:#f60
}
@media(max-width:768px){
  header{padding:20px}
  header h1{font-size:32px}
  .hero img{height:280px}
  .hero-content{padding:20px}
  .grid{grid-template-columns:1fr}
}
</style>
</head>
<body>

<header>
  <div class='date-field' id='publishDate'></div>
  <h1>AutoIntel.News <span style="color:#f60;font-family:Times,'Times New Roman',serif">ō͡≡o˞̶</span></h1>
  <h3>Automotive Intelligence. Curated Daily.</h3>
  <p><b>Today's Drive:</b> Manufacturers announce ambitious plans while market data reveals a different story: EVs stall in new sales, hybrids dominate buyer preference, affordability crises deepen, yet performance culture thrives. The real story lies in the contradictions.</p>
</header>

<script>
document.getElementById('publishDate').textContent = new Date().toLocaleDateString('en-US', {weekday:'long',year:'numeric',month:'long',day:'numeric'}).toUpperCase();
</script>

<div class='wrap'>

<!-- Hero Story -->
<div class='hero'>
  <img src="https://www.autonews.com/resizer/v2/HC73AQ735RAZ3IT6ZV637ZPD3E.jpg?auth=0022658d37a51863922355078a47a0b5e383df3a09b725a443cb699b6011369f&amp;width=1200#.jpg" alt="Hero Story">
  <div class='hero-content'>
    <span class='badge'>FEATURE STORY</span>
    <h2>Weekend Drive: Honda is considering a new North American factory; GM raises its guidance for a second time this year</h2>
    <p>Honda has its sights set on a new North American factory. President Donald Trump has ordered 50 percent tariffs on some Canadian goods. Plus, Gener...</p>
    <div class='hero-tension'><b>The Tension:</b> OEM announcements multiply while execution reality—production, affordability, and market appetite—remain questionable.</div>
  </div>
</div>


<!-- OEM Spotlight Section -->
<div class='sec'>
  <h2>OEM Spotlight</h2>
  <small><b>Where Plans Meet Reality</b></small>
</div>

<div class='grid'>
  <a href="https://www.autonews.com/podcasts/daily-drive/an-weekend-drive-honda-is-considering-a-new-north-american-factory-0725/" target="_blank">
    <div class='card'>
      <img src="https://www.autonews.com/resizer/v2/HC73AQ735RAZ3IT6ZV637ZPD3E.jpg?auth=0022658d37a51863922355078a47a0b5e383df3a09b725a443cb699b6011369f&amp;width=1200#.jpg" alt="Weekend Drive: Honda is considering a new North American factory; GM raises its guidance for a second time this year">
      <div class='card-content'>
        <span class='badge'>AUTONEWS</span>
        <h3>Weekend Drive: Honda is considering a new North American factory; GM raises i...</h3>
        <p>Honda has its sights set on a new North American factory. President Donald Trump has ordered 50 percent tariffs on some Canadian goods. Plus, Gener...</p>
        <div class='card-tension'><b>Tension:</b> OEM announcements multiply while execution reality—production, affordability, and market appetite—remain questionable.</div>
        <small>Read on autonews.com</small>
      </div>
    </div>
  </a>
  <a href="https://www.wardsauto.com/news/ford-global-power-products-debut-home-backup-solution/826066/" target="_blank">
    <div class='card'>
      <img src="https://imgproxy.divecdn.com/D9N3Nz4gIfh_8CFTNIqzoAY3MgbSqebznZWRFW3YGd0/g:ce/rs:fit:770:435/Z3M6Ly9kaXZlc2l0ZS1zdG9yYWdlL2RpdmVpbWFnZS9Sb3VnZV9FbGVjdHJpY19WZWhpY2xlX0NlbnRlcl8wM19fSmFjcXVlbGluZV9MYW56LmpwZw==.webp" alt="Ford, Global Power Products debut home backup solution">
      <div class='card-content'>
        <span class='badge'>WARDSAUTO</span>
        <h3>Ford, Global Power Products debut home backup solution</h3>
        <p>More than 800 electric utilities have approved GPP’s GenerLink transfer switch, which provides backup power for outlets and hardwired appliances at...</p>
        <div class='card-tension'><b>Tension:</b> Affordability crisis deepens with rising incentives and negative equity, yet market remains driven by luxury launches.</div>
        <small>Read on wardsauto.com</small>
      </div>
    </div>
  </a>
  <a href="https://www.wardsauto.com/news/ford-chinas-geely-to-build-cars-in-spain-in-joint-venture/825995/" target="_blank">
    <div class='card'>
      <img src="https://imgproxy.divecdn.com/7gtt5ErIuVi7WwBYy13OWl3d2NLs3QCWlsevrRtvl0A/g:ce/rs:fit:770:435/Z3M6Ly9kaXZlc2l0ZS1zdG9yYWdlL2RpdmVpbWFnZS9Gb3JkS3VnYVNwYWluMjAyNS5qcGc=.webp" alt="Ford, China’s Geely to build cars in Spain in joint venture">
      <div class='card-content'>
        <span class='badge'>WARDSAUTO</span>
        <h3>Ford, China’s Geely to build cars in Spain in joint venture</h3>
        <p>The deal calls for the automakers to build two new Ford multi-energy vehicles and two new Geely electric SUVs at the Valencia plant.</p>
        <div class='card-tension'><b>Tension:</b> Manufacturer EV investment continues despite new EV market share slipping to 5.9%—a disconnect between strategy and sales.</div>
        <small>Read on wardsauto.com</small>
      </div>
    </div>
  </a>
  <a href="https://www.wardsauto.com/news/ford-recalls-nearly-388k-suvs-for-binding-second-row-seat-switches/825957/" target="_blank">
    <div class='card'>
      <img src="https://imgproxy.divecdn.com/wREhPyQW5AAQ6a3OrUCt7WIaY0anOT4Xqi1UO8TrPyM/g:ce/rs:fit:770:435/Z3M6Ly9kaXZlc2l0ZS1zdG9yYWdlL2RpdmVpbWFnZS9TY3JlZW5zaG90XzIwMjYtMDctMjJfYXRfMi40NS4yMFBNLnBuZw==.webp" alt="Ford recalls nearly 388K SUVs for binding second-row seat switches">
      <div class='card-content'>
        <span class='badge'>WARDSAUTO</span>
        <h3>Ford recalls nearly 388K SUVs for binding second-row seat switches</h3>
        <p>The recall expands a previous one in June 2025 for switches that can stick and cause the second-row seats to suddenly slide or fold.</p>
        <div class='card-tension'><b>Tension:</b> Market realities often contradict headline announcements—dig deeper for the real story.</div>
        <small>Read on wardsauto.com</small>
      </div>
    </div>
  </a>
  <a href="https://www.wardsauto.com/news/honda-confirms-next-gen-ridgeline-pickup/825975/" target="_blank">
    <div class='card'>
      <img src="https://imgproxy.divecdn.com/Z70QNs_rLy1DV9YnHa_0EK3tUe67zpBTLEz28IPUgJs/g:ce/rs:fit:770:435/Z3M6Ly9kaXZlc2l0ZS1zdG9yYWdlL2RpdmVpbWFnZS9OZXh0X0dlbl9SaWRnZWxpbmVfVGVhc2VyXy1fRklOQUxfNy05LTI2LmpwZw==.webp" alt="Honda confirms next-gen Ridgeline pickup">
      <div class='card-content'>
        <span class='badge'>WARDSAUTO</span>
        <h3>Honda confirms next-gen Ridgeline pickup</h3>
        <p>Set to arrive within two years, the third-generation Ridgeline will continue to be built in Alabama.</p>
        <div class='card-tension'><b>Tension:</b> Market realities often contradict headline announcements—dig deeper for the real story.</div>
        <small>Read on wardsauto.com</small>
      </div>
    </div>
  </a>
  <a href="https://www.kbb.com/car-news/honda-pauses-manual-transmission-civic-si-acura-integra-a-spec/" target="_blank">
    <div class='card'>
      <img src="https://dam.coxautoinc.com/asset/3902c8ef-b12b-443d-9ed3-f9a697097feb/OG/2025-Honda-Civic-Si.jpg" alt="Honda Pauses Manual Transmission Civic Si, Acura Integra A-Spec">
      <div class='card-content'>
        <span class='badge'>KBB</span>
        <h3>Honda Pauses Manual Transmission Civic Si, Acura Integra A-Spec</h3>
        <p>Honda confirmed the Si&#x27;s return, but did not give details on its transmission.</p>
        <div class='card-tension'><b>Tension:</b> Market realities often contradict headline announcements—dig deeper for the real story.</div>
        <small>Read on kbb.com</small>
      </div>
    </div>
  </a>
</div>

<!-- Market Intelligence Section -->
<div class='sec'>
  <h2>Market Intelligence</h2>
  <small><b>What Buyers Really Do</b></small>
</div>

<div class='grid'>
  <a href="https://www.autonews.com/data-center/sales-data/an-estimated-europe-registrations-country-june-2026/" target="_blank">
    <div class='card'>
      <img src="https://www.autonews.com/resizer/v2/TR2DA323XVAMFMMPAVKPO2ULS4.jpg?focal=2593%2C960&amp;amp;auth=10ebe786ad39816053b023bbae7807c94f0375a19b99bfde436449d27be01820&amp;amp;width=3648&amp;amp;height=2052" alt="Estimated Europe registrations by country, June &amp; YTD 2026">
      <div class='card-content'>
        <span class='badge'>AUTONEWS</span>
        <h3>Estimated Europe registrations by country, June &amp; YTD 2026</h3>
        <p>Unit registrations of passenger vehicles listed alphabetically by country for the current and previous year periods</p>
        <div class='card-tension'><b>Tension:</b> Market data reveals structural shifts: what OEMs announce rarely aligns with what buyers actually purchase.</div>
        <small>Read on autonews.com</small>
      </div>
    </div>
  </a>
  <a href="https://www.autonews.com/data-center/sales-data/an-estimated-europe-registrations-make-june-2026/" target="_blank">
    <div class='card'>
      <img src="https://www.autonews.com/resizer/v2/TR2DA323XVAMFMMPAVKPO2ULS4.jpg?focal=2593%2C960&amp;amp;auth=10ebe786ad39816053b023bbae7807c94f0375a19b99bfde436449d27be01820&amp;amp;width=3648&amp;amp;height=2052" alt="Estimated Europe registrations by make, June &amp; YTD 2026">
      <div class='card-content'>
        <span class='badge'>AUTONEWS</span>
        <h3>Estimated Europe registrations by make, June &amp; YTD 2026</h3>
        <p>Unit registrations of passenger vehicles listed alphabetically by brand and automaker for the current and previous year periods</p>
        <div class='card-tension'><b>Tension:</b> Market data reveals structural shifts: what OEMs announce rarely aligns with what buyers actually purchase.</div>
        <small>Read on autonews.com</small>
      </div>
    </div>
  </a>
  <a href="https://www.wardsauto.com/news/ally-financial-sees-loan-applications-rise-to-record-levels-in-q2/825938/" target="_blank">
    <div class='card'>
      <img src="https://imgproxy.divecdn.com/X0Fu3zVaTa61gkKxe-yk-EiDIuRzHgzhvydUqAl4FDY/g:ce/rs:fit:770:435/Z3M6Ly9kaXZlc2l0ZS1zdG9yYWdlL2RpdmVpbWFnZS9jYXJfbG9hbl9nZXR0eWltYWdlcy0yMTQ4ODIzNjM5LTYxMng2MTIuanBn.webp" alt="Ally Financial sees loan applications rise to record levels in Q2">
      <div class='card-content'>
        <span class='badge'>WARDSAUTO</span>
        <h3>Ally Financial sees loan applications rise to record levels in Q2</h3>
        <p>The lender&#x27;s increase in applications from the top of the purchase funnel allows Ally to be more selective while growing volume.</p>
        <div class='card-tension'><b>Tension:</b> Market realities often contradict headline announcements—dig deeper for the real story.</div>
        <small>Read on wardsauto.com</small>
      </div>
    </div>
  </a>
</div>

<!-- EV & Technology Section -->
<div class='sec'>
  <h2>EV & Technology</h2>
  <small><b>The Electrification Paradox</b></small>
</div>

<div class='grid'>
  <a href="https://www.kbb.com/car-advice/how-much-does-it-cost-to-charge-an-ev/" target="_blank">
    <div class='card'>
      <img src="https://dam.coxautoinc.com/asset/1eb14d22-7da6-409d-b68f-f78d0a77396d/OG/Electrify-America-Charging.jpg" alt="How Much Does It Cost to Charge an Electric Car?">
      <div class='card-content'>
        <span class='badge'>KBB</span>
        <h3>How Much Does It Cost to Charge an Electric Car?</h3>
        <p>Learn how to calculate the cost of charging EVs at home and at charging stations, the charge levels to choose from and how to find the right plug f...</p>
        <div class='card-tension'><b>Tension:</b> Affordability crisis deepens with rising incentives and negative equity, yet market remains driven by luxury launches.</div>
        <small>Read on kbb.com</small>
      </div>
    </div>
  </a>
  <a href="https://www.caranddriver.com/news/a73259033/chevy-equinox-ev-next-gen-report/" target="_blank">
    <div class='card'>
      <img src="https://hips.hearstapps.com/hmg-prod/images/2024-chevrolet-equinox-ev-3rs-584-6657c7cc55102.jpg?crop=1.00xw:0.753xh;0,0.202xh&amp;resize=1200:*" alt="Report: Chevrolet Is Already Cooking Up a Next-Generation Equinox EV">
      <div class='card-content'>
        <span class='badge'>CARANDDRIVER</span>
        <h3>Report: Chevrolet Is Already Cooking Up a Next-Generation Equinox EV</h3>
        <p>The next version of the compact electric SUV is expected to arrive for the 2029 model year and will ride on a new platform.</p>
        <div class='card-tension'><b>Tension:</b> Manufacturer EV investment continues despite new EV market share slipping to 5.9%—a disconnect between strategy and sales.</div>
        <small>Read on caranddriver.com</small>
      </div>
    </div>
  </a>
  <a href="https://www.caranddriver.com/news/a73249953/2027-toyota-crown-update-details/" target="_blank">
    <div class='card'>
      <img src="https://hips.hearstapps.com/hmg-prod/images/a22fa349-798d-4457-95e2-6e82c8f96be8.png?crop=0.468xw:0.311xh;0.340xw,0.366xh&amp;resize=1200:*" alt="Toyota Updates the Oddball Crown for 2027 with New Hybrid Setup">
      <div class='card-content'>
        <span class='badge'>CARANDDRIVER</span>
        <h3>Toyota Updates the Oddball Crown for 2027 with New Hybrid Setup</h3>
        <p>Toyota says the Crown XLE, Limited, and Nightshade get an updated hybrid system, but it&#x27;s being coy about the details of this revised setup.</p>
        <div class='card-tension'><b>Tension:</b> Manufacturer EV investment continues despite new EV market share slipping to 5.9%—a disconnect between strategy and sales.</div>
        <small>Read on caranddriver.com</small>
      </div>
    </div>
  </a>
  <a href="https://www.roadandtrack.com/news/a73257286/subaru-is-dedicating-a-team-to-making-its-cars-more-fun/" target="_blank">
    <div class='card'>
      <img src="https://hips.hearstapps.com/hmg-prod/images/2025-subaru-wrx-ts-4-67606dfa28b20.jpg?crop=1xw:0.75xh;0xw,0.25xh&amp;resize=1200:*" alt="Subaru Is Dedicating a Team to Making Its Cars More Fun">
      <div class='card-content'>
        <span class='badge'>ROADANDTRACK</span>
        <h3>Subaru Is Dedicating a Team to Making Its Cars More Fun</h3>
        <p>The new Sports Vehicle Planning Office is possible because of Subaru’s surging hybrid and EV sales.</p>
        <div class='card-tension'><b>Tension:</b> Manufacturer EV investment continues despite new EV market share slipping to 5.9%—a disconnect between strategy and sales.</div>
        <small>Read on roadandtrack.com</small>
      </div>
    </div>
  </a>
  <a href="https://www.motor1.com/news/802709/genesis-considering-pickup-truck/" target="_blank">
    <div class='card'>
      <img src="https://cdn.motor1.com/images/mgl/40YPGJ/s1/genesis-truck-rumor.jpg" alt="A Genesis Pickup Truck Could Be Back On The Table Thanks To Hyundai">
      <div class='card-content'>
        <span class='badge'>MOTOR1</span>
        <h3>A Genesis Pickup Truck Could Be Back On The Table Thanks To Hyundai</h3>
        <p>The idea of a Genesis pickup truck isn&#x27;t dead after all. In fact, it may be closer to reality than ever.</p>
        <div class='card-tension'><b>Tension:</b> Market realities often contradict headline announcements—dig deeper for the real story.</div>
        <small>Read on motor1.com</small>
      </div>
    </div>
  </a>
  <a href="https://www.thedrive.com/news/ban-on-chinese-tech-threatens-to-push-new-car-prices-even-higher" target="_blank">
    <div class='card'>
      <img src="https://www.thedrive.com/wp-content/uploads/2026/07/GettyImages-2255530896.jpg?quality=85&amp;amp;w=2048" alt="New Cars Would Get Even Pricier With Ban on Chinese Tech">
      <div class='card-content'>
        <span class='badge'>THEDRIVE</span>
        <h3>New Cars Would Get Even Pricier With Ban on Chinese Tech</h3>
        <p>One former Detroit auto executive said his &quot;jaw dropped&quot; when he saw how much pricier an equivalent non-China ADAS system would cost. The post New ...</p>
        <div class='card-tension'><b>Tension:</b> Manufacturer EV investment continues despite new EV market share slipping to 5.9%—a disconnect between strategy and sales.</div>
        <small>Read on thedrive.com</small>
      </div>
    </div>
  </a>
</div>

<!-- Motorsports Section -->
<div class='sec'>
  <h2>Motorsports</h2>
  <small><b>When Culture Thrives</b></small>
</div>

<div class='grid'>
  <a href="https://www.caranddriver.com/news/a73252090/days-of-thunder-reboot-details/" target="_blank">
    <div class='card'>
      <img src="https://hips.hearstapps.com/hmg-prod/images/fb1b9195-f7b2-436f-a223-b02c87098126.jpeg?crop=1.00xw:0.753xh;0,0.0612xh&amp;resize=1200:*" alt="&#x27;Days of Thunder&#x27; Reboot Inches Closer to the Start Line">
      <div class='card-content'>
        <span class='badge'>CARANDDRIVER</span>
        <h3>&#x27;Days of Thunder&#x27; Reboot Inches Closer to the Start Line</h3>
        <p>The classic 1990 NASCAR movie has Tom Cruise and Jerry Bruckheimer on board and is close to having a director.</p>
        <div class='card-tension'><b>Tension:</b> Performance culture thrives on track and in culture while consumers tighten budgets—passion persists amid economic strain.</div>
        <small>Read on caranddriver.com</small>
      </div>
    </div>
  </a>
  <a href="https://www.thedrive.com/news/leo-leclerc-caught-peeing-on-red-bulls-garage-is-peak-f1-shenanigans" target="_blank">
    <div class='card'>
      <img src="https://www.thedrive.com/wp-content/uploads/2026/07/GettyImages-2287438779.jpg?quality=85" alt="Leo Leclerc Caught Peeing on Red Bull’s Garage Is Peak F1 Shenanigans">
      <div class='card-content'>
        <span class='badge'>THEDRIVE</span>
        <h3>Leo Leclerc Caught Peeing on Red Bull’s Garage Is Peak F1 Shenanigans</h3>
        <p>Do you think that photo ended up in Max Verstappen&#x27;s inbox? Probably so. The post Leo Leclerc Caught Peeing on Red Bull’s Garage Is Peak F1 Shenani...</p>
        <div class='card-tension'><b>Tension:</b> Performance culture thrives on track and in culture while consumers tighten budgets—passion persists amid economic strain.</div>
        <small>Read on thedrive.com</small>
      </div>
    </div>
  </a>
</div>

<!-- Performance Builds Section -->
<div class='sec'>
  <h2>Performance Builds</h2>
  <small><b>Built Against the Odds</b></small>
</div>

<div class='grid'>
  <a href="https://www.caranddriver.com/news/a73256154/ford-bronco-bronco-raptor-engine-fire-recall/" target="_blank">
    <div class='card'>
      <img src="https://hips.hearstapps.com/hmg-prod/images/bronco-60th-anniversary-package-03-688d01c971d96.jpg?crop=0.731xw:0.547xh;0.155xw,0.257xh&amp;resize=1200:*" alt="Ford Recalls 565K Bronco, Bronco Raptor SUVs over Potential Engine Fires">
      <div class='card-content'>
        <span class='badge'>CARANDDRIVER</span>
        <h3>Ford Recalls 565K Bronco, Bronco Raptor SUVs over Potential Engine Fires</h3>
        <p>A problem with the engine compartment wiring harness could lead to a short circuit, creating a fire in the engine bay.</p>
        <div class='card-tension'><b>Tension:</b> Performance culture thrives on track and in culture while consumers tighten budgets—passion persists amid economic strain.</div>
        <small>Read on caranddriver.com</small>
      </div>
    </div>
  </a>
  <a href="https://www.thedrive.com/news/aston-martin-f1-rolls-out-significant-16-part-aero-upgrade-for-this-weekends-hungarian-gp" target="_blank">
    <div class='card'>
      <img src="https://www.thedrive.com/wp-content/uploads/2026/07/GettyImages-2287477178.jpg?quality=85" alt="Aston Martin F1 Rolls Out ‘Significant’ 16-Part Aero Upgrade for This Weekend’s Hungarian GP">
      <div class='card-content'>
        <span class='badge'>THEDRIVE</span>
        <h3>Aston Martin F1 Rolls Out ‘Significant’ 16-Part Aero Upgrade for This Weekend...</h3>
        <p>While the upgrades are quite promising on paper and in simulations, the AMR26 of Lance Stroll had to retire from FP1 with a broken suspension. The ...</p>
        <div class='card-tension'><b>Tension:</b> Performance culture thrives on track and in culture while consumers tighten budgets—passion persists amid economic strain.</div>
        <small>Read on thedrive.com</small>
      </div>
    </div>
  </a>
  <a href="https://www.thedrive.com/news/bad-door-handles-are-trapping-people-in-cars-the-feds-are-finally-stepping-in" target="_blank">
    <div class='card'>
      <img src="https://www.thedrive.com/wp-content/uploads/2026/07/GettyImages-2189374777.jpg?quality=85&amp;amp;w=2048" alt="Bad Door Handles Are Trapping People in Cars. The Feds Are Finally Stepping in">
      <div class='card-content'>
        <span class='badge'>THEDRIVE</span>
        <h3>Bad Door Handles Are Trapping People in Cars. The Feds Are Finally Stepping in</h3>
        <p>The National Highway Traffic Safety Administration aims to &quot;mandate a robust and obvious door egress system in all motor vehicles.&quot; The post Bad Do...</p>
        <div class='card-tension'><b>Tension:</b> Performance culture thrives on track and in culture while consumers tighten budgets—passion persists amid economic strain.</div>
        <small>Read on thedrive.com</small>
      </div>
    </div>
  </a>
  <a href="https://www.thedrive.com/news/ford-recalls-over-half-a-million-broncos-for-engine-fire-risk-tds" target="_blank">
    <div class='card'>
      <img src="https://www.thedrive.com/wp-content/uploads/2026/07/GettyImages-1233462832.jpg?quality=85&amp;amp;w=2048" alt="Ford Recalls Over Half a Million Broncos for Engine Fire Risk: TDS">
      <div class='card-content'>
        <span class='badge'>THEDRIVE</span>
        <h3>Ford Recalls Over Half a Million Broncos for Engine Fire Risk: TDS</h3>
        <p>Also, Honda is pausing production of its manual sport sedans and a few hundred Jeeps are being recalled for thin wheels. The post Ford Recalls Over...</p>
        <div class='card-tension'><b>Tension:</b> Performance culture thrives on track and in culture while consumers tighten budgets—passion persists amid economic strain.</div>
        <small>Read on thedrive.com</small>
      </div>
    </div>
  </a>
  <a href="https://www.theautopian.com/120-years-ago-these-were-the-cars-that-tried-to-cross-two-continents/" target="_blank">
    <div class='card'>
      <img src="https://images-stag.jazelc.com/uploads/theautopian-m2en/Race_to_the_Future_TS3.png" alt="120 Years Ago, These Wild Men Tried To Cross The Globe In Early Automobiles With Less Than 50 Horsepower">
      <div class='card-content'>
        <span class='badge'>THEAUTOPIAN</span>
        <h3>120 Years Ago, These Wild Men Tried To Cross The Globe In Early Automobiles W...</h3>
        <p>In January 1907 Le Matin, a Parisian newspaper, threw down a gauntlet to the world. What they proposed was an automobile race across two continents...</p>
        <div class='card-tension'><b>Tension:</b> Performance culture thrives on track and in culture while consumers tighten budgets—passion persists amid economic strain.</div>
        <small>Read on theautopian.com</small>
      </div>
    </div>
  </a>
</div>

<!-- Suppliers Section -->
<div class='sec'>
  <h2>Suppliers</h2>
  <small><b>Behind the Lines</b></small>
</div>

<div class='grid'>
  <a href="https://www.autonews.com/data-center/manufacturing-data/production-downtime/an-north-america-assembly-plant-downtime-072726/" target="_blank">
    <div class='card'>
      <img src="https://www.autonews.com/resizer/v2/TR2DA323XVAMFMMPAVKPO2ULS4.jpg?focal=2593%2C960&amp;amp;auth=10ebe786ad39816053b023bbae7807c94f0375a19b99bfde436449d27be01820&amp;amp;width=3648&amp;amp;height=2052" alt="North America production downtime – 07/27/26">
      <div class='card-content'>
        <span class='badge'>AUTONEWS</span>
        <h3>North America production downtime – 07/27/26</h3>
        <p>North America car and truck assembly plant downtime for the current week</p>
        <div class='card-tension'><b>Tension:</b> Market realities often contradict headline announcements—dig deeper for the real story.</div>
        <small>Read on autonews.com</small>
      </div>
    </div>
  </a>
</div>

<!-- Dealer News Section -->
<div class='sec'>
  <h2>Dealer News</h2>
  <small><b>At the Point of Sale</b></small>
</div>

<div class='grid'>
  <a href="https://www.autonews.com/retail/an-penske-mitsui-private-shareholders-0724/" target="_blank">
    <div class='card'>
      <img src="https://www.autonews.com/resizer/v2/AEZ4XZVL4VF3XMXIZSIVES2RUM.jpg?auth=0140ccfb2b1b7f0236a29a91ba57977f483c0505f9071767aaf2774ef29a59a9#.jpg" alt="Why minority shareholder opinion matters in bid to take Penske Automotive private">
      <div class='card-content'>
        <span class='badge'>AUTONEWS</span>
        <h3>Why minority shareholder opinion matters in bid to take Penske Automotive pri...</h3>
        <p>Penske Corp. owns the majority of Penske Automotive Group Inc. shares, but it&#x27;s likely to listen to investors who own the 28 percent of stock Pensk...</p>
        <div class='card-tension'><b>Tension:</b> Market realities often contradict headline announcements—dig deeper for the real story.</div>
        <small>Read on autonews.com</small>
      </div>
    </div>
  </a>
  <a href="https://www.autonews.com/retail/an-penske-mitsui-private-public-dealers-0724/" target="_blank">
    <div class='card'>
      <img src="https://www.autonews.com/resizer/v2/TR2DA323XVAMFMMPAVKPO2ULS4.jpg?auth=10ebe786ad39816053b023bbae7807c94f0375a19b99bfde436449d27be01820&amp;width=1200#.jpg" alt="Why other public dealership groups are unlikely to follow if Penske Automotive goes private">
      <div class='card-content'>
        <span class='badge'>AUTONEWS</span>
        <h3>Why other public dealership groups are unlikely to follow if Penske Automotiv...</h3>
        <p>Penske Corp. and Mitsui&#x27;s $3.8 billion bid to take Penske Automotive private is unlikely to spark similar moves among the five other major public f...</p>
        <div class='card-tension'><b>Tension:</b> Market realities often contradict headline announcements—dig deeper for the real story.</div>
        <small>Read on autonews.com</small>
      </div>
    </div>
  </a>
  <a href="https://www.wardsauto.com/news/penske-and-mitsui-seek-to-take-penske-auto-private-in-38b-deal/826024/" target="_blank">
    <div class='card'>
      <img src="https://imgproxy.divecdn.com/jWhcd8f-pphdtAy9nzx7cXfFYK8SqtjQuevbSKJQx_M/g:ce/rs:fit:770:435/Z3M6Ly9kaXZlc2l0ZS1zdG9yYWdlL2RpdmVpbWFnZS9BbmdsZWQtRWxldmF0aW9uLVZpZXdfdE1EQjVPSC5qcGc=.webp" alt="Penske and Mitsui seek to take Penske Auto private in $3.8B deal">
      <div class='card-content'>
        <span class='badge'>WARDSAUTO</span>
        <h3>Penske and Mitsui seek to take Penske Auto private in $3.8B deal</h3>
        <p>Two current owners of global retailer Penske Automotive Group are offering $210 a share, subject to shareholder and regulatory approval.</p>
        <div class='card-tension'><b>Tension:</b> Market realities often contradict headline announcements—dig deeper for the real story.</div>
        <small>Read on wardsauto.com</small>
      </div>
    </div>
  </a>
  <a href="https://www.caranddriver.com/news/a73258248/subaru-getaway-production-delayed/" target="_blank">
    <div class='card'>
      <img src="https://hips.hearstapps.com/hmg-prod/images/ce88f837-8f55-406a-a575-f963025e0bcb.jpg?crop=1.00xw:0.753xh;0,0.165xh&amp;resize=1200:*" alt="Subaru Delays Its Most Powerful Model Yet, the 420-HP Getaway SUV">
      <div class='card-content'>
        <span class='badge'>CARANDDRIVER</span>
        <h3>Subaru Delays Its Most Powerful Model Yet, the 420-HP Getaway SUV</h3>
        <p>The Getaway was supposed to arrive at dealerships in late 2026, but may not show up until 2027 as Subaru follows Toyota in delaying its three-row EV.</p>
        <div class='card-tension'><b>Tension:</b> Market realities often contradict headline announcements—dig deeper for the real story.</div>
        <small>Read on caranddriver.com</small>
      </div>
    </div>
  </a>
</div>

<!-- Industry News Section -->
<div class='sec'>
  <h2>Industry News</h2>
  <small><b>Market Signals</b></small>
</div>

<div class='grid'>
  <a href="https://www.kbb.com/car-news/2027-volvo-ex60-rated-at-330-miles-of-range/" target="_blank">
    <div class='card'>
      <img src="https://dam.coxautoinc.com/asset/7e7be64c-a500-4a2d-970c-46d75bb47b1e/OG/2027-volvo-ex-60-front-qtr.jpg" alt="2027 Volvo EX60 Rated at 330 Miles of Range">
      <div class='card-content'>
        <span class='badge'>KBB</span>
        <h3>2027 Volvo EX60 Rated at 330 Miles of Range</h3>
        <p>The 2027 Volvo EX60 midsize SUV has an EPA-rated range of 330 miles.</p>
        <div class='card-tension'><b>Tension:</b> Market realities often contradict headline announcements—dig deeper for the real story.</div>
        <small>Read on kbb.com</small>
      </div>
    </div>
  </a>
  <a href="https://www.theautopian.com/we-need-to-discuss-the-lemon-situation-tales-from-the-slack/" target="_blank">
    <div class='card'>
      <img src="https://images-stag.jazelc.com/uploads/theautopian-m2en/Tales_From_The_Slack_Lemons_TS.jpg" alt="We Need To Discuss The Lemon Situation: Tales From The Slack">
      <div class='card-content'>
        <span class='badge'>THEAUTOPIAN</span>
        <h3>We Need To Discuss The Lemon Situation: Tales From The Slack</h3>
        <p>Oh, snap! You gotta be a Member to enjoy this sweet, sweet content. Why not join today? Click here, or on the graphic! The post We Need To Discuss ...</p>
        <div class='card-tension'><b>Tension:</b> Market realities often contradict headline announcements—dig deeper for the real story.</div>
        <small>Read on theautopian.com</small>
      </div>
    </div>
  </a>
  <a href="https://electrek.co/2026/07/24/a-1-2-gw-solar-farm-is-rising-at-a-texas-coal-site-but-coal-is-staying/" target="_blank">
    <div class='card'>
      <img src="https://i0.wp.com/electrek.co/wp-content/uploads/sites/3/2026/07/Twin-Oaks-Power-Station.jpg?resize=1200%2C628&amp;quality=82&amp;strip=all&amp;ssl=1" alt="A 1.2 GW solar farm is rising at a Texas coal site – but coal is staying">
      <div class='card-content'>
        <span class='badge'>ELECTREK</span>
        <h3>A 1.2 GW solar farm is rising at a Texas coal site – but coal is staying</h3>
        <p>One of North America’s biggest coal-site solar projects is now under construction in Texas – but the coal plant next door isn’t going anywhere. Her...</p>
        <div class='card-tension'><b>Tension:</b> Market realities often contradict headline announcements—dig deeper for the real story.</div>
        <small>Read on electrek.co</small>
      </div>
    </div>
  </a>
  <a href="https://cleantechnica.com/2026/07/24/trump-administration-admits-retaliatory-grant-cancellations/" target="_blank">
    <div class='card'>
      <img src="https://cleantechnica.com/wp-content/uploads/2023/04/Judge-Gavel-Court-CleanTechnica-Watermark.png" alt="Trump Administration Admits Retaliatory Grant Cancellations">
      <div class='card-content'>
        <span class='badge'>CLEANTECHNICA</span>
        <h3>Trump Administration Admits Retaliatory Grant Cancellations</h3>
        <p>Washington, D.C. — Today, the New York Times uncovered recent court filings where the Trump administration admitted to targeting states that voted ...</p>
        <div class='card-tension'><b>Tension:</b> Market realities often contradict headline announcements—dig deeper for the real story.</div>
        <small>Read on cleantechnica.com</small>
      </div>
    </div>
  </a>
</div>

<footer>
  <p>
    <span class='stat'>65 Stories</span>
    <span class='stat'>11 Publishers</span>
    <span class='stat'>~48 min read</span>
  </p>
  <p>Issue #002 | July 25, 2026</p>
  <p style="color:#555;margin-top:20px">AutoIntel.News reveals market contradictions behind automotive headlines. We highlight tensions between announcements and reality, strategy and execution, OEM plans and buyer behavior. All links open in new tabs.</p>
</footer>

</div>

</body>
</html>
