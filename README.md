[index.html.html](https://github.com/user-attachments/files/23699182/index.html.html)
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Baw Baw Animal Rescue Inc.</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <meta name="description" content="From goldfish to roo, it all starts with you. Adopt, donate, and help save lives across the Baw Baw region.">
  <style>
    :root{
      --green:#2b5f4a; /* only use logo green for headings/accents */
      --cream:#fffdf8;
      --ink:#222;
      --radius:16px;
      --shadow:0 8px 24px rgba(0,0,0,.08);
      --max:1100px;
    }
    *{box-sizing:border-box}
    html,body{margin:0;padding:0}
    body{
      font-family: "Segoe UI", system-ui, -apple-system, Roboto, Arial, "Helvetica Neue", "Noto Sans";
      background:var(--cream);
      color:var(--ink);
      line-height:1.65;
    }
    header{position:sticky; top:0; z-index:50; background:#fff; border-bottom:1px solid #eee}
    .nav{
      max-width:var(--max); margin:0 auto; padding:14px 20px;
      display:flex; align-items:center; justify-content:space-between;
    }
    .brand{display:flex; align-items:center; gap:12px; text-decoration:none; color:var(--green); font-weight:800}
    .brand img{height:44px; width:auto}
    nav a{margin:0 8px; text-decoration:none; color:var(--green); font-weight:600}
    section{max-width:var(--max); margin:0 auto; padding:60px 20px}
    h1,h2,h3{color:var(--green); margin-top:0}
    .hero{text-align:center; padding:80px 20px}
    .hero img{max-width:180px; margin-bottom:20px}
    .lead{color:#4a4a4a}
    .grid{display:grid; gap:22px}
    @media(min-width:760px){
      .cols-2{grid-template-columns:1fr 1fr}
      .cols-3{grid-template-columns:repeat(3,1fr)}
    }
    .card{background:#fff; border-radius:var(--radius); box-shadow:var(--shadow); padding:18px}
    .pet img{width:100%; border-radius:var(--radius)}
    .gallery img{width:100%; border-radius:var(--radius)}
    .btn{display:inline-block; text-decoration:none; color:var(--green); font-weight:700; border:2px solid var(--green); border-radius:12px; padding:10px 14px}
    footer{text-align:center; padding:40px 20px; background:#fafafa; color:#555}
  </style>
</head>
<body>

  <!-- Header -->
  <header>
    <div class="nav">
      <a class="brand" href="#home">
        <img src="1EcTJah7LbS2wgiVDcszm.jpeg" alt="Baw Baw Animal Rescue logo">
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

  <!-- Home -->
  <section id="home" class="hero">
    <img src="1EcTJah7LbS2wgiVDcszm.jpeg" alt="Rescue heart logo">
    <h1>From goldfish to roo, it all starts with you</h1>
    <p class="lead">We’re a volunteer‑run nonprofit caring for animals across the Baw Baw region. Compassion guides everything we do.</p>
    <p><a class="btn" href="#adopt">See adoptable animals</a> <a class="btn" href="#donate">Support our work</a></p>
  </section>

  <!-- Adopt -->
  <section id="adopt">
    <h2>Adopt a friend</h2>
    <p class="lead">When you adopt, you change a life — yours and theirs.</p>
    <div class="grid cols-3" style="margin-top:16px">
      <div class="card pet">
        <img src="bLtdkPWC2J1zoC27w8oYT.jpeg" alt="Kangaroo in bushland">
        <h3>Koda</h3>
        <p>Playful spirit with a calm temperament. Loves bush walks.</p>
        <p><a class="btn" href="#contact">Enquire</a></p>
      </div>
      <div class="card pet">
        <img src="K5dmWNP7cCs3gv8CjF5zn.jpeg" alt="Koala with joey">
        <h3>Rosie & Joey</h3>
        <p>Gentle duo seeking a safe habitat and attentive care.</p>
        <p><a class="btn" href="#contact">Enquire</a></p>
      </div>
      <div class="card pet">
        <img src="KEc9hYqHSL85AcMYrtmkH.jpeg" alt="Sugar glider peeking from hollow">
        <h3>Whiskers</h3>
        <p>Curious and social — perfect for experienced carers.</p>
        <p><a class="btn" href="#contact">Enquire</a></p>
      </div>
    </div>
  </section>

  <!-- Donate -->
  <section id="donate">
    <h2>Donate</h2>
    <p class="lead">Your generosity funds vet care, food, transport, and rehabilitation.</p>
    <div class="grid cols-3" style="margin-top:16px">
      <div class="card">
        <h3>$25</h3>
        <p>Vaccinations and basic supplies.</p>
        <p><a class="btn" href="#contact">Donate $25</a></p>
      </div>
      <div class="card">
        <h3>$50</h3>
        <p>Food for a week and enrichment toys.</p>
        <p><a class="btn" href="#contact">Donate $50</a></p>
      </div>
      <div class="card">
        <h3>$100</h3>
        <p>Vet check and intake transport.</p>
        <p><a class="btn" href="#contact">Donate $100</a></p>
      </div>
    </div>
    <p class="lead" style="margin-top:10px">Replace these buttons with your real donation link when ready (PayPal, Stripe, or GiveNow).</p>
  </section>

  <!-- Gallery -->
  <section id="gallery">
    <h2>Wildlife gallery</h2>
    <p class="lead">A glimpse of the lives you help protect.</p>
    <div class="grid cols-3 gallery" style="margin-top:16px">
      <div><img src="xif4imEepz5HNbkmNdZQ6.jpeg" alt="Kangaroos at sunset"></div>
      <div><img src="epkVj41Hamc7ybDeirPdT.jpeg" alt="Galah on railing"></div>
      <div><img src="Fn6erJVLnfkUVVUDE3Fyh.jpeg" alt="Kookaburra on branch"></div>
      <div><img src="sJQbWgVav4SeqXaaud1DQ.jpeg" alt="Echidna close-up"></div>
      <div><img src="NhiXtycmBmgoH1k27tLBN.jpeg" alt="Lizard on rock"></div>
      <div><img src="7D7Vam3Pn74WwxA9Z6haz.webp" alt="Camel in semi-arid landscape"></div>
      <div><img src="1hAEEeNtkZPeeU5PjxeKY.jpeg" alt="Koala climbing a tree"></div>
      <div><img src="RFi5BbBEW5VTJXbPL77ti.jpeg" alt="Kangaroo crossing rural road"></div>
    </div>
  </section>

  <!-- Contact -->
  <section id="contact">
    <h2>Contact us</h2>
    <div class="grid cols-2" style="margin-top:12px">
      <div class="card">
        <p><b style="color:var(--green)">Email:</b> info@bawbawanimalrescue.org</p>
        <p><b style="color:var(--green)">Facebook:</b> @BawBawAnimalRescue</p>
        <p><b style="color:var(--green)">Instagram:</b> @BawBawRescue</p>
        <img src="1EcTJah7LbS2wgiVDcszm.jpeg" alt="Baw Baw Animal Rescue heart logo" style="margin-top:10px; max-width:160px">
      </div>
      <div class="card">
        <p>Want to adopt, donate, or volunteer? Reach out and we’ll connect you with the right team.</p>
        <p class="lead">For emergencies, contact local wildlife services and your nearest vet.</p>
      </div>
    </div>
  </section>

  <footer>
    <p>&copy; 2025 Baw Baw Animal Rescue Inc.</p>
  </footer>

</body>
</html>
