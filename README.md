[index.html](https://github.com/user-attachments/files/23780635/index.html)
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
