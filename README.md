[index.html.html](https://github.com/user-attachments/files/23699322/index.html.html)
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Baw Baw Animal Rescue Inc.</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link href="https://fonts.googleapis.com/css2?family=Merriweather:wght@400;700;900&display=swap" rel="stylesheet">
  <style>
    :root {
      --bg: #f4e7d4;
      --text: #2b5f4a;
      --accent: #e07a5f;
      --white: #ffffff;
      --radius: 16px;
      --shadow: 0 6px 18px rgba(0,0,0,.1);
      --max: 1100px;
    }
    * { box-sizing: border-box; margin: 0; padding: 0 }
    body {
      font-family: 'Merriweather', serif;
      background: var(--bg);
      color: var(--text);
      line-height: 1.7;
    }
    img { max-width: 100%; display: block; border-radius: 12px }

    header {
      background: var(--white);
      border-bottom: 1px solid rgba(0,0,0,.1);
      position: sticky;
      top: 0;
      z-index: 10;
    }
    .nav {
      max-width: var(--max);
      margin: auto;
      padding: 16px;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }
    .nav a {
      text-decoration: none;
      color: var(--text);
      margin: 0 10px;
      font-weight: bold;
    }
    .hero {
      text-align: center;
      padding: 80px 20px;
    }
    .hero h1 {
      font-size: 2.5em;
      margin-bottom: 20px;
      color: var(--text);
    }
    section {
      max-width: var(--max);
      margin: auto;
      padding: 60px 20px;
    }
    h2 {
      margin-bottom: 20px;
      color: var(--text);
    }
    .grid {
      display: grid;
      gap: 20px;
    }
    @media(min-width: 700px) {
      .grid.cols-2 { grid-template-columns: 1fr 1fr; }
      .grid.cols-3 { grid-template-columns: repeat(3, 1fr); }
    }
    .card {
      background: var(--white);
      border: 1px solid #ddd;
      border-radius: var(--radius);
      padding: 20px;
      box-shadow: var(--shadow);
    }
    .btn {
      display: inline-block;
      text-decoration: none;
      color: var(--white);
      background: var(--accent);
      font-weight: bold;
      border-radius: 12px;
      padding: 10px 16px;
      margin-top: 10px;
    }
    footer {
      text-align: center;
      padding: 40px 20px;
      background: var(--white);
      color: var(--text);
    }
  </style>
</head>
<body>

<header>
  <div class="nav">
    <div><strong>Baw Baw Animal Rescue Inc.</strong></div>
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
  <img src="kk9cNDHnLzbKu35pMfcgu.jpeg" alt="Logo">
  <h1>From goldfish to roo, it all starts with you</h1>
  <p>We’re a volunteer‑run nonprofit caring for animals across the Baw Baw region. Compassion guides everything we do.</p>
</section>

<section id="adopt">
  <h2>Adopt</h2>
  <div class="grid cols-3">
    <div class="card">
      <img src="UMcsUcg72hYVcpZonV32m.jpeg" alt="Kangaroos">
      <h3>Koda</h3>
      <p>Playful kangaroo who loves bush walks.</p>
      <a class="btn" href="#contact">Enquire</a>
    </div>
    <div class="card">
      <img src="3f8wjdG3wsZQ29612HdAA.jpeg" alt="Koalas">
      <h3>Rosie & Joey</h3>
      <p>Gentle duo seeking a safe habitat and attentive care.</p>
      <a class="btn" href="#contact">Enquire</a>
    </div>
    <div class="card">
      <img src="i6dun9qHeT6eSDCt8fAgZ.jpeg" alt="Sugar glider">
      <h3>Whiskers</h3>
      <p>Curious and social — perfect for experienced carers.</p>
      <a class="btn" href="#contact">Enquire</a>
    </div>
  </div>
</section>

<section id="donate">
  <h2>Donate</h2>
  <div class="grid cols-3">
    <div class="card">
      <h3>$25</h3>
      <p>Provides vaccinations and basic supplies for one animal.</p>
      <a class="btn" href="#contact">Donate</a>
    </div>
    <div class="card">
      <h3>$50</h3>
      <p>Covers food and enrichment for a week.</p>
      <a class="btn" href="#contact">Donate</a>
    </div>
    <div class="card">
      <h3>$100</h3>
      <p>Funds vet checks and emergency transport.</p>
      <a class="btn" href="#contact">Donate</a>
    </div>
  </div>
</section>

<section id="membership">
  <h2>Membership</h2>
  <div class="grid cols-3">
    <div class="card">
      <h3>Individual — $25</h3>
      <p>Supports one rescued animal.</p>
      <a class="btn" href="#contact">Join</a>
    </div>
    <div class="card">
      <h3>Family — $45</h3>
      <p>Supports multiple animals and includes family updates.</p>
      <a class="btn" href="#contact">Join</a>
    </div>
    <div class="card">
      <h3>Sponsor — $80</h3>
      <p>Includes name recognition and sponsor updates.</p>
      <a class="btn" href="#contact">Join</a>
    </div>
  </div>
</section>

<section id="contact">
  <h2>Contact</h2>
  <div class="grid cols-2">
    <div class="card">
      <h3>Reach us</h3>
      <p><b>Email:</b> Bawbawanimalrescue@Gmail.com</p>
      <p><b>Phone:</b> 0400239030</p>
      <p><b>Address:</b> 2353 Korumburra-Warragul Rd, Tetoora Road VIC 3821</p>
    </div>
    <div class="card">
      <h3>Message</h3>
      <p>Want to adopt, donate, volunteer, or become a member? Reach out and we’ll connect you with the right team.</p>
      <a class="btn" href="mailto:Bawbawanimalrescue@Gmail.com">Email Us</a>
    </div>
  </div>
</section>

<footer>
  &copy; 2025 Baw Baw Animal Rescue Inc.
</footer>

</body>
</html>
