[index.html.html](https://github.com/user-attachments/files/23694564/index.html.html)
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Baw Baw Animal Rescue Inc.</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <style>
    /* Colors inspired by your logo */
    :root {
      --primary: #2563eb;   /* deep blue */
      --secondary: #10b981; /* green */
      --accent: #f59e0b;    /* goldfish orange */
      --neutral: #f9fafb;   /* light background */
    }

    body {
      font-family: Arial, sans-serif;
      margin: 0;
      background: var(--neutral);
      color: #111;
    }

    header {
      background: var(--primary);
      color: white;
      padding: 20px;
      text-align: center;
    }

    header h1 {
      margin: 0;
    }

    nav {
      margin-top: 10px;
    }

    nav a {
      color: white;
      margin: 0 12px;
      text-decoration: none;
      font-weight: bold;
    }

    nav a:hover {
      text-decoration: underline;
    }

    section {
      max-width: 900px;
      margin: 40px auto;
      padding: 20px;
      background: white;
      border-radius: 8px;
      box-shadow: 0 2px 6px rgba(0,0,0,0.1);
    }

    section h2 {
      color: var(--primary);
    }

    .button {
      display: inline-block;
      background: var(--secondary);
      color: white;
      padding: 10px 14px;
      border-radius: 6px;
      text-decoration: none;
      margin-top: 10px;
    }

    .button:hover {
      background: #059669;
    }

    footer {
      text-align: center;
      color: #666;
      padding: 20px;
      background: #eee;
      margin-top: 40px;
    }

    .motto {
      font-style: italic;
      color: var(--accent);
      margin-top: 10px;
    }

    img {
      max-width: 100%;
      border-radius: 8px;
    }
  </style>
</head>
<body>
  <header>
    <h1>Baw Baw Animal Rescue Inc.</h1>
    <p class="motto">From goldfish to roo, it all starts with you</p>
    <nav>
      <a href="#home">Home</a>
      <a href="#adopt">Adopt</a>
      <a href="#donate">Donate</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <!-- Home Section -->
  <section id="home">
    <h2>Welcome</h2>
    <p>We are a volunteer‑run non‑profit rescuing and rehoming animals in the Baw Baw region. Every life matters — from the smallest goldfish to the tallest roo.</p>
    <img src="images/home.jpg" alt="Rescue animals">
  </section>

  <!-- Adopt Section -->
  <section id="adopt">
    <h2>Adopt a Friend</h2>
    <p>Looking for a forever friend? Meet some of our wonderful animals ready for adoption.</p>
    <div>
      <img src="images/dog.jpg" alt="Rescue dog">
      <h3>Buddy</h3>
      <p>Playful 3‑year‑old dog who loves walks and cuddles.</p>
    </div>
    <div>
      <img src="images/cat.jpg" alt="Rescue cat">
      <h3>Mittens</h3>
      <p>Gentle 2‑year‑old cat looking for a loving home.</p>
    </div>
  </section>

  <!-- Donate Section -->
  <section id="donate">
    <h2>Support Our Mission</h2>
    <p>Your donations help pay for food, vet bills, and transport. Every dollar makes a difference.</p>
    <a class="button" href="https://www.paypal.me/YourRescue">Donate via PayPal</a>
  </section>

  <!-- Contact Section -->
  <section id="contact">
    <h2>Contact Us</h2>
    <p>Email: info@bawbawanimalrescue.org</p>
    <p>Facebook: @BawBawAnimalRescue</p>
    <p>Instagram: @BawBawRescue</p>
  </section>

  <footer>
    &copy; 2025 Baw Baw Animal Rescue Inc.
  </footer>
</body>
</html>
