:root{
  --bg:#f7f1e6;           /* light beige */
  --ink:#8a5a2b;          /* warm orange-brown for headings */
  --text:#3a4a3f;         /* deep earthy text */
  --accent:#2f7d5f;       /* green buttons */
  --overlay:#f1e2cc;      /* semi-transparent beige blocks */
  --card:#ffffff;
  --muted:#e9dcc6;
  --radius:14px;
  --shadow:0 8px 24px rgba(0,0,0,.12);
  --max:1100px;
}

*{box-sizing:border-box}
html,body{margin:0;padding:0}
body{
  font-family:"Merriweather",serif;
  background:var(--bg);
  color:var(--text);
  line-height:1.7;
}

a{color:var(--text);text-decoration:none}
img{max-width:100%;display:block;border-radius:12px}

header{
  background:#fff;border-bottom:1px solid rgba(0,0,0,.1);
  position:sticky;top:0;z-index:50;
}
.nav{
  max-width:var(--max);margin:0 auto;padding:12px 18px;
  display:flex;align-items:center;justify-content:space-between;gap:12px;
}
.brand{display:flex;align-items:center;gap:10px;font-weight:900;color:var(--text)}
.brand img{height:42px}
.menu{display:flex;flex-wrap:wrap;gap:10px}
.menu a{padding:8px 10px;border-radius:10px;font-weight:700}
.menu a.active{background:var(--muted)}

main{max-width:var(--max);margin:0 auto;padding:28px 18px}
h1,h2,h3{color:var(--ink);margin:0 0 14px}

.hero{
  position:relative;border-radius:16px;overflow:hidden;
  box-shadow:var(--shadow);
}
.hero img{width:100%;height:auto;display:block}
.hero .center{
  position:absolute;inset:0;display:flex;align-items:center;justify-content:center;
  text-align:center;padding:28px;
}
.hero .block{
  background:rgba(241,226,204,.92); /* semi-transparent beige */
  border-radius:16px;padding:22px;max-width:820px;
}
.hero .block h1{margin-bottom:12px}
.hero .block p{margin:0 0 16px}
.btn{
  display:inline-block;background:var(--accent);color:#fff;
  padding:10px 16px;border-radius:12px;font-weight:800
}

.card{
  background:var(--card);border-radius:16px;box-shadow:var(--shadow);padding:18px;
}
.grid{display:grid;gap:18px}
.cols-2{grid-template-columns:1.1fr .9fr}
.cols-3{grid-template-columns:repeat(3,1fr)}
@media(max-width:900px){.cols-2,.cols-3{grid-template-columns:1fr}}

.overlay-section{
  position:relative;border-radius:16px;overflow:hidden;box-shadow:var(--shadow);
}
.overlay-section .text{
  position:absolute;left:20px;top:20px;right:20px;
  background:rgba(241,226,204,.95);padding:18px;border-radius:12px;
}

.meta{color:#5b4a33;font-size:.9rem}
.pills{display:flex;gap:8px;flex-wrap:wrap}
.pill{background:var(--muted);border-radius:999px;padding:6px 10px;font-weight:700}
.field{margin:10px 0}
.field label{display:block;font-weight:700;margin-bottom:6px}
.field input,.field textarea,.field select{
  width:100%;padding:10px 12px;border-radius:10px;border:1px solid #d7c7ad;background:#fff;font-family:"Merriweather",serif
}

.section-title{font-size:1.6rem;margin-bottom:10px;color:var(--ink)}
.footer-sub{
  background:#fff;border-top:1px solid rgba(0,0,0,.1);
  margin-top:30px;padding:22px 18px;color:#5b4a33;text-align:center
}
.subblock{
  background:#fff;border-radius:16px;box-shadow:var(--shadow);padding:18px
}
.tag{background:var(--muted);border-radius:999px;padding:6px 10px;font-weight:700}
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Baw Baw Animal Rescue Inc. — Home</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link href="https://fonts.googleapis.com/css2?family=Merriweather:wght@400;700;900&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="style.css">
</head>
<body>
<header>
  <div class="nav">
    <a class="brand" href="index.html">
      <img src="images/logo.png" alt="Baw Baw Animal Rescue Inc.">
      <span>BAW BAW ANIMAL RESCUE INC.</span>
    </a>
    <nav class="menu">
      <a class="active" href="index.html">Home</a>
      <a href="about.html">About</a>
      <a href="blog.html">Blog</a>
      <a href="contact.html">Contact</a>
      <a href="donate.html">Donate</a>
      <a href="subscriptions.html">My Subscriptions</a>
      <a href="notifications.html">Notifications</a>
      <a href="groups.html">Groups</a>
      <a href="members.html">Members</a>
      <a href="events.html">Events</a>
      <a href="book.html">Book Online</a>
    </nav>
  </div>
</header>

<main>
  <!-- Kangaroo hero exactly like your screenshot -->
  <section class="hero">
    <img src="images/home-hero-kangaroo.jpg" alt="Kangaroo on a sunlit rural road">
    <div class="center">
      <div class="block">
        <h1>Welcome to Baw Baw Animal Rescue Inc.</h1>
        <p>Our mission is to rescue, care for, and rehome animals in need, while promoting responsible pet ownership and reducing animal suffering. As a non‑profit, every resource we receive goes directly toward saving lives and giving animals a second chance.</p>
        <a class="btn" href="about.html">Learn More</a>
      </div>
    </div>
  </section>

  <!-- Mission overlay (tree background + semi-transparent beige) -->
  <section class="overlay-section" style="margin-top:22px">
    <img src="images/home-mission-tree.jpg" alt="Sunlit tree background">
    <div class="text">
      <h2>Our Animal Rescue Mission</h2>
      <p>Baw Baw Animal Rescue Inc. is a community-driven organisation committed to giving vulnerable animals the chance at a better life. Our work begins with rescue—finding animals out of unsafe, neglected, or abandoned situations—and continues with dedicated care, rehabilitation, and ultimately rehoming them with families who will provide the love and security they deserve.</p>
      <p>We believe that every animal has the right to live free from suffering and we strive to make that vision a reality through hands-on support and education. Beyond rescue, we actively promote responsible pet ownership, helping people understand the commitments of pet ownership, pet protection, veterinary care, and the lifelong commitment that comes with welcoming a pet into their home.</p>
      <p>Every donation, volunteer hour, and rescued life we achieve is used directly to save lives through emergency medical treatment, providing food and shelter, or supporting adoption programs. Our focus is always on giving animals a second chance. We are proud to be part of a compassionate network of people who believe in reducing animal suffering and building a kinder future—one rescue at a time.</p>
    </div>
  </section>

  <!-- New To The Family... -->
  <section style="margin-top:22px">
    <h2 class="section-title">New To The Family...</h2>
    <div class="grid cols-3">
      <article class="card">
        <img src="images/blog-1-shoes.jpg" alt="City street shoes with lights">
        <div class="meta">autarchlabs • Mar 22 • 2 min read</div>
        <h3>Eco-Friendly Home Decor: Nature-Inspired Design Ideas</h3>
        <p class="meta">253 views • 0 comments • 0 likes</p>
      </article>
      <article class="card">
        <img src="images/blog-2-beach.jpg" alt="Scenic beach sunset">
        <div class="meta">autarchlabs • Mar 22 • 2 min read</div>
        <h3>Protecting Our Planet: Simple Steps to Environmental Conservation</h3>
        <p class="meta">122 views • 0 comments • 0 likes</p>
      </article>
      <article class="card">
        <img src="images/blog-3-portrait.jpg" alt="Woman outdoors portrait">
        <div class="meta">autarchlabs • Mar 22 • 2 min read</div>
        <h3>Sustainable Living Tips: Reduce Waste and Conserve Energy</h3>
        <p class="meta">50 views • 0 comments • 0 likes</p>
      </article>
    </div>
    <p style="text-align:center;margin-top:10px"><a class="btn" href="blog.html">Discover More</a></p>
  </section>

  <!-- Latest Rescue Updates (sugar glider + right text) -->
  <section style="margin-top:22px" class="grid cols-2">
    <div class="card">
      <img src="images/sugar-glider.jpg" alt="Sugar glider peeking from tree hollow">
    </div>
    <div class="card">
      <h3>Animal Welfare</h3>
      <p><strong>Urgency of Animal Rescue</strong></p>
      <p>Learn about the latest developments in animal welfare and the urgent need for action to rescue and protect animals in distress.</p>
    </div>
  </section>

  <!-- Responsible pet ownership (lizard, left text) -->
  <section style="margin-top:22px" class="grid cols-2">
    <div class="card">
      <h3>Promoting Responsible Pet Ownership</h3>
      <p><strong>Caring for Animals in Need</strong></p>
      <p>Discover the importance of responsible pet ownership and the critical role we play in caring for animals in need of a loving home.</p>
    </div>
    <div class="card">
      <img src="images/lizard.jpg" alt="Lizard on a rock">
    </div>
  </section>

  <!-- Fostering and Adoption (parrot + right text) -->
  <section style="margin-top:22px" class="grid cols-2">
    <div class="card">
      <img src="images/parrot.jpg" alt="Pink and grey parrot on railing">
    </div>
    <div class="card">
      <h3>Fostering and Adoption</h3>
      <p><strong>Providing Second Chances</strong></p>
      <p>Explore our fostering and adoption programs, providing second chances for animals in need of a forever home.</p>
    </div>
  </section>

  <!-- FAQs -->
  <section style="margin-top:22px" class="card">
    <h2 class="section-title">FAQs</h2>
    <h3>Why is Animal Rescue Important?</h3>
    <p>Animal rescue is crucial for providing a safe and nurturing environment for animals in need. It involves rescuing, rehabilitating, and rehoming animals to give them a chance at a better life.</p>
    <h3>How Can I Help Rescue Animals?</h3>
    <p>Supporting animal rescue organizations, volunteering at shelters, and considering pet adoption are effective ways to make a positive impact on animal rescue efforts.</p>
    <h3>What Are the Benefits of Animal Adoption?</h3>
    <p>Animal adoption provides a loving home for pets in need, reduces overpopulation in shelters, and brings joy and companionship to both the animal and the adopter.</p>
    <h3>How Can I Support Animal Welfare?</h3>
    <p>Individuals actions like fostering animals, promoting adoption events, and advocating for animal welfare laws can significantly impact the well-being of animals in our community.</p>
  </section>

  <!-- Echidna image -->
  <section style="margin-top:22px" class="card">
    <img src="images/echidna.jpg" alt="Echidna foraging on grass and dirt">
  </section>
</main>

<footer class="footer-sub">
  © 2025 Baw Baw Animal Rescue Inc.
</footer>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Baw Baw Animal Rescue Inc. — About</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link href="https://fonts.googleapis.com/css2?family=Merriweather:wght@400;700;900&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="style.css">
</head>
<body>
<header>
  <div class="nav">
    <a class="brand" href="index.html"><img src="images/logo.png" alt=""><span>BAW BAW ANIMAL RESCUE INC.</span></a>
    <nav class="menu">
      <a href="index.html">Home</a><a class="active" href="about.html">About</a><a href="blog.html">Blog</a><a href="contact.html">Contact</a><a href="donate.html">Donate</a><a href="subscriptions.html">My Subscriptions</a><a href="notifications.html">Notifications</a><a href="groups.html">Groups</a><a href="members.html">Members</a><a href="events.html">Events</a><a href="book.html">Book Online</a>
    </nav>
  </div>
</header>
<main>
  <h1 style="color:#e4792f">Our Mission</h1>
  <div class="grid cols-2">
    <div class="card"><img src="images/about-koalas.jpg" alt="Two koalas on a tree"></div>
    <div class="card">
      <p style="color:#e4792f"><strong>At Baw Baw Animal Rescue</strong> our mission is to rescue, care for, and rehome animals in need, while promoting responsible pet ownership and reducing animal suffering. As a non‑profit, every resource we receive goes directly toward saving lives and giving animals a second chance.</p>
      <p><a class="btn" href="index.html">Learn More</a></p>
    </div>
  </div>
</main>
<footer class="footer-sub">© 2025 Baw Baw Animal Rescue Inc.</footer>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Baw Baw Animal Rescue Inc. — Blog</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link href="https://fonts.googleapis.com/css2?family=Merriweather:wght@400;700;900&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="style.css">
</head>
<body>
<header>
  <div class="nav">
    <a class="brand" href="index.html"><img src="images/logo.png" alt=""><span>BAW BAW ANIMAL RESCUE INC.</span></a>
    <nav class="menu">
      <a href="index.html">Home</a><a href="about.html">About</a><a class="active" href="blog.html">Blog</a><a href="contact.html">Contact</a><a href="donate.html">Donate</a><a href="subscriptions.html">My Subscriptions</a><a href="notifications.html">Notifications</a><a href="groups.html">Groups</a><a href="members.html">Members</a><a href="events.html">Events</a><a href="book.html">Book Online</a>
    </nav>
  </div>
</header>
<main>
  <h1>All Posts</h1>
  <div class="grid">
    <article class="card">
      <img src="images/post-decor.jpg" alt="Autumn leaves with person walking">
      <div class="meta">By ayushchadha • 2 min read • 250 views • 2 likes</div>
      <h3>Eco-Friendly Home Decor: Nature-Inspired Design Ideas</h3>
      <p>Are you looking to bring the beauty of nature into your home while also reducing your carbon footprint and promoting sustainability? If...</p>
    </article>
    <article class="card">
      <img src="images/post-plant.jpg" alt="Hands holding a small plant">
      <div class="meta">By ayushchadha • 2 min read • 230 views • 1 like</div>
      <h3>Protecting Our Planet: Simple Steps to Environmental Conservation</h3>
      <p>In an age where environmental conservation is more crucial than ever, it is important for individuals to take simple steps to protect our...</p>
    </article>
  </div>
</main>
<footer class="footer-sub">© 2025 Baw Baw Animal Rescue Inc.</footer>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Baw Baw Animal Rescue Inc. — Contact</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link href="https://fonts.googleapis.com/css2?family=Merriweather:wght@400;700;900&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="style.css">
</head>
<body>
<header>
  <div class="nav">
    <a class="brand" href="index.html"><img src="images/logo.png" alt=""><span>BAW BAW ANIMAL RESCUE INC.</span></a>
    <nav class="menu">
      <a href="index.html">Home</a><a href="about.html">About</a><a href="blog.html">Blog</a><a class="active" href="contact.html">Contact</a><a href="donate.html">Donate</a><a href="events.html">Events</a><a href="book.html">Book Online</a>
    </nav>
  </div>
</header>
<main>
  <h1>Get Involved</h1>
  <div class="grid cols-2">
    <form class="card">
      <div class="field"><label>First name *</label><input type="text" placeholder="First name" required></div>
      <div class="field"><label>Last name *</label><input type="text" placeholder="Last name" required></div>
      <div class="field"><label>Email *</label><input type="email" placeholder="you@example.com" required></div>
      <div class="field"><label>Phone</label><input type="tel" placeholder="0400 000 000"></div>
      <div class="field"><label>Message</label><textarea rows="6" placeholder="How can we help?"></textarea></div>
      <button class="btn" type="submit">Submit</button>
    </form>
    <div class="card">
      <p>At Baw Baw Animal Rescue Inc., we are dedicated to supporting animals in need and promoting responsible pet ownership. Whether you have questions about adoption, want to volunteer, or are interested in collaborating with us, we are here to listen and assist you.</p>
      <p class="meta">Feel free to reach out to us with any inquiries, feedback, or partnership requests.</p>
    </div>
  </div>
</main>
<footer class="footer-sub">© 2025 Baw Baw Animal Rescue Inc.</footer>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Baw Baw Animal Rescue Inc. — Donate</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link href="https://fonts.googleapis.com/css2?family=Merriweather:wght@400;700;900&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="style.css">
</head>
<body>
<header>
  <div class="nav">
    <a class="brand" href="index.html"><img src="images/logo.png" alt=""><span>BAW BAW ANIMAL RESCUE INC.</span></a>
    <nav class="menu">
      <a href="index.html">Home</a><a href="about.html">About</a><a href="blog.html">Blog</a><a href="contact.html">Contact</a><a class="active" href="donate.html">Donate</a><a href="subscriptions.html">My Subscriptions</a><a href="notifications.html">Notifications</a><a href="groups.html">Groups</a><a href="members.html">Members</a><a href="events.html">Events</a><a href="book.html">Book Online</a>
    </nav>
  </div>
</header>
<main>
  <h1>Make a difference</h1>
  <div class="grid cols-2">
    <div class="card"><img src="images/donate-koi.jpg" alt="Bright koi fish swimming"></div>
    <form class="card">
      <p>Change starts with people like you. Your donation helps make a real impact, one action at a time. Together, we can do more.</p>
      <div class="field"><label>Frequency</label>
        <select><option>One time</option><option>Monthly</option><option>Yearly</option></select>
      </div>
      <div class="pills"><span class="pill">$50</span><span class="pill">$100</span><span class="pill">$200</span><span class="pill">$1,000</span></div>
      <button class="btn" type="button">Donate $50</button>
      <p class="meta" style="margin-top:10px">This site can't accept donations right now. Upgrade your plan to start collecting donations.</p>
    </form>
  </div>
</main>
<footer class="footer-sub">© 2025 Baw Baw Animal Rescue Inc.</footer>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Baw Baw Animal Rescue Inc. — Subscriptions</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link href="https://fonts.googleapis.com/css2?family=Merriweather:wght@400;700;900&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="style.css">
</head>
<body>
<header>
  <div class="nav">
    <a class="brand" href="index.html"><img src="images/logo.png" alt=""><span>BAW BAW ANIMAL RESCUE INC.</span></a>
    <nav class="menu">
      <a href="index.html">Home</a><a href="about.html">About</a><a href="blog.html">Blog</a><a href="contact.html">Contact</a><a href="donate.html">Donate</a><a class="active" href="subscriptions.html">My Subscriptions</a><a href="notifications.html">Notifications</a><a href="groups.html">Groups</a><a href="members.html">Members</a><a href="events.html">Events</a><a href="book.html">Book Online</a>
    </nav>
  </div>
</header>
<main>
  <h1>Subscriptions</h1>
  <div class="grid cols-3">
    <div class="card">
      <h3>Beginner <span class="pill">Active</span></h3>
      <p>Free Plan</p>
      <p class="meta">Payments completed: 3 of 6</p>
      <p class="meta">Next payment: Nov 27, 2025</p>
      <p class="meta">Payment method: Visa ****9128</p>
    </div>
    <div class="card">
      <h3>Pro <span class="pill">Active</span></h3>
      <p class="meta">Expire: Nov 27, 2025</p>
    </div>
    <div class="card">
      <h3>VIP <span class="pill">Expired</span></h3>
      <p class="meta">Expire: Nov 27, 2025</p>
    </div>
  </div>
</main>
<footer class="footer-sub">© 2025 Baw Baw Animal Rescue Inc.</footer>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Baw Baw Animal Rescue Inc. — Notifications</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link href="https://fonts.googleapis.com/css2?family=Merriweather:wght@400;700;900&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="style.css">
</head>
<body>
<header>
  <div class="nav">
    <a class="brand" href="index.html">
      <img src="images/logo.png" alt="">
      <span>BAW BAW ANIMAL RESCUE INC. • ABN: 57 507 774 758</span>
    </a>
    <nav class="menu">
      <a href="index.html">Home</a><a href="about.html">About</a><a href="blog.html">Blog</a><a href="contact.html">Contact</a><a href="donate.html">Donate</a><a href="subscriptions.html">My Subscriptions</a><a class="active" href="notifications.html">Notifications</a><a href="groups.html">Groups</a><a href="members.html">Members</a><a href="events.html">Events</a><a href="book.html">Book Online</a>
    </nav>
  </div>
</header>
<main>
  <h1>Notifications</h1>
  <div class="grid">
    <div class="card"><strong>John Smith</strong> likes your post “some post”. <span class="meta">now</span></div>
    <div class="card"><strong>Chew Chang</strong> likes your post “some post”. <span class="meta">1 hour ago</span></div>
    <div class="card"><strong>Brad Pitt</strong> likes your post “some post”. <span class="meta">yesterday</span></div>
  </div>
</main>
<footer class="footer-sub">© 2025 Baw Baw Animal Rescue Inc.</footer>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Baw Baw Animal Rescue Inc. — Groups</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link href="https://fonts.googleapis.com/css2?family=Merriweather:wght@400;700;900&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="style.css">
</head>
<body>
<header>
  <div class="nav">
    <a class="brand" href="index.html"><img src="images/logo.png" alt=""><span>BAW BAW ANIMAL RESCUE GROUP</span></a>
    <nav class="menu">
      <a href="index.html">Home</a><a href="notifications.html">Notifications</a><a class="active" href="groups.html">Groups</a><a href="members.html">Members</a><a href="events.html">Events</a><a href="subscriptions.html">My Subscriptions</a><a href="book.html">Book Online</a>
    </nav>
  </div>
</header>
<main>
  <h1>Group Feed</h1>
  <div class="grid cols-2">
    <div class="card">
      <div class="meta">Posted 3 days ago • Baw Baw Animal Rescue Group</div>
      <strong>JaySanchu10</strong>
      <p>Welcome to the group Baw Baw Animal Rescue Group! A space for us to connect and share with each other. Start by posting something, sharing media, or creating a poll.</p>
      <div class="pills" style="margin:8px 0"><span class="pill">Comment</span><span class="pill">Like</span><span class="pill">Share</span></div>
      <hr style="margin:16px 0;border:none;border-top:1px solid #e0d3bb">
      <div class="pills"><span class="pill">Add Photo</span><span class="pill">Add Video</span><span class="pill">Add GIF</span></div>
      <div class="field"><textarea rows="3" placeholder="Create a post..."></textarea></div>
      <a class="btn" href="#">Create a Post</a>
    </div>
    <aside class="card">
      <div class="field"><label>Search</label><input type="search" placeholder="Search"></div>
      <h3>My Groups</h3>
      <p>Baw Baw Animal Rescue Group • 1 member</p>
      <p><a class="btn" href="#">Invite Members</a></p>
    </aside>
  </div>
</main>
<footer class="footer-sub">© 2025 Baw Baw Animal Rescue Inc.</footer>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Baw Baw Animal Rescue Inc. — Members</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link href="https://fonts.googleapis.com/css2?family=Merriweather:wght@400;700;900&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="style.css">
</head>
<body>
<header>
  <div class="nav">
    <a class="brand" href="index.html"><img src="images/logo.png" alt=""><span>BAW BAW ANIMAL RESCUE INC. • TO ALL CREATURES BIG AND SMALL</span></a>
    <nav class="menu">
      <a href="index.html">Home</a><a href="about.html">About</a><a href="blog.html">Blog</a><a href="contact.html">Contact</a><a href="donate.html">Donate</a><a href="subscriptions.html">My Subscriptions</a><a href="notifications.html">Notifications</a><a class="active" href="members.html">Members</a><a href="events.html">Events</a><a href="book.html">Book Online</a>
    </nav>
  </div>
</header>
<main>
  <h1>Members</h1>
  <div class="grid cols-2">
    <div class="card" style="display:flex;align-items:center;gap:14px">
      <img src="images/member-avatar.jpg" alt="Cloudy sky avatar" style="width:70px;height:70px;border-radius:50%">
      <div>
        <strong>joyclarkinfo</strong> <span class="pill">Admin 👑</span>
        <p><a class="btn" href="#">My Profile</a></p>
      </div>
    </div>
    <div class="card">
      <div class="field"><label>All members</label><select><option>All members</option><option>Admins</option><option>Volunteers</option></select></div>
      <div class="field"><label>Find a member...</label><input type="search" placeholder="Find a member..."></div>
      <div class="pills"><span class="pill">Grid</span><span class="pill">List</span></div>
    </div>
  </div>
</main>
<footer class="footer-sub">© 2025 Baw Baw Animal Rescue Inc.</footer>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Baw Baw Performing Arts Centre — Upcoming Events</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link href="https://fonts.googleapis.com/css2?family=Merriweather:wght@400;700;900&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="style.css">
</head>
<body>
<header>
  <div class="nav">
    <a class="brand" href="index.html"><img src="images/logo-performing-arts.png" alt=""><span>BAW BAW PERFORMING ARTS CENTRE</span></a>
    <nav class="menu">
      <a href="index.html">Home</a><a href="about.html">About</a><a href="blog.html">Blog</a><a href="contact.html">Contact</a><a href="donate.html">Donate</a><a href="subscriptions.html">My Subscriptions</a><a href="notifications.html">Notifications</a><a href="groups.html">Groups</a><a href="members.html">Members</a><a class="active" href="events.html">Events</a><a href="book.html">Book Online</a>
    </nav>
  </div>
</header>
<main>
  <h1>Upcoming Events</h1>
  <div class="grid cols-3">
    <div class="card">
      <img src="images/event-soul.jpg" alt="Keyboard on yellow">
      <h3>Soul Concert</h3>
      <p class="meta">Tue, 09 Jan • Mountain View</p>
      <p><a class="btn" href="#">More info</a> <a class="btn" href="#">RSVP</a></p>
    </div>
    <div class="card">
      <img src="images/event-ballet.jpg" alt="Ballet leap on orange">
      <h3>Modern Ballet</h3>
      <p class="meta">Tue, 06 Feb • Filarton District</p>
      <p><a class="btn" href="#">More info</a> <a class="btn" href="#">RSVP</a></p>
    </div>
    <div class="card">
      <img src="images/event-album.jpg" alt="Album launch on green">
      <h3>Album Launch</h3>
      <p class="meta">Sat, 17 Mar • West Village</p>
      <p><a class="btn" href="#">More info</a> <a class="btn" href="#">RSVP</a></p>
    </div>
  </div>
</main>
<footer class="footer-sub">© 2025 Baw Baw Performing Arts Centre</footer>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Baw Baw Animal Rescue Inc. — Book Online</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link href="https://fonts.googleapis.com/css2?family=Merriweather:wght@400;700;900&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="style.css">
</head>
<body>
<header>
  <div class="nav">
    <a class="brand" href="index.html"><img src="images/logo.png" alt=""><span>BAW BAW ANIMAL RESCUE INC.</span></a>
    <nav class="menu">
      <a href="index.html">Home</a><a href="about.html">About</a><a href="blog.html">Blog</a><a href="contact.html">Contact</a><a href="donate.html">Donate</a><a href="subscriptions.html">My Subscriptions</a><a href="notifications.html">Notifications</a><a href="groups.html">Groups</a><a href="members.html">Members</a><a href="events.html">Events</a><a class="active" href="book.html">Book Online</a>
    </nav>
  </div>
</header>
<main>
  <h1>Our Services</h1>
  <div class="pills" style="margin-bottom:10px">
    <span class="pill">All Services</span><span class="pill">Category 1</span><span class="pill">Category 2</span><span class="pill">Category 3</span>
  </div>
  <div class="grid cols-3">
    <div class="card">
      <img src="images/service-portrait.jpg" alt="Portrait on teal">
      <h3>Service name</h3>
      <p class="meta">USD 45</p>
      <a class="btn" href="#">Book Now</a>
    </div>
    <div class="card">
      <img src="images/service-ceramics.jpg" alt="Pink ceramic dishes">
      <h3>Service name</h3>
      <p class="meta">USD 45</p>
      <a class="btn" href="#">Book Now</a>
    </div>
    <div class="card">
      <img src="images/service-stairs.jpg" alt="Green stairwell">
      <h3>Service name</h3>
      <p class="meta">USD 45</p>
      <a class="btn" href="#">Book Now</a>
    </div>
  </div>
</main>
<footer class="footer-sub">© 2025 Baw Baw Animal Rescue Inc.</footer>
</body>
</html>
bawbaw-site/
  index.html
  about.html
  blog.html
  contact.html
  donate.html
  subscriptions.html
  notifications.html
  groups.html
  members.html
  events.html
  book.html
  style.css
  images/
    logo.png
    home-hero-kangaroo.jpg
    home-mission-tree.jpg
    blog-1-shoes.jpg
    blog-2-beach.jpg
    blog-3-portrait.jpg
    sugar-glider.jpg
    lizard.jpg
    parrot.jpg
    echidna.jpg
    about-koalas.jpg
    post-decor.jpg
    post-plant.jpg
    donate-koi.jpg
    member-avatar.jpg
    logo-performing-arts.png
    event-soul.jpg
    event-ballet.jpg
    event-album.jpg
    service-portrait.jpg
    service-ceramics.jpg
    service-stairs.jpg
