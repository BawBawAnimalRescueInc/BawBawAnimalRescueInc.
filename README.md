[index.html.html](https://github.com/user-attachments/files/23699276/index.html.html)
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Baw Baw Animal Rescue Inc.</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <meta name="description" content="From goldfish to roo, it all starts with you. Baw Baw Animal Rescue Inc. — adopt, donate, join as a member, and help save lives.">
  <!-- Google Fonts -->
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;800&display=swap" rel="stylesheet">
  <style>
    :root{
      --green:#2b5f4a;   /* dark green from logo */
      --beige:#f5f0e6;   /* warm beige background */
      --white:#ffffff;
      --radius:16px;
      --shadow:0 6px 18px rgba(0,0,0,.12);
      --max:1100px;
    }
    *{box-sizing:border-box}
    html,body{margin:0;padding:0}
    body{
      font-family: 'Poppins', sans-serif;
      background:var(--beige);
      color:var(--green);
      line-height:1.7;
    }
    img{max-width:100%; display:block; border-radius:12px}

    header{
      position:sticky; top:0; z-index:50;
      background:var(--white);
      border-bottom:1px solid rgba(0,0,0,.1);
    }
    .nav{
      max-width:var(--max); margin:0 auto; padding:14px 20px;
      display:flex; align-items:center; justify-content:space-between;
    }
    .brand{display:flex; align-items:center; gap:12px; text-decoration:none; color:var(--green); font-weight:800}
    .brand img{height:44px}
    nav a{margin:0 8px; text-decoration:none; color:var(--green); font-weight:600}
    .hamburger{display:none; border:none; background:transparent; color:var(--green); font-weight:800}
    @media(max-width:900px){
      .menu{display:none}
      .hamburger{display:block}
      .menu.open{display:flex; gap:8px; flex-wrap:wrap; margin-top:10px}
    }

    section{max-width:var(--max); margin:0 auto; padding:60px 20px}
    h1,h2,h3{color:var(--green); margin:0 0 10px}
    .lead{opacity:.9}

    .hero{text-align:center; padding:80px 20px}
    .hero img{max-width:160px; margin-bottom:20px}
    .motto{display:inline-block; font-weight:800; border:2px solid var(--green); border-radius:999px; padding:10px 14px}

    .grid{display:grid; gap:22px}
    @media(min-width:760px){
      .cols-2{grid-template-columns:1fr 1fr}
      .cols-3{grid-template-columns:repeat(3,1fr)}
    }

    .card{background:var(--white); border-radius:var(--radius); box-shadow:var(--shadow); padding:18px}
    .btn{display:inline-block; text-decoration:none; color:var(--green); font-weight:700; border:2px solid var(--green); border-radius:12px; padding:10px 14px}

    footer{background:var(--white); border-top:1px solid rgba(0,0,0,.1); text-align:center; padding:40px 20px; color:var(--green)}
  </style>
</head>
<body>

<header>
  <div class="nav">
    <a class="brand" href="#home">
      <img src="kk9cNDHnLzbKu35pMfcgu.jpeg" alt="Baw Baw Animal Rescue logo">
      <span>Baw Baw Animal Rescue Inc.</span>
    </a>
    <button class="hamburger" onclick="toggleMenu()">Menu</button>
    <nav id="menu" class="menu">
      <a href="#home">Home</a>
      <a href="#adopt">Adopt</a>
      <a href="#donate">Donate</a>
      <a href="#membership">Membership</a>
      <a href="#gallery">Gallery</a>
      <a href="#contact">Contact</a>
    </nav>
  </div>
</header>

<section id="home" class="hero">
  <img src="36qRwJD4q5cF9nRT1YChg.jpeg" alt="Rescue logo">
  <h1>From goldfish to roo, it all starts with you</h1>
  <p class="lead">We’re a volunteer‑run nonprofit caring for animals across the Baw Baw region. Compassion guides everything we do.</p>
  <p style="margin-top:14px"><span class="motto">Rescue • Rehabilitate • Rehome</span></p>
</section>

<section id="adopt">
  <h2>Adopt a friend</h2>
  <div class="grid cols-3" style="margin-top:16px">
    <div class="card">
      <img src="UMcsUcg72hYVcpZonV32m.jpeg" alt="Kangaroos">
      <h3>Koda</h3>
      <p>Playful kangaroo who loves bush walks.</p>
    </div>
    <div class="card">
      <img src="3f8wjdG3wsZQ29612HdAA.jpeg" alt="Koalas">
      <h3>Rosie & Joey</h3>
      <p>Gentle duo seeking a safe habitat and attentive care.</p>
    </div>
    <div class="card">
      <img src="i6dun9qHeT6eSDCt8fAgZ.jpeg" alt="Sugar glider">
      <h3>Whiskers</h3>
      <p>Curious and social — perfect for experienced carers.</p>
    </div>
  </div>
</section>

<section id="donate">
  <h2>Donate</h2>
  <div class="grid cols-3" style="margin-top:16px">
    <div class="card"><h3>$25</h3><p>Vaccinations and supplies.</p></div>
    <div class="card"><h3>$50</h3><p>Food and enrichment toys.</p></div>
    <div class="card"><h3>$100</h3><p>Vet check and transport.</p></div>
  </div>
</section>

<section id="membership">
  <h2>Membership</h2>
  <div class="grid cols-3" style="margin-top:16px">
    <div class="card"><h3>Individual — $25</h3><p>Supports one rescued animal.</p></div>
    <div class="card"><h3>Family — $45</h3><p>Supports multiple animals and includes family updates.</p></div>
    <div class="card"><h3>Sponsor — $80</h3><p>Name recognition and sponsor updates.</p></div>
  </div>
</section>

<section id="gallery">
  <h2>Wildlife gallery</h2>
  <div class="grid cols-3" style="margin-top:16px">
    <div><img src="SBTgmrBdAtLS1AVGFFBw3.jpeg" alt="Kangaroos at sunset"></div>
    <div><img src="17pE61thU9GysXennv6Cu.jpeg" alt="Galah"></div>
    <div><img src="Vkb53e77RixsHYGBCLkTh.jpeg" alt="Kookaburra"></div>
    <div><img src="2SAhXFqv5Tk7bd3TfSRo2.jpeg" alt="Echidna"></div>
    <div><img src="EorNVftjQKAjoKPD7WC1M.jpeg" alt="Lizard"></div>
    <div><img src="A2s7nSLzqfiJVrgmAFXJY.webp" alt="Camel"></div>
    <div><img src="E33pPsfmnRxnaABPi2YVK.jpeg" alt="Koala climbing"></div>
    <div><img src="8jvVDbK7Hf32LUfCZbCba.jpeg" alt="Kangaroo crossing road"></div>
  </div>
</section>

<section id="contact">
  <h2>Contact us</h2>
  <div class="grid cols-2" style="margin-top:12px">
