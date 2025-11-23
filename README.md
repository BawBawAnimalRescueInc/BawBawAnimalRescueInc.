[index.html.html](https://github.com/user-attachments/files/23699240/index.html.html)
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Baw Baw Animal Rescue Inc.</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <meta name="description" content="Baw Baw Animal Rescue Inc. — From goldfish to roo, it all starts with you. Adopt, donate, join as a member, and help save lives.">
  <style>
    /* ===== Brand style (matches your screenshot and logo) ===== */
    :root{
      --green:#2b5f4a;         /* dark green from the logo for ALL text */
      --cream:#fffdf5;         /* soft cream page background */
      --white:#ffffff;
      --radius:16px;
      --shadow:0 8px 24px rgba(0,0,0,.08);
      --max:1100px;
    }

    /* Base */
    *{box-sizing:border-box}
    html,body{margin:0;padding:0}
    body{
      font-family: "Segoe UI", system-ui, -apple-system, Roboto, Arial, "Helvetica Neue", "Noto Sans";
      background:var(--cream);
      color:var(--green);     /* all writing uses the dark green */
      line-height:1.7;
    }
    img{max-width:100%; display:block; border-radius:12px}

    /* Top navigation (clean like your inspo) */
    header{
      position:sticky; top:0; z-index:50;
      background:rgba(255,255,255,0.85);
      backdrop-filter: saturate(1.2) blur(8px);
      border-bottom:1px solid rgba(0,0,0,.06);
    }
    .nav{
      max-width:var(--max); margin:0 auto; padding:14px 20px;
      display:flex; align-items:center; justify-content:space-between;
    }
    .brand{
      display:flex; align-items:center; gap:12px; text-decoration:none; color:var(--green); font-weight:800;
    }
    .brand img{height:42px; width:auto; border-radius:8px}
    nav a{
      text-decoration:none; color:var(--green); font-weight:700; padding:8px 10px; border-radius:10px;
    }
    .hamburger{ display:none; border:none; background:transparent; color:var(--green); font-weight:800 }
    @media(max-width:900px){
      .menu{ display:none }
      .hamburger{ display:block }
      .menu.open{ display:flex; gap:8px; flex-wrap:wrap; margin-top:10px }
    }

    /* Sections */
    section{ max-width:var(--max); margin:0 auto; padding:60px 20px }
    h1,h2,h3{ color:var(--green); margin:0 0 10px }
    .lead{ opacity:.9 }

    /* Hero: centered, spacious, logo + motto */
    .hero{
      text-align:center; padding:80px 20px;
    }
    .hero .logo-row{
      display:flex; align-items:center; justify-content:center; gap:14px; margin-bottom:16px;
    }
    .hero .logo-row img{ height:54px; width:auto }
    .motto{
      display:inline-block; font-weight:800;
      border:2px solid var(--green); border-radius:999px; padding:10px 14px;
    }

    /* Simple grid utilities */
    .grid{ display:grid; gap:22px }
    @media(min-width:760px){
      .cols-2{ grid-template-columns: 1fr 1fr }
      .cols-3{ grid-template-columns: repeat(3, 1fr) }
      .cols-4{ grid-template-columns: repeat(4, 1fr) }
    }

    /* Cards: clean, airy */
    .card{
      background:var(--white);
      border:1px solid rgba(0,0,0,.08);
      border-radius:var(--radius);
      box-shadow:var(--shadow);
      padding:18px;
    }

    /* Buttons: outline, green text only */
    .btn{
      display:inline-block; text-decoration:none; color:var(--green); font-weight:800;
      border:2px solid var(--green); border-radius:12px; padding:10px 14px;
    }

    /* Footer */
    footer{
      background:#fff; border-top:1px solid rgba(0,0,0,.06);
      text-align:center; padding:40px 20px; color:var(--green);
    }
  </style>
</head>
<body>

  <!-- Navigation -->
  <header>
    <div class="nav">
      <a class="brand" href="#home" aria-label="Baw Baw Animal Rescue home">
        <img src="97E1EL6N8tTR5ddBFHi9g.jpeg" alt="Baw Baw Animal Rescue logo">
        <span>Baw Baw Animal Rescue Inc.</span>
      </a>
      <button class="hamburger" aria-label="Open menu" onclick="toggleMenu()">Menu</button>
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

  <!-- Home -->
  <section id="home" class="hero">
    <div class="logo-row">
      <img src="97E1EL6N8tTR5ddBFHi9g.jpeg" alt="Logo 1">
      <img src="4JVVjiT1BMWgpH3C6StWc.jpeg" alt="Logo 2">
    </div>
    <h1>From goldfish to roo, it all starts with you</h1>
    <p class="lead">We’re a volunteer‑run nonprofit caring for animals across the Baw Baw region. Compassion guides everything we do.</p>
    <p style="margin-top:14px">
      <span class="motto">Rescue • Rehabilitate • Rehome</span>
    </p>
    <p style="margin-top:18px">
      <a class="btn" href="#adopt">See adoptable animals</a>
      <a class="btn" href="#donate" style="margin-left:10px">Support our work</a>
    </p>
  </section>

  <!-- Adopt -->
  <section id="adopt">
    <h2>Adopt a friend</h2>
    <p class="lead">When you adopt, you change a life — yours and theirs.</p>
    <div class="grid cols-3" style="margin-top:16px">
      <div class="card">
        <img src="P6WuHSBd9MRcANXqtLszc.jpeg" alt="Kangaroos in bushland">
        <h3>Koda</h3>
        <p>Playful spirit with a calm temperament. Loves bush walks.</p>
        <p><a class="btn" href="#contact">Enquire</a></p>
      </div>
      <div class="card">
        <img src="tHcFUbByo9fhunkYCzLY8.jpeg" alt="Koala with joey">
        <h3>Rosie & Joey</h3>
        <p>Gentle duo seeking a safe habitat and attentive care.</p>
        <p><a class="btn" href="#contact">Enquire</a></p>
      </div>
      <div class="card">
        <img src="YZTGPm7G1mBPrmgPzKMDw.jpeg" alt="Sugar glider peeking from hollow">
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
    <p class="lead" style="margin-top:10px">Add your real donation link here when ready (PayPal, Stripe, or GiveNow).</p>
  </section>

  <!-- Membership -->
  <section id="membership">
    <h2>Membership</h2>
    <p class="lead">Join our compassionate community and help us rescue, rehabilitate, and rehome animals in need.</p>
    <div class="grid cols-3" style="margin-top:16px">
      <div class="card">
        <h3>Individual — $25</h3>
        <p>Supports one rescued animal.</p>
        <p><a class="btn" href="#contact">Become a member</a></p>
      </div>
      <div class="card">
        <h3>Family — $45</h3>
        <p>Supports multiple animals and includes family updates.</p>
        <p><a class="btn" href="#contact">Become a member</a></p>
      </div>
      <div class="card">
        <h3>Sponsor — $80</h3>
        <p>Name recognition and sponsor updates.</p>
        <p><a class="btn" href="#contact">Become a sponsor</a></p>
      </div>
    </div>
    <div class="card" style="margin-top:16px">
      <h3>Details</h3>
      <p>All fees are non‑refundable and go directly to the care of rescued animals.</p>
      <p><b>Address:</b> 2353 Korumburra‑Warragul Rd, Tetoora Road VIC 3821</p>
      <p><b>Email:</b> Bawbawanimalrescue@Gmail.com</p>
      <p><b>Phone:</b> 0400239030</p>
    </div>
  </section>

  <!-- Gallery -->
  <section id="gallery">
    <h2>Wildlife gallery</h2>
    <p class="lead">A glimpse of the lives you help protect — native icons and little wonders.</p>
    <div class="grid cols-3" style="margin-top:16px">
      <div><img src="yRDbRTsPCFEu8qYRDNiCk.jpeg" alt="Kangaroos at sunset"></div>
      <div><img src="SWcJoiX5vvdK7vXp6iBBD.jpeg" alt="Galah on railing"></div>
      <div><img src="FzrSiad5UZzGRL9f4EqG7.jpeg" alt="Kookaburra on branch"></div>
      <div><img src="xgUQvGULSTWSGa5fzjeng.jpeg" alt="Echidna close-up"></div>
      <div><img src="p99hQCADMYmhLPskgJXx4.jpeg" alt="Lizard on rock"></div>
      <div><img src="rGDcraHhNVfkgcw5cQrmJ.webp" alt="Camel in semi-arid landscape"></div>
      <div><img src="DryiTft89B9qS1nTC1qAw.jpeg" alt="Koala climbing a tree"></div>
      <div><img src="qNxSvpPCca9mj2iEWxm9g.jpeg" alt="Kangaroo crossing rural road"></div>
    </div>
  </section>

  <!-- Contact -->
  <section id="contact">
    <h2>Contact us</h2>
    <div class="grid cols-2" style="margin-top:12px">
      <div class="card">
        <h3>Reach us directly</h3>
        <p><b>Email:</b> Bawbawanimalrescue@Gmail.com</p>
        <p><b>Phone:</b> 0400239030</p>
        <p><b>Address:</b> 2353 Korumburra‑Warragul Rd, Tetoora Road VIC 3821</p>
        <img src="97E1EL6N8tTR5ddBFHi9g.jpeg" alt="Baw Baw Animal Rescue logo" style="margin-top:10px; max-width:180px">
      </div>
      <div class="card">
        <h3>Message</h3>
        <p>Want to adopt, donate, volunteer, or become a member? Reach out and we’ll connect you with the right team.</p>
        <p class="lead">For emergencies, contact local wildlife services and your nearest vet.</p>
        <p style="margin-top:12px">
          <a class="btn" href="mailto:Bawbawanimalrescue@Gmail.com">Email us</a>
          <a class="btn" href="#membership" style="margin-left:10px">Join as a member</a>
        </p>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer>
    <p>&copy; 2025 Baw Baw Animal Rescue Inc. — From goldfish to roo, it all starts with you.</p>
  </footer>

  <script>
    // Mobile menu toggle
    function toggleMenu(){
      const menu = document.getElementById('menu');
      if(menu) menu.classList.toggle('open');
    }
    window.toggleMenu = toggleMenu;

    // Smooth scroll for internal links
    document.querySelectorAll('a[href^="#"]').forEach(a=>{
      a.addEventListener('click', e=>{
        const id = a.getAttribute('href').slice(1);
        const el = document.getElementById(id);
        if(el){
          e.preventDefault();
          el.scrollIntoView({behavior:'smooth', block:'start'});
          const menu = document.getElementById('menu');
          if(menu && menu.classList.contains('open')) menu.classList.remove('open');
        }
      });
    });
  </script>
</body>
</html>
 <!-- Gallery -->
  <section id="gallery">
    <h2>Wildlife gallery</h2>
    <p class="lead">A glimpse of the lives you help protect — native icons and little wonders.</p>
    <div class="grid cols-3" style="margin-top:16px">
      <div><img src="yRDbRTsPCFEu8qYRDNiCk.jpeg" alt="Kangaroos at sunset"></div>
      <div><img src="SWcJoiX5vvdK7vXp6iBBD.jpeg" alt="Galah on railing"></div>
      <div><img src="FzrSiad5UZzGRL9f4EqG7.jpeg" alt="Kookaburra on branch"></div>
      <div><img src="xgUQvGULSTWSGa5fzjeng.jpeg" alt="Echidna close-up"></div>
      <div><img src="p99hQCADMYmhLPskgJXx4.jpeg" alt="Lizard on rock"></div>
      <div><img src="rGDcraHhNVfkgcw5cQrmJ.webp" alt="Camel in semi-arid landscape"></div>
      <div><img src="DryiTft89B9qS1nTC1qAw.jpeg" alt="Koala climbing a tree"></div>
      <div><img src="qNxSvpPCca9mj2iEWxm9g.jpeg" alt="Kangaroo crossing rural road"></div>
    </div>
  </section>
