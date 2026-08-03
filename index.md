<html lang="en">
<head>
<meta charset='utf-8'>
<meta name='viewport' content='width=device-width,initial-scale=1'>
<meta name='description' content='AutoIntel.News is currently undergoing maintenance. Check back soon for automotive industry intelligence.'>
<title>AutoIntel.News - Check Back Soon</title>
<style>
body{
  margin:0;
  background:#0f0f10;
  color:#eee;
  font-family:Arial,sans-serif;
  font-size:16px;
  line-height:1.6;
  min-height:100vh;
  display:flex;
  flex-direction:column
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
header h1 .car-symbol{
  font-style:italic;
  color:#f60;
  font-family:Times,'Times New Roman',serif
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
  margin:15px 0 0 0
}
.wrap{
  max-width:700px;
  margin:auto;
  padding:24px;
  flex-grow:1;
  display:flex;
  align-items:center;
  justify-content:center
}
.card{
  background:#1b1b1b;
  border-radius:14px;
  border:1px solid #2a2a2a;
  border-left:5px solid #f60;
  padding:48px 40px;
  text-align:center;
  box-shadow:0 4px 12px rgba(0,0,0,0.3)
}
.badge{
  background:#f60;
  color:#fff;
  padding:6px 14px;
  border-radius:999px;
  font-size:11px;
  font-weight:bold;
  display:inline-block;
  margin-bottom:20px;
  letter-spacing:0.5px
}
.card h2{
  margin:0 0 16px 0;
  font-size:28px;
  color:#fff;
  line-height:1.3
}
.card p{
  margin:0 0 18px 0;
  font-size:15px;
  color:#ccc;
  line-height:1.6
}
.card-tension{
  margin-top:20px;
  padding-top:18px;
  border-top:1px solid #2a2a2a;
  font-size:13px;
  color:#f60;
  font-style:italic;
  line-height:1.5
}
.gear{
  font-size:42px;
  color:#f60;
  display:inline-block;
  margin-bottom:20px;
  animation:spin 6s linear infinite
}
@keyframes spin{
  from{transform:rotate(0deg)}
  to{transform:rotate(360deg)}
}
@media(prefers-reduced-motion:reduce){
  .gear{animation:none}
}
footer{
  text-align:center;
  padding:30px;
  color:#666;
  font-size:13px
}
@media(max-width:768px){
  header{padding:20px}
  header h1{font-size:32px}
  .card{padding:32px 24px}
  .card h2{font-size:22px}
}
</style>
</head>
<body>

<header>
  <div class='date-field' id='publishDate'></div>
  <h1>AutoIntel.News <span class='car-symbol'>ō͡≡o˞̶</span></h1>
  <p class='tagline'>Automotive Intelligence. Curated Daily.</p>
</header>

<div class='wrap'>
  <div class='card'>
    <span class='badge'>UNDER MAINTENANCE</span>
    <div class='gear'>⚙</div>
    <h2>We're tuning up the engine.</h2>
    <p>AutoIntel.News is offline briefly while we update today's intelligence. Fresh stories, tensions, and analysis will be back shortly.</p>
    <div class='card-tension'><b>The Tension:</b> Even the best newsroom needs a pit stop now and then.</div>
  </div>
</div>

<footer>
  <p>Check back soon. &mdash; AutoIntel.News</p>
</footer>

<script>
document.getElementById('publishDate').textContent = new Date().toLocaleDateString('en-US', {weekday:'long',year:'numeric',month:'long',day:'numeric'}).toUpperCase();
</script>

</body>
</html>
