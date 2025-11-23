[index.html.html](https://github.com/user-attachments/files/23699315/index.html.html)
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Baw Baw Animal Rescue Inc.</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <meta name="description" content="From goldfish to roo, it all starts with you. Baw Baw Animal Rescue Inc. — adopt, donate, join as a member, and help save lives.">
  <link href="https://fonts.googleapis.com/css2?family=Merriweather:wght@400;700;900&display=swap" rel="stylesheet">
  <style>
    :root {
      --green: #2b5f4a;
      --orange: #f4a261;
      --white: #ffffff;
      --radius: 16px;
      --shadow: 0 6px 18px rgba(0,0,0,.1);
      --max: 1100px;
    }
    * { box-sizing: border-box }
    html, body { margin: 0; padding: 0 }
    body {
      font-family: 'Merriweather', serif;
      background: var(--orange);
      color: var(--green);
      line-height: 1.7;
    }
    img { max-width: 100%; display: block; border-radius: 12px }

    header {
      position: sticky; top: 0; z-index: 50;
      background: var(--white);
      border-bottom: 1px solid rgba(0,0,0,.1);
    }
    .nav {
      max-width: var(--max); margin: 0 auto; padding: 14px 20px;
      display: flex; align-items: center; justify-content: space-between;
    }
    .brand {
      display: flex; align-items: center; gap: 12px;
      text-decoration: none; color: var(--green); font-weight: 900;
    }
    .brand img { height: 44px }
    nav a {
      margin: 0 8px; text-decoration: none;
      color: var(--green); font-weight: 700;
    }

    section { max-width: var(--max); margin: 0 auto; padding: 60px 20px }
    h1, h2, h3 { color: var(--green); margin-top: 0 }
    .lead { opacity: .95 }

    .hero { text-align: center; padding: 80px 20px }
    .hero img { max-width: 180px; margin-bottom: 20px }
    .motto {
      display: inline-block; font-weight: 900;
      border: 2px solid var(--green); border-radius: 999px;
      padding: 10px 14px;
    }

    .grid { display: grid; gap: 22px }
    @media(min-width:760px){
      .cols-2 { grid-template-columns: 1fr 1fr }
      .cols-3 { grid-template-columns: repeat(3, 1fr) }
    }

    .card {
      background: var(--white);
      border-radius: var(--radius);
      box-shadow: var(--shadow);
      padding: 18px;
    }

    .btn {
      display: inline-block;
      text-decoration: none;
      color: var(--green);
      font-weight: 700;
      border: 2px solid var(--green);
      border-radius: 12px;
      padding: 10px 14px;
    }

    footer {
      background: var(--white);
      border-top: 1px solid rgba(0,0,0,.1);
      text-align: center;
      padding: 40px 20px;
      color: var(--green);
    }
  </style>
</head>
<body>

<header>
  <div class="nav">
    <a class="brand" href="#home">
      <img src="kk9cNDHnLzbKu35pMfcgu.jpeg" alt="Logo">
      <span>Baw Baw Animal Rescue Inc.</span>
    </a>
    <nav>
      <a href="#home">Home</a>
      <a href="#adopt">Adopt</a>
      <a href="#donate">Donate</a>
      <a href="#membership">Membership</a>
      <a href="#contact">Contact</a>
    </nav>
  </div>
</header>

<section id="home" class="hero">
  <img src="36qRwJD4q5cF9nRT1YChg.jpeg" alt="Logo 2">
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
    <div class="card">
      <h3>$25</h3>
      <p>Provides vaccinations and basic supplies for one animal.</p>
    </div>
    <div class="card">
      <h3>$50</h3>
      <p>Covers food and enrichment for a week.</p>
    </div>
    <div class="card">
      <h3>$100</h3>
      <p>Funds vet checks and emergency transport.</p>
    </div>
  </div>
</section>

<section id="membership">
  <h2>Membership</h2>
  <div class="grid cols-3" style="margin-top:16px">
    <div class="card">
      <h3>Individual — $25</h3>
      <p>Supports one rescued animal.</p>
    </div>
    <div class="card">
      <h3>Family — $45</h3>
      <p>Supports multiple animals and includes family updates.</p>
    </div>
    <div class="card">
      <h3>Sponsor — $80</h3>
      <p>Includes name recognition and sponsor updates.</p>
    </div>
  </div>
  <div class="card" style="margin-top:16px">
    <h3>Why Join?</h3>
    <p>Your membership helps us provide food, shelter, medical care, and love to animals who deserve a second chance. Every dollar goes directly to their wellbeing.</p>
    <p><b>Address:</b> 2353 Korumburra-Warragul Rd, Tetoora Road VIC 3821</p>
    <p><b>Email:</b> Bawbawanimalrescue@Gmail.com</p>
    <p><b>Phone:</b> 0400239030</p>
  </div>
</section>

<section id="contact">
  <h2>Contact us</h2>
  <div class="grid cols-2" style="margin-top:12px">
    <div class="card">
      <h3>Reach us directly</h3>
      <p><b>Email:</b> Bawbawanimalrescue@Gmail.com</p>
      <p><b>Phone:</b> 0400239030</p>
      <p><b>Address:</b> 2353 Korumburra-Warragul Rd, Tetoora Road VIC 3821</p>
      <img src="kk9cNDHnLzbKu35pMfcgu.jpeg" alt="Logo" style="margin-top:10px; max-width:180px">
    </div>
    <div class="card">
      <h3>Message</h3>
      <p>Want to adopt, donate, volunteer, or become a member? Reach out and we’ll connect you with the right team.</p>
      <p class="lead">For emergencies, contact local wildlife services and your nearest vet.</p>
      <p style="margin-top:12px">
        <a class="btn" href="mailto:Bawbawanimalrescue@Gmail.com">Email us</a>
      </p>
    </div>
