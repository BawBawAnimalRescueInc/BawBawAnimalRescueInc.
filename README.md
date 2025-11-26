[Uploading index.html…]()
<!-- ===== shared.css ===== -->
<style>
  :root{
    --bg:#f6c28b;        /* warm orange */
    --text:#2b5f4a;      /* deep green */
    --ink:#7a5f3a;       /* brown accent for headings */
    --white:#ffffff;
    --muted:#f8e7cf;
    --btn:#2f7d5f;       /* green button */
    --radius:14px;
    --shadow:0 6px 18px rgba(0,0,0,.12);
    --max:1100px;
  }
  *{box-sizing:border-box}
  html,body{margin:0;padding:0}
  body{
    font-family:'Merriweather',serif;
    background:var(--bg);
    color:var(--text);
    line-height:1.7;
  }
  a{color:var(--text);text-decoration:none}
  img{max-width:100%;display:block;border-radius:12px}
  header{
    background:var(--white);
    border-bottom:1px solid rgba(0,0,0,.1);
    position:sticky;top:0;z-index:50;
  }
  .nav{
    max-width:var(--max);margin:0 auto;padding:12px 18px;
    display:flex;align-items:center;justify-content:space-between;gap:14px;
  }
  .brand{display:flex;align-items:center;gap:12px;font-weight:900;color:var(--text)}
  .brand img{height:40px}
  .menu{display:flex;flex-wrap:wrap;gap:12px}
  .menu a{font-weight:700;padding:8px 10px;border-radius:10px}
  .menu a.active{background:var(--muted)}
  main{max-width:var(--max);margin:0 auto;padding:34px 18px}
  h1,h2,h3{color:var(--ink);margin:0 0 14px}
  .card{
    background:var(--white);border-radius:var(--radius);
    box-shadow:var(--shadow);padding:18px;
  }
  .grid{display:grid;gap:18px}
  @media(min-width:820px){
    .cols-2{grid-template-columns:1.2fr .8fr}
    .cols-3{grid-template-columns:repeat(3,1fr)}
  }
  .btn{
    display:inline-block;background:var(--btn);color:#fff;
    padding:10px 16px;border-radius:12px;font-weight:800
  }
  .pill{display:inline-block;border:1.5px solid var(--text);border-radius:999px;padding:6px 10px;font-weight:700}
  .sidebar{
    background:var(--white);border-radius:var(--radius);box-shadow:var(--shadow);padding:18px
  }
  .field{margin:10px 0}
  .field label{display:block;font-weight:700;margin-bottom:6px}
  .field input,.field textarea,.field select{
    width:100%;padding:10px 12px;border-radius:10px;border:1px solid #d7c7ad;background:#fff;font-family:'Merriweather',serif
  }
  .meta{color:#5b4a33;font-size:.9rem}
  footer{
    background:var(--white);border-top:1px solid rgba(0,0,0,.1);
    margin-top:30px;padding:22px 18px;color:#5b4a33;text-align:center
  }
  .subblock{
    background:var(--white);border-radius:16px;box-shadow:var(--shadow);padding:18px
  }
  .list{display:flex;gap:8px;flex-wrap:wrap}
  .list .tag{background:var(--muted);border-radius:999px;padding:6px 10px;font-weight:700}
</style>

<!-- ===== shared header/footer snippet (use in all pages) ===== -->
<!-- Link Google Font once per page head -->
<link href="https://fonts.googleapis.com/css2?family=Merriweather:wght@400;700;900&display=swap" rel="stylesheet">

<!-- ========================= index.html (Home) ========================= -->
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Baw Baw Animal Rescue Inc. — Home</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <!-- inject shared.css + font above -->
</head>
<body>
<header>
  <div class="nav">
    <a class="brand" href="index.html">
      <img src="logo.png" alt="Baw Baw Animal Rescue Inc.">
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
  <h1>Welcome to Baw Baw Animal Rescue Inc.</h1>
  <div class="grid cols-2">
    <div class="card">
      <img src="home-hero-kangaroo.jpg" alt="Kangaroo crossing rural road at sunset">
      <p>Our mission is to rescue, care for, and rehome animals in need, while promoting responsible pet ownership and reducing animal suffering. As a non‑profit, every resource we receive goes directly toward saving lives and giving animals a second chance.</p>
      <p><a class="btn" href="about.html">Learn More</a></p>
    </div>
    <div class="subblock">
      <h3>Stay connected</h3>
      <div class="field">
        <label>Email *</label>
        <input type="email" placeholder="you@example.com">
      </div>
      <div class="field" style="display:flex;align-items:center;gap:8px">
        <input type="checkbox" id="sub1">
        <label for="sub1">I want to subscribe to your mailing list.</label>
      </div>
      <p><a class="btn" href="#">Subscribe</a></p>
      <p class="meta">Privacy Policy • Accessibility Statement</p>
    </div>
  </div>
</main>

<footer>
  © 2025 Baw Baw Animal Rescue Inc. — ABN 43 925 209 665
</footer>
</body>
</html>

<!-- ========================= about.html (About / Our Mission) ========================= -->
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Baw Baw Animal Rescue Inc. — About</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <!-- inject shared.css + font -->
</head>
<body>
<header>
  <div class="nav">
    <a class="brand" href="index.html"><img src="logo.png" alt=""><span>BAW BAW ANIMAL RESCUE INC.</span></a>
    <nav class="menu">
      <a href="index.html">Home</a><a class="active" href="about.html">About</a><a href="blog.html">Blog</a><a href="contact.html">Contact</a><a href="donate.html">Donate</a><a href="subscriptions.html">My Subscriptions</a><a href="notifications.html">Notifications</a><a href="groups.html">Groups</a><a href="members.html">Members</a><a href="events.html">Events</a><a href="book.html">Book Online</a>
    </nav>
  </div>
</header>
<main>
  <h1 style="color:#e4792f">Our Mission</h1>
  <div class="grid cols-2">
    <div class="card">
      <img src="about-koalas.jpg" alt="Two koalas on a tree">
    </div>
    <div class="card">
      <p style="color:#e4792f"><strong>At Baw Baw Animal Rescue</strong> our mission is to rescue, care for, and rehome animals in need, while promoting responsible pet ownership and reducing animal suffering. As a non‑profit, every resource we receive goes directly toward saving lives and giving animals a second chance.</p>
      <p><a class="btn" href="index.html">Learn More</a></p>
    </div>
  </div>
</main>
<footer>© 2025 Baw Baw Animal Rescue Inc.</footer>
</body>
</html>

<!-- ========================= blog.html (All Posts) ========================= -->
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Baw Baw Animal Rescue Inc. — Blog</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <!-- inject shared.css + font -->
</head>
<body>
<header>
  <div class="nav">
    <a class="brand" href="index.html"><img src="logo.png" alt=""><span>BAW BAW ANIMAL RESCUE INC.</span></a>
    <nav class="menu">
      <a href="index.html">Home</a><a href="about.html">About</a><a class="active" href="blog.html">Blog</a><a href="contact.html">Contact</a><a href="donate.html">Donate</a><a href="subscriptions.html">My Subscriptions</a><a href="notifications.html">Notifications</a><a href="groups.html">Groups</a><a href="members.html">Members</a><a href="events.html">Events</a><a href="book.html">Book Online</a>
    </nav>
  </div>
</header>
<main>
  <h1>All Posts</h1>
  <div class="grid">
    <article class="card">
      <img src="post-decor.jpg" alt="Autumn leaves with city lights">
      <div class="meta">By @jacksmith • 2 min read • 250 views • 12 likes</div>
      <h3>Eco‑Friendly Home Decor: Nature‑Inspired Design Ideas</h3>
      <p>Are you looking to bring the beauty of nature into your home while also reducing your carbon footprint and promoting sustainability?...</p>
    </article>
    <article class="card">
      <img src="post-plant.jpg" alt="Hands holding a small plant">
      <div class="meta">By @janesmith • 2 min read • 180 views • 14 likes</div>
      <h3>Protecting Our Planet: Simple Steps to Environmental Conservation</h3>
      <p>In an age where environmental conservation is more crucial than ever, it is important for individuals to take simple steps to protect our...</p>
    </article>
  </div>
  <div class="subblock" style="margin-top:18px">
    <h3>Stay connected</h3>
    <div class="field"><label>Email *</label><input type="email" placeholder="you@example.com"></div>
    <div class="field" style="display:flex;gap:8px;align-items:center"><input type="checkbox" id="subb"><label for="subb">I want to subscribe to your mailing list.</label></div>
    <a class="btn" href="#">Subscribe</a>
    <p class="meta" style="margin-top:8px">123‑456‑7890 • info@mysite.com • 500 Terry Francine St.</p>
    <p class="meta">Privacy Policy • Accessibility Statement</p>
  </div>
</main>
<footer>© 2025 Baw Baw Animal Rescue Inc.</footer>
</body>
</html>

<!-- ========================= contact.html (Contact) ========================= -->
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Baw Baw Animal Rescue Inc. — Contact</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <!-- inject shared.css + font -->
</head>
<body>
<header>
  <div class="nav">
    <a class="brand" href="index.html"><img src="logo.png" alt=""><span>BAW BAW ANIMAL RESCUE INC.</span></a>
    <nav class="menu">
      <a href="index.html">Home</a><a href="about.html">About</a><a href="blog.html">Blog</a><a class="active" href="contact.html">Contact</a><a href="donate.html">Donate</a><a href="subscriptions.html">My Subscriptions</a><a href="notifications.html">Notifications</a><a href="groups.html">Groups</a><a href="members.html">Members</a><a href="events.html">Events</a><a href="book.html">Book Online</a>
    </nav>
  </div>
</header>
<main>
  <h1>Get Involved</h1>
  <div class="grid cols-2">
    <form class="card">
      <div class="field"><label>Name</label><input type="text" placeholder="Full name"></div>
      <div class="field"><label>Email</label><input type="email" placeholder="you@example.com"></div>
      <div class="field"><label>Phone</label><input type="tel" placeholder="0400 000 000"></div>
      <div class="field"><label>Message</label><textarea rows="6" placeholder="How can we help?"></textarea></div>
      <button class="btn" type="submit">Submit</button>
    </form>
    <div class="card">
      <p>At Baw Baw Animal Rescue Inc., we are dedicated to supporting animals in need and promoting responsible pet ownership. Whether you have questions about adoption, want to volunteer, or are interested in collaborating with us, we are here to listen and assist you.</p>
      <p class="meta">Feel free to reach out with any inquiries, feedback, or partnership requests.</p>
    </div>
  </div>
</main>
<footer>© 2025 Baw Baw Animal Rescue Inc.</footer>
</body>
</html>

<!-- ========================= donate.html (Donate) ========================= -->
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Baw Baw Animal Rescue Inc. — Donate</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <!-- inject shared.css + font -->
</head>
<body>
<header>
  <div class="nav">
    <a class="brand" href="index.html"><img src="logo.png" alt=""><span>BAW BAW ANIMAL RESCUE INC.</span></a>
    <nav class="menu">
      <a href="index.html">Home</a><a href="about.html">About</a><a href="blog.html">Blog</a><a href="contact.html">Contact</a><a class="active" href="donate.html">Donate</a><a href="subscriptions.html">My Subscriptions</a><a href="notifications.html">Notifications</a><a href="groups.html">Groups</a><a href="members.html">Members</a><a href="events.html">Events</a><a href="book.html">Book Online</a>
    </nav>
  </div>
</header>
<main>
  <h1>Make a difference</h1>
  <div class="grid cols-2">
    <div class="card">
      <img src="donate-koi.jpg" alt="Bright koi fish swimming">
    </div>
    <form class="card">
      <p>Change starts when people help you. Your donation helps make a real impact, one action at a time. Together, we can do more.</p>
      <div class="field">
        <label>Frequency</label>
        <select>
          <option>One time</option>
          <option>Monthly</option>
          <option>Yearly</option>
        </select>
      </div>
      <div class="list" style="margin:10px 0">
        <span class="tag">$50</span><span class="tag">$100</span><span class="tag">$200</span><span class="tag">$1,000</span>
      </div>
      <button class="btn" type="button">Donate $50</button>
      <p class="meta" style="margin-top:10px">This site can't accept donations right now.</p>
    </form>
  </div>
</main>
<footer>© 2025 Baw Baw Animal Rescue Inc.</footer>
</body>
</html>

<!-- ========================= subscriptions.html (My Subscriptions) ========================= -->
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Baw Baw Animal Rescue Inc. — My Subscriptions</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <!-- inject shared.css + font -->
</head>
<body>
<header>
  <div class="nav">
    <a class="brand" href="index.html"><img src="logo.png" alt=""><span>BAW BAW ANIMAL RESCUE INC.</span></a>
    <nav class="menu">
      <a href="index.html">Home</a><a href="about.html">About</a><a href="blog.html">Blog</a><a href="contact.html">Contact</a><a href="donate.html">Donate</a><a class="active" href="subscriptions.html">My Subscriptions</a><a href="notifications.html">Notifications</a><a href="groups.html">Groups</a><a href="members.html">Members</a><a href="events.html">Events</a><a href="book.html">Book Online</a>
    </nav>
  </div>
</header>
<main>
  <h1>My Subscriptions</h1>
  <div class="grid">
    <div class="card">
      <h3>Beginner <span class="pill">Active</span></h3>
      <p>Free Plan</p>
      <p class="meta">Payments completed: 3 of 6</p>
      <p class="meta">Next payment: Nov 27, 2025 • Last payment: Nov 27, 2025</p>
      <p class="meta">Payment method: Visa ****9128</p>
    </div>
    <div class="card">
      <h3>Pro <span class="pill">Active</span></h3>
      <p class="meta">Expires: Nov 27, 2025</p>
    </div>
    <div class="card">
      <h3>VIP <span class="pill">Expired</span></h3>
      <p class="meta">Expired: Nov 27, 2025</p>
    </div>
  </div>
  <div class="subblock" style="margin-top:18px">
    <h3>Stay connected</h3>
    <div class="field"><label>Email *</label><input type="email" placeholder="you@example.com"></div>
    <div class="field" style="display:flex;gap:8px;align-items:center"><input type="checkbox" id="subs"><label for="subs">I want to subscribe to your mailing list.</label></div>
    <a class="btn" href="#">Subscribe</a>
  </div>
</main>
<footer>© 2025 Baw Baw Animal Rescue Inc.</footer>
</body>
</html>

<!-- ========================= notifications.html (Notifications) ========================= -->
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Baw Baw Animal Rescue Inc. — Notifications</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <!-- inject shared.css + font -->
</head>
<body>
<header>
  <div class="nav">
    <a class="brand" href="index.html"><img src="logo.png" alt=""><span>BAW BAW ANIMAL RESCUE INC.</span></a>
    <nav class="menu">
      <a href="index.html">Home</a><a href="about.html">About</a><a href="blog.html">Blog</a><a href="contact.html">Contact</a><a href="donate.html">Donate</a><a href="subscriptions.html">My Subscriptions</a><a class="active" href="notifications.html">Notifications</a><a href="groups.html">Groups</a><a href="members.html">Members</a><a href="events.html">Events</a><a href="book.html">Book Online</a>
    </nav>
  </div>
</header>
<main>
  <h1>Notifications</h1>
  <p><a class="btn" href="#">Mark all as read (2)</a></p>
  <div class="grid">
    <div class="card"><strong>John Smith</strong> likes your post “some post”. <span class="meta">now</span></div>
    <div class="card"><strong>Chew Chang</strong> likes your post “some post”. <span class="meta">1 hour ago</span></div>
    <div class="card"><strong>Brad Pitt</strong> likes your post “some post”. <span class="meta">yesterday</span></div>
  </div>
</main>
<footer>© 2025 Baw Baw Animal Rescue Inc.</footer>
</body>
</html>

<!-- ========================= groups.html (Groups / Group Feed) ========================= -->
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Baw Baw Animal Rescue Inc. — Groups</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <!-- inject shared.css + font -->
</head>
<body>
<header>
  <div class="nav">
    <a class="brand" href="index.html"><img src="logo.png" alt=""><span>BAW BAW ANIMAL RESCUE INC.</span></a>
    <nav class="menu">
      <a href="index.html">Home</a><a href="notifications.html">Notifications</a><a class="active" href="groups.html">Groups</a><a href="members.html">Members</a><a href="events.html">Events</a><a href="subscriptions.html">My Subscriptions</a><a href="book.html">Book Online</a>
    </nav>
  </div>
</header>
<main>
  <h1>Group Feed</h1>
  <div class="grid cols-2">
    <div class="card">
      <div class="list" style="margin-bottom:10px">
        <a class="tag" href="#">Add Photo</a><a class="tag" href="#">Add Video</a><a class="tag" href="#">Add GIF</a>
      </div>
      <div class="field"><textarea rows="4" placeholder="Share something with the group..."></textarea></div>
      <a class="btn" href="#">Create a Post</a>
      <hr style="margin:18px 0;border:none;border-top:1px solid #e0d3bb">
      <div class="card" style="background:#fff">
        <strong>JaySanchu</strong>
        <p>Welcome to the group Baw Baw Animal Rescue Group! A space for us to connect and share with each other. Start by posting, sharing, commenting, and creating a post.</p>
        <div class="field"><input type="text" placeholder="Write a comment..."></div>
      </div>
    </div>
    <aside class="sidebar">
      <div class="field"><label>Search</label><input type="search" placeholder="Search"></div>
      <h3>My Groups</h3>
      <div class="card" style="margin-top:8px">
        <strong>Baw Baw Animal Rescue Group</strong>
        <p><a class="btn" href="#">Leave Group</a></p>
      </div>
      <div class="card" style="margin-top:12px">
        <h3>Invite Members</h3>
        <p>Send out personal invites to get more members in your group.</p>
      </div>
    </aside>
  </div>
</main>
<footer>© 2025 Baw Baw Animal Rescue Inc.</footer>
</body>
</html>

<!-- ========================= members.html (Members) ========================= -->
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Baw Baw Animal Rescue Inc. — Members</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <!-- inject shared.css + font -->
</head>
<body>
<header>
  <div class="nav">
    <a class="brand" href="index.html"><img src="logo.png" alt=""><span>BAW BAW ANIMAL RESCUE INC. • ABN 43 925 209 665</span></a>
    <nav class="menu">
      <a href="index.html">Home</a><a href="about.html">About</a><a href="blog.html">Blog</a><a href="contact.html">Contact</a><a href="donate.html">Donate</a><a href="subscriptions.html">My Subscriptions</a><a href="notifications.html">Notifications</a><a class="active" href="members.html">Members</a><a href="events.html">Events</a><a href="book.html">Book Online</a>
    </nav>
  </div>
</header>
<main>
  <h1>Members</h1>
  <div class="grid cols-2">
    <div class="card" style="display:flex;align-items:center;gap:14px">
      <img src="member-joyclarkinfo.jpg" alt="Cloudy sky avatar" style="width:70px;height:70px;border-radius:50%">
      <div>
        <strong>joyclarkinfo</strong> <span class="pill">Admin</span>
        <p><a class="btn" href="#">My Profile</a></p>
      </div>
    </div>
    <div class="card">
      <div class="field"><label>All members</label><select><option>All members</option><option>Admins</option><option>Volunteers</option></select></div>
      <div class="field"><label>Find a member...</label><input type="search" placeholder="Search members"></div>
      <div class="list"><span class="tag">Grid</span><span class="tag">List</span></div>
    </div>
  </div>
</main>
<footer>© 2025 Baw Baw Animal Rescue Inc.</footer>
</body>
</html>

<!-- ========================= events.html (Upcoming Events) ========================= -->
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Baw Baw Animal Rescue Inc. — Events</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <!-- inject shared.css + font -->
</head>
<body>
<header>
  <div class="nav">
    <a class="brand" href="index.html"><img src="logo.png" alt=""><span>BAW BAW ANIMAL RESCUE INC.</span></a>
    <nav class="menu">
      <a href="index.html">Home</a><a href="about.html">About</a><a href="blog.html">Blog</a><a href="contact.html">Contact</a><a href="donate.html">Donate</a><a href="subscriptions.html">My Subscriptions</a><a href="notifications.html">Notifications</a><a href="groups.html">Groups</a><a href="members.html">Members</a><a class="active" href="events.html">Events</a><a href="book.html">Book Online</a>
    </nav>
  </div>
</header>
<main>
  <h1>Upcoming Events</h1>
  <div class="grid cols-3">
    <div class="card">
      <img src="event-soul.jpg" alt="Soul concert keyboard on yellow">
      <h3>Soul Concert</h3>
      <p class="meta">Tue, 09 Jan • Mountain View</p>
      <p><a class="btn" href="#">More info</a> <a class="btn" href="#">RSVP</a></p>
    </div>
    <div class="card">
      <img src="event-ballet.jpg" alt="Modern ballet leap on orange">
      <h3>Modern Ballet</h3>
      <p class="meta">Tue, 06 Feb • Filation District</p>
      <p><a class="btn" href="#">More info</a> <a class="btn" href="#">RSVP</a></p>
    </div>
    <div class="card">
      <img src="event-album.jpg" alt="Album launch with microphone on green">
      <h3>Album Launch</h3>
      <p class="meta">Sat, 17 Mar • West Village</p>
      <p><a class="btn" href="#">More info</a> <a class="btn" href="#">RSVP</a></p>
    </div>
  </div>
</main>
<footer>© 2025 Baw Baw Animal Rescue Inc.</footer>
</body>
</html>

<!-- ========================= book.html (Book Online / Services) ========================= -->
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Baw Baw Animal Rescue Inc. — Book Online</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <!-- inject shared.css + font -->
</head>
<body>
<header>
  <div class="nav">
    <a class="brand" href="index.html"><img src="logo.png" alt=""><span>BAW BAW ANIMAL RESCUE INC.</span></a>
    <nav class="menu">
      <a href="index.html">Home</a><a href="about.html">About</a><a href="blog.html">Blog</a><a href="contact.html">Contact</a><a href="donate.html">Donate</a><a href="subscriptions.html">My Subscriptions</a><a href="notifications.html">Notifications</a><a href="groups.html">Groups</a><a href="members.html">Members</a><a href="events.html">Events</a><a class="active" href="book.html">Book Online</a>
    </nav>
  </div>
</header>
<main>
  <h1>Our Services</h1>
  <div class="list" style="margin-bottom:12px">
    <span class="tag">All Services</span><span class="tag">Category 1</span><span class="tag">Category 2</span><span class="tag">Category 3</span>
  </div>
  <div class="grid cols-3">
    <div class="card">
      <img src="service-portrait.jpg" alt="Portrait on teal">
      <h3>Service name</h3>
      <p class="meta">USD 45</p>
      <a class="btn" href="#">Book Now</a>
    </div>
    <div class="card">
      <img src="service-ceramics.jpg" alt="Pink ceramic dishes">
      <h3>Service name</h3>
      <p class="meta">USD 45</p>
      <a class="btn" href="#">Book Now</a>
    </div>
    <div class="card">
      <img src="service-stairs.jpg" alt="Green stairwell">
      <h3>Service name</h3>
      <p class="meta">USD 45</p>
      <a class="btn" href="#">Book Now</a>
    </div>
  </div>
</main>
<footer>© 2025 Baw Baw Animal Rescue Inc.</footer>
</body>
</html>
