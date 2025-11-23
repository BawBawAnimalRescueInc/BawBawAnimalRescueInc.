[index.html](https://github.com/user-attachments/files/23699069/index.html)
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Baw Baw Animal Rescue Inc.</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <meta name="description" content="From goldfish to roo, it all starts with you. Baw Baw Animal Rescue Inc. — adopt, donate, and help save lives.">
  <style>
    /* =========================================
       Brand and theme
       Adjust these to match your logo vibes
       ========================================= */
    :root{
      --blue:#1f3d7a;      /* Deep rescue blue */
      --green:#20b27b;     /* Hopeful green */
      --gold:#f5a623;      /* Goldfish gold accent */
      --charcoal:#121417;  /* Dark text */
      --cloud:#f5f7fb;     /* Light background */
      --white:#ffffff;

      --maxw:1100px;
      --radius:18px;
      --shadow:0 12px 28px rgba(18,20,23,.18);
      --shadow-soft:0 6px 18px rgba(18,20,23,.12);
    }

    /* Reset + base */
    *{box-sizing:border-box}
    html,body{margin:0;padding:0}
    body{
      font-family: ui-sans-serif, system-ui, -apple-system, Segoe UI, Roboto, "Helvetica Neue", Arial, "Noto Sans", "Liberation Sans";
      color:var(--charcoal);
      background:
        radial-gradient(1200px 500px at 100% -100%, rgba(32,178,123,.08), transparent 60%),
        radial-gradient(800px 400px at -40% 10%, rgba(245,166,35,.12), transparent 55%),
        var(--cloud);
      line-height:1.5;
    }
    img{max-width:100%;display:block;border-radius:12px}

    /* Decorative paw pattern in header */
    .paw-bg{
      background-image:
        radial-gradient(circle at 8px 8px, rgba(255,255,255,.25) 3px, transparent 4px),
        radial-gradient(circle at 28px 12px, rgba(255,255,255,.25) 3px, transparent 4px),
        radial-gradient(circle at 16px 24px, rgba(255,255,255,.25) 4px, transparent 5px);
      background-size: 36px 36px;
    }

    /* Header / nav */
    header{
      position:sticky; top:0; z-index:50;
      backdrop-filter: saturate(1.2) blur(8px);
    }
    .nav{
      display:flex; align-items:center; justify-content:space-between;
      max-width:var(--maxw); margin:0 auto; padding:14px 20px;
    }
    .brand{
      display:flex; align-items:center; gap:12px; text-decoration:none; color:var(--charcoal);
      font-weight:700; letter-spacing:.2px;
    }
    .logo{
      width:42px; height:42px; border-radius:50%;
      background: conic-gradient(from 210deg, var(--blue), var(--blue) 35%, var(--green) 35%, var(--green) 68%, var(--gold) 68%, var(--gold) 100%);
      box-shadow: var(--shadow-soft);
      position:relative;
    }
    .logo:after{
      content:""; position:absolute; inset:7px; border-radius:50%;
      background: radial-gradient(circle at 55% 40%, #fff 12%, transparent 13%),
                  radial-gradient(circle at 35% 40%, #fff 12%, transparent 13%),
                  radial-gradient(circle at 45% 60%, #fff 16%, transparent 17%);
      opacity:.7;
    }

    .menu a{
      text-decoration:none; color:var(--charcoal); font-weight:600; padding:10px 12px; border-radius:10px;
    }
    .menu a:hover{ background:rgba(32,178,123,.12) }
    .cta{
      background:var(--green); color:var(--white); padding:10px 14px; border-radius:12px; text-decoration:none; font-weight:700;
      box-shadow: var(--shadow-soft);
    }
    .cta:hover{ filter:brightness(1.08) }

    /* Hero */
    .hero{
      position:relative; overflow:hidden;
      background: linear-gradient(135deg, var(--blue), #274a97 60%), url('') center/cover no-repeat;
      color:var(--white);
    }
    .hero-wrap{
      max-width:var(--maxw); margin:0 auto; padding:72px 20px;
      display:grid; grid-template-columns: 1.1fr .9fr; gap:32px;
    }
    .motto{
      display:inline-block; background:rgba(245,166,35,.18); color:#fff; padding:8px 12px; border-radius:12px; font-weight:700;
      border:1px solid rgba(245,166,35,.4);
    }
    .hero h1{font-size:clamp(28px, 6vw, 52px); margin:.6em 0 .4em; line-height:1.05}
    .hero p{font-size:clamp(14px, 2.2vw, 18px); opacity:.92}

    .hero-card{
      background:var(--white); color:var(--charcoal); border-radius:var(--radius); box-shadow:var(--shadow);
      padding:20px;
      transform: rotate(-1deg);
    }
    .hero-card h3{margin-top:0}
    .stat{
      display:flex; align-items:center; gap:12px; padding:10px 12px; border-radius:12px; background:#f8fbf9; border:1px solid #e6f3ee;
    }
    .stat b{color:var(--green)}

    /* Sections */
    section{ max-width:var(--maxw); margin:0 auto; padding:60px 20px }
    .section-title{ font-size:26px; margin:0 0 18px; color:var(--blue) }
    .grid{ display:grid; gap:22px }
    @media(min-width:760px){
      .grid.cols-2{ grid-template-columns: 1fr 1fr }
      .grid.cols-3{ grid-template-columns: repeat(3, 1fr) }
    }

    .card{
      background:var(--white); border-radius:var(--radius); box-shadow:var(--shadow-soft);
      border:1px solid #eaeef7; padding:18px;
    }
    .badge{
      display:inline-block; background:rgba(245,166,35,.14); color:#8a5a00; border:1px solid rgba(245,166,35,.35);
      padding:6px 10px; border-radius:999px; font-weight:700; font-size:14px;
    }
    .btn{
      display:inline-block; text-decoration:none; font-weight:700; border-radius:12px; padding:10px 14px;
      border:2px solid var(--green); color:var(--green);
    }
    .btn.fill{ background:var(--green); color:#fff }
    .btn:hover{ filter:brightness(1.06) }

    /* Adopt gallery cards */
    .pet{ display:grid; grid-template-columns: 120px 1fr; gap:14px; align-items:center }
    .pet .thumb{
      width:120px; height:120px; border-radius:12px; background:
        radial-gradient(circle at 30% 30%, #ffd89b, #f5a623 65%),
        linear-gradient(135deg, #ffe9c7, #f7cd86);
      position:relative;
    }
    .thumb:after{
      content:""; position:absolute; inset:0; border-radius:12px; background:
        radial-gradient(circle at 70% 30%, rgba(32,178,123,.5) 10%, transparent 12%),
        radial-gradient(circle at 30% 70%, rgba(31,61,122,.45) 10%, transparent 12%);
      mix-blend-mode:multiply; opacity:.5;
    }

    /* Donate block */
    .donate{
      background:linear-gradient(135deg, rgba(32,178,123,.12), rgba(31,61,122,.12));
      border:1px solid #d8e8e2; padding:22px; border-radius:var(--radius);
    }
    .donate .options{ display:flex; gap:12px; flex-wrap:wrap }
    .tier{ flex:1 1 160px; background:#fff; border:1px solid #eaeef7; border-radius:14px; padding:14px; text-align:center }

    /* Contact */
    .contact{
      background:#fff; border-radius:var(--radius); border:1px solid #eaeef7; padding:22px;
    }
    .contact .row{ display:grid; gap:12px }
    @media(min-width:760px){ .contact .row{ grid-template-columns: 1fr 1fr } }
    input,textarea{
      width:100%; padding:12px 14px; border-radius:12px; border:1px solid #d9dfeb; font:inherit; background:#fbfcff;
    }
    textarea{ min-height:120px }
    .note{ font-size:13px; color:#58627a }

    /* Footer */
    footer{
      padding:40px 20px; text-align:center; color:#6b7280;
    }
    .foot-brand{ font-weight:800; color:var(--blue) }

    /* Back to top */
    .top{
      position:fixed; right:18px; bottom:18px; z-index:40;
      background:var(--blue); color:#fff; border:none; border-radius:999px; padding:12px 14px; box-shadow:var(--shadow-soft);
      cursor:pointer; display:none;
    }

    /* Mobile nav */
    .hamburger{ display:none; border:none; background:transparent; font-weight:800; font-size:16px }
    @media(max-width:860px){
      .hero-wrap{ grid-template-columns: 1fr }
      .menu{ display:none }
      .hamburger{ display:block }
      .menu.open{ display:flex; gap:8px; flex-wrap:wrap; margin-top:8px }
      .menu.open a{ background:#fff }
    }

    /* Subtle animation */
    .float { animation: float 6s ease-in-out infinite }
    @keyframes float {
      0%{ transform:translateY(0) }
      50%{ transform:translateY(-6px) }
      100%{ transform:translateY(0) }
    }
  </style>
</head>
<body>

  <!-- Sticky navigation -->
  <header class="paw-bg">
    <div class="nav">
      <a class="brand" href="#home" aria-label="Baw Baw Animal Rescue home">
        <span class="logo float"></span>
        <span>Baw Baw Animal Rescue Inc.</span>
      </a>
      <button class="hamburger" aria-label="Open menu" onclick="toggleMenu()">Menu</button>
      <nav id="menu" class="menu">
        <a href="#home">Home</a>
        <a href="#adopt">Adopt</a>
        <a href="#donate">Donate</a>
        <a href="#about">About</a>
        <a href="#contact" class="cta">Contact</a>
      </nav>
    </div>
  </header>

  <!-- Hero -->
  <section id="home" class="hero">
    <div class="hero-wrap">
      <div>
        <span class="motto">From goldfish to roo, it all starts with you</span>
        <h1>Rescue. Rehabilitate. Rehome.</h1>
        <p>We’re a volunteer‑run nonprofit helping animals across the Baw Baw region. No creature is too small or too tall — every life deserves care.</p>
        <div style="display:flex; gap:10px; margin-top:14px">
          <a class="btn fill" href="#adopt">Find a friend</a>
          <a class="btn" href="#donate">Support our work</a>
        </div>
        <div style="display:flex; gap:10px; margin-top:18px">
          <span class="stat"><b>1,200+</b> animals assisted</span>
          <span class="stat"><b>95%</b> adoption success</span>
        </div>
      </div>
      <div class="hero-card">
        <h3>Today’s spotlight</h3>
        <p class="badge">Ready for adoption</p>
        <div class="grid cols-2" style="margin-top:12px">
          <div>
            <div class="thumb" aria-hidden="true"></div>
            <p><b>River</b> — calm senior cat who loves sunny windowsills.</p>
          </div>
          <div>
            <div class="thumb" aria-hidden="true"></div>
            <p><b>Koda</b> — joyful dog who thrives on bush walks and belly rubs.</p>
          </div>
        </div>
        <a class="btn fill" href="#adopt" style="margin-top:10px">See more pets</a>
      </div>
    </div>
  </section>

  <!-- Adopt gallery -->
  <section id="adopt">
    <h2 class="section-title">Adopt a friend</h2>
    <p>When you adopt, you change a life — yours and theirs. Meet some of our beautiful companions waiting for their forever homes.</p>
    <div class="grid cols-3" style="margin-top:18px">
      <div class="card pet">
        <div class="thumb" aria-hidden="true"></div>
        <div>
          <h3>Willow</h3>
          <p>Gentle 2‑year‑old with a soft spot for string toys and quiet naps.</p>
          <a class="btn" href="#contact">Enquire</a>
        </div>
      </div>
      <div class="card pet">
        <div class="thumb" aria-hidden="true"></div>
        <div>
          <h3>Diesel</h3>
          <p>Playful 3‑year‑old adventurer; happiest on trails and beaches.</p>
          <a class="btn" href="#contact">Enquire</a>
        </div>
      </div>
      <div class="card pet">
        <div class="thumb" aria-hidden="true"></div>
        <div>
          <h3>Sunny</h3>
          <p>Curious goldfish with a shimmering tail — small life, big joy.</p>
          <a class="btn" href="#contact">Enquire</a>
        </div>
      </div>
    </div>
    <div class="card" style="margin-top:18px">
      <p class="note">All adoptions include vet checks, microchipping, and a care guide. We’ll match you with the right companion.</p>
    </div>
  </section>

  <!-- Donate -->
  <section id="donate">
    <h2 class="section-title">Donate to save lives</h2>
    <p>Your generosity funds vet care, food, emergency transport, and rehabilitation. Every dollar keeps us moving.</p>
    <div class="donate">
      <div class="options">
        <div class="tier">
          <h3>$25</h3>
          <p>Vaccinations and basic supplies.</p>
          <a class="btn fill" href="https://www.paypal.me/YourRescue" target="_blank" rel="noopener">Give $25</a>
        </div>
        <div class="tier">
          <h3>$50</h3>
          <p>Food for a week and enrichment toys.</p>
          <a class="btn fill" href="https://www.paypal.me/YourRescue" target="_blank" rel="noopener">Give $50</a>
        </div>
        <div class="tier">
          <h3>$100</h3>
          <p>Vet check + transportation for intake.</p>
          <a class="btn fill" href="https://www.paypal.me/YourRescue" target="_blank" rel="noopener">Give $100</a>
        </div>
      </div>
      <p class="note" style="margin-top:12px">Prefer bank transfer or monthly giving? Contact us and we’ll set you up.</p>
    </div>
  </section>

  <!-- About -->
  <section id="about">
    <h2 class="section-title">About our mission</h2>
    <div class="grid cols-2">
      <div class="card">
        <p class="badge">Community led</p>
        <h3>From goldfish to roo</h3>
        <p>We respond to calls across Baw Baw and surrounds, partner with local vets, and support foster carers. Whether it’s a tiny tank or open pasture, we believe in compassionate, practical care.</p>
      </div>
      <div class="card">
        <p class="badge">Transparency</p>
        <h3>How we operate</h3>
        <p>We’re volunteer‑run and donation‑funded. Our books are open, our processes are clear, and our network is growing thanks to people like you.</p>
      </div>
    </div>
  </section>

  <!-- Contact -->
  <section id="contact">
    <h2 class="section-title">Contact us</h2>
    <div class="contact">
      <div class="row">
        <div>
          <label for="name">Name</label>
          <input id="name" type="text" placeholder="Your name">
        </div>
        <div>
          <label for="email">Email</label>
          <input id="email" type="email" placeholder="you@example.org">
        </div>
      </div>
      <div style="margin-top:12px">
        <label for="message">Message</label>
        <textarea id="message" placeholder="Tell us who you’d like to adopt or how you’d like to help"></textarea>
      </div>
      <div style="margin-top:12px">
        <button class="btn fill" onclick="alert('Thanks for reaching out! Please email info@bawbawanimalrescue.org so we can reply.');">Send message</button>
        <p class="note" style="margin-top:8px">This demo form doesn’t send emails. To make it work, use Formspree or a similar service and replace the button with a real form action.</p>
      </div>
      <div style="margin-top:16px; display:grid; gap:12px">
        <div class="stat"><b>Email:</b> info@bawbawanimalrescue.org</div>
        <div class="stat"><b>Facebook:</b> @BawBawAnimalRescue</div>
        <div class="stat"><b>Instagram:</b> @BawBawRescue</div>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer>
    <div class="foot-brand">Baw Baw Animal Rescue Inc.</div>
    <div>&copy; 2025. All rights reserved. ABN / Inc. details here.</div>
  </footer>

  <button class="top" id="topBtn" onclick="window.scrollTo({top:0,behavior:'smooth'})">Top</button>

  <script>
    // Smooth section navigation
    document.querySelectorAll('a[href^="#"]').forEach(a=>{
      a.addEventListener('click', e=>{
        const id = a.getAttribute('href').slice(1);
        const el = document.getElementById(id);
        if(el){
          e.preventDefault();
          el.scrollIntoView({behavior:'smooth', block:'start'});
          if(window.innerWidth<860){
            document.getElementById('menu').classList.remove('open');
          }
        }
      });
    });

    // Back-to-top visibility
    const topBtn = document.getElementById('topBtn');
    window.addEventListener('scroll', ()=>{
      topBtn.style.display = window.scrollY>600 ? 'block' : 'none';
    });

    // Mobile menu toggle
    function toggleMenu(){
      document.getElementById('menu').classList.toggle('open');
    }
    window.toggleMenu = toggleMenu;
  </script>
</body>
</html>
