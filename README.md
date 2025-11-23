[index.html.html](https://github.com/user-attachments/files/23699162/index.html.html)
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Baw Baw Animal Rescue Inc.</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <style>
    :root {
      --green: #2b5f4a; /* logo green */
      --cream: #fffdf8;
      --ink: #222;
      --radius: 16px;
      --shadow: 0 6px 18px rgba(0,0,0,.08);
      --max: 1100px;
    }
    body {
      margin:0; font-family: "Segoe UI", system-ui, sans-serif;
      background: var(--cream); color: var(--ink); line-height:1.6;
    }
    header {
      background:#fff; border-bottom:1px solid #eee; position:sticky; top:0; z-index:50;
    }
    .nav {
      max-width:var(--max); margin:0 auto; padding:14px 20px;
      display:flex; align-items:center; justify-content:space-between;
    }
    .brand { display:flex; align-items:center; gap:12px; text-decoration:none; color:var(--green); font-weight:800 }
    .brand img { height:44px }
    nav a { margin:0 8px; text-decoration:none; color:var(--green); font-weight:600 }
    h1,h2,h3 { color:var(--green); margin-top:0 }
    section { max-width:var(--max); margin:0 auto; padding:60px 20px }
    .hero { text-align:center; padding:80px 20px }
    .hero img { max-width:160px; margin-bottom:20px }
    .grid { display:grid; gap:20px }
    @media(min-width:760px){ .cols-2{grid-template-columns:1fr 1fr} .cols-3{grid-template-columns:repeat(3,1fr)} }
    .card { background:#fff; border-radius:var(--radius); box-shadow:var(--shadow); padding:18px }
    .pet img { width:100%; border-radius:var(--radius) }
    footer { text-align:center; padding:40px 20px; background:#fafafa; color:#555 }
  </style>
</head>
<body>

<header>
  <div class="nav">
    <a class="brand" href="#home">
      <img src="logo.jpeg" alt="Baw Baw Animal Rescue logo">
      <span>Baw Baw Animal Rescue Inc.</span>
    </a>
    <nav>
      <a href="#home">Home</a>
      <a href="#adopt">Adopt</a>
      <a href="#donate">Donate</a>
      <a href="#gallery">Gallery</a>
      <a href="#contact">Contact</a>
    </nav>
  </div>
</header>

<section id="home" class="hero">
  <img src="logo.jpeg" alt="Rescue logo">
  <h1>From goldfish to roo, it all starts with you</h1>
  <p>We’re a volunteer‑run nonprofit caring for animals across the Baw Baw region. Compassion guides everything we do.</p>
</section>

<section id="adopt">
  <h2>Adopt a Friend</h2>
  <div class="grid cols-3">
    <div class="card pet">
      <img src="kangaroo.jpeg" alt="Kangaroo">
      <h3>Koda</h3>
      <p>Playful kangaroo who loves bush walks.</p>
    </div>
    <div class="card pet">
      <img src="koala.jpeg" alt="Koala">
      <h3>Rosie</h3>
      <p>Gentle koala mum with her joey.</p>
    </div>
    <div class="card pet">
      <img src="sugarglider.jpeg" alt="Sugar glider">
      <h3>Whiskers</h3>
      <p>Curious sugar glider looking for a safe home.</p>
    </div>
  </div>
</section>

<section id="donate">
  <h2>Donate</h2>
  <div class="grid cols-3">
    <div class="card"><h3>$25</h3><p>Vaccinations and supplies.</p></div>
    <div class="card"><h3>$50</h3><p>Food and enrichment toys.</p></div>
    <div class="card"><h3>$100</h3><p>Vet check and transport.</p></div>
  </div>
</section>

<section id="gallery">
  <h2>Wildlife Gallery</h2>
  <div class="grid cols-3">
    <div><img src="echidna.jpeg" alt="Echidna"></div>
    <div><img src="galah.jpeg" alt="Galah"></div>
    <div><img src="kookaburra.jpeg" alt="Kookaburra"></div>
    <div><img src="camel.jpeg" alt="Camel"></div>
    <div><img src="lizard.jpeg" alt="Lizard"></div>
    <div><img src="kangaroo-road.jpeg" alt="Kangaroo crossing road"></div>
  </div>
</section>

<section id="contact">
  <h2>Contact Us</h2>
  <div class="grid cols-2">
    <div class="card">
      <p><b>Email:</b> info@bawbawanimalrescue.org</p>
      <p><b>Facebook:</b> @BawBawAnimalRescue</p>
      <p><b>Instagram:</b> @BawBawRescue</p>
    </div>
    <div class="card">
      <p>Want to adopt, donate, or volunteer? Reach out and we’ll connect you with the right team.</p>
    </div>
  </div>
</section>

<footer>
  <p>&copy; 2025 Baw Baw Animal Rescue Inc.</p>
</footer>

</body>
</html>
