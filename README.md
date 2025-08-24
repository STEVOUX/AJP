<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>AJP — Alliance for the Beard (Official)</title>
  <meta name="description" content="AJP — Antony Jose Padammattumal. People-first support & mental care. Famous for the BEARD. News, leadership, gallery, volunteer and contact." />
  <meta property="og:title" content="AJP — Antony Jose Padammattumal" />
  <meta property="og:description" content="Without Beard Our Leader Verum Monna — AJP official site" />
  <meta property="og:type" content="website" />
  <meta name="theme-color" content="#1f1020" />

  <!-- Fonts -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&family=Playfair+Display:wght@700&display=swap" rel="stylesheet">

  <style>
    :root{
      --bg:#0b0710;          /* deep dark */
      --bg-soft:#111217;     /* card background */
      --txt:#fff7f5;         /* primary text */
      --muted:#f0d9d6;       /* secondary text */
      --accent-1:#ff6f3c;    /* orange */
      --accent-2:#ff3b57;    /* rose/red */
      --accent-3:#ff9f1c;    /* saffron */
      --shadow: 0 10px 30px rgba(0,0,0,.5);
      --radius: 16px;
    }
    *{box-sizing:border-box}
    html{scroll-behavior:smooth}
    body{margin:0;font-family:Poppins,system-ui,-apple-system,Segoe UI,Roboto,Ubuntu,"Helvetica Neue",Arial; color:var(--txt); background:
      radial-gradient(1200px 800px at 80% -10%, rgba(40,20,10,0.35) 0%, transparent 50%),
      linear-gradient(180deg, #07050a 0%, var(--bg) 100%);}

    a{color:var(--accent-1);text-decoration:none}
    img{max-width:100%;display:block}
    .container{width:min(1200px,94%);margin-inline:auto}

    /* Header / Nav */
    header{position:sticky;top:0;z-index:80;background:linear-gradient(180deg, rgba(0,0,0,.45), rgba(0,0,0,.25));backdrop-filter: blur(6px);border-bottom:1px solid rgba(255,255,255,.03)}
    .nav{display:flex;align-items:center;justify-content:space-between;gap:12px;padding:12px 0}
    .brand{display:flex;align-items:center;gap:12px}
    .brand .logo{width:48px;height:48px;border-radius:12px;background:linear-gradient(135deg,var(--accent-3),var(--accent-1)); display:grid;place-items:center;color:#120406;font-weight:900;font-family:"Playfair Display",serif;box-shadow:var(--shadow);font-size:20px}
    .brand h1{font-family:"Playfair Display",serif; font-size:20px;letter-spacing:.2px;margin:0}
    .brand small{display:block;color:var(--muted);font-weight:600;line-height:1.05;font-size:12px}
    .links{display:flex;gap:16px;align-items:center;white-space:nowrap}
    .links a{color:var(--txt);opacity:.95;font-weight:700;padding:8px 10px;border-radius:10px}
    .links a:hover{color:var(--accent-3);background:rgba(255,255,255,.02)}
    .btn{display:inline-flex;align-items:center;gap:10px;padding:10px 16px;border-radius:999px;border:1px solid rgba(255,255,255,.06);color:var(--txt);font-weight:700;background:linear-gradient(180deg,rgba(255,255,255,.02),rgba(255,255,255,.01));box-shadow:var(--shadow)}
    .hamburger{display:none;border:1px solid rgba(255,255,255,.06);background:transparent;border-radius:12px;padding:8px;color:var(--txt)}

    /* Hero */
    .hero{position:relative;overflow:hidden;padding-bottom:18px}
    .hero::before{content:"";position:absolute;inset:0;background-image:url('https://cdn.discordapp.com/attachments/1361326986131149063/1409146094918701076/AJP_1.jpg?ex=68ac5111&is=68aaff91&hm=e72f4ef6b2efb953a57dff32022d298921d98c1882f012a114161066bff753e1&');background-size:cover;background-position:center;opacity:.26;filter:grayscale(8%) contrast(105%) saturate(110%)}
    .hero .overlay{position:absolute;inset:0;background:linear-gradient(180deg, rgba(10,6,10,0.35), rgba(8,4,6,0.6));mix-blend-mode:multiply}
    .hero .wrap{position:relative;padding:84px 0 48px; display:grid;grid-template-columns:1.1fr .9fr;gap:28px;align-items:center}
    .pill{display:inline-flex;gap:10px;align-items:center;background:linear-gradient(90deg, rgba(255,111,60,.08), rgba(255,59,87,.06));border-radius:999px;padding:8px 12px;color:var(--muted);font-weight:700}
    .hero h2{font-family:"Playfair Display",serif;font-size:48px;line-height:1.02;margin:12px 0;color:var(--txt)}
    .hero p{color:var(--muted);font-size:16px}
    .hero .cta{display:flex;gap:12px;flex-wrap:wrap;margin-top:14px}
    .muted{color:var(--muted)}
    .card{background:linear-gradient(180deg, rgba(255,255,255,.02), rgba(255,255,255,.01));border:1px solid rgba(255,255,255,.04);border-radius:var(--radius);box-shadow:var(--shadow)}
    .highlight { color: var(--accent-2); font-weight:800; }

    /* grid */
    .grid{display:grid;gap:18px}
    .grid.cols-3{grid-template-columns:repeat(3,1fr)}
    .grid.cols-2{grid-template-columns:repeat(2,1fr)}
    .stat{display:flex;align-items:center;gap:12px}

    /* Leadership cards */
    .leader-card{display:flex;gap:12px;align-items:center;padding:14px;border-radius:12px}
    .leader-card img{width:92px;height:92px;border-radius:12px;object-fit:cover;border:2px solid rgba(255,255,255,.04)}
    .leader-card h4{margin:0;font-size:18px}
    .leader-card p{margin:0;color:var(--muted);font-size:13px}

    /* Gallery */
    .gallery{display:grid;grid-template-columns:repeat(6,1fr);gap:10px}
    .gallery img{border-radius:12px;cursor:pointer;border:1px solid rgba(255,255,255,.06);height:110px;object-fit:cover}

    /* Info / Contact */
    .info{display:grid;grid-template-columns:1.2fr 1fr;gap:22px}
    .map{border:0;width:100%;height:320px;border-radius:12px;filter:saturate(110%) contrast(110%)}

    /* News */
    .composer{display:grid;gap:10px}
    .composer input, .composer textarea{padding:12px;border-radius:10px;border:1px solid rgba(255,255,255,.06);background:rgba(255,255,255,.02);color:var(--txt)}
    .post{background:linear-gradient(180deg, rgba(255,255,255,.01), rgba(255,255,255,.02));border:1px solid rgba(255,255,255,.04);border-radius:12px;padding:12px}
    .post h4{margin:0 0 6px}
    .post time{color:var(--muted);font-size:12px}
    .post .post-meta{display:flex;gap:10px;align-items:center;flex-wrap:wrap;margin-top:10px}

    /* footer */
    footer{background:linear-gradient(180deg, rgba(255,255,255,.01), rgba(255,255,255,.02));border-top:1px solid rgba(255,255,255,.03);padding:22px 0;color:var(--muted)}

    /* responsive */
    @media (max-width:980px){
      .hero .wrap{grid-template-columns:1fr}
      .grid.cols-3{grid-template-columns:1fr 1fr}
      .info{grid-template-columns:1fr}
      .gallery{grid-template-columns:repeat(3,1fr)}
    }
    @media (max-width:760px){
      .links{display:none}
      .hamburger{display:inline-flex}
      .grid.cols-3, .grid.cols-2{grid-template-columns:1fr}
      .hero h2{font-size:34px}
      .gallery{grid-template-columns:repeat(2,1fr)}
      .gallery img{height:90px}
    }

    /* small helpers */
    .chip{display:inline-block;padding:6px 10px;border-radius:999px;background:rgba(255,255,255,.02);font-weight:700;color:var(--muted);font-size:13px}
    .center{display:flex;align-items:center;justify-content:center}
  </style>
</head>
<body>
  <!-- Header -->
  <header>
    <div class="container nav">
      <div class="brand">
        <div class="logo" aria-hidden>🧔</div>
        <div>
          <h1>AJP</h1>
          <small>Antony Jose Padammattumal — Official</small>
        </div>
      </div>

      <nav class="links" aria-label="Primary">
        <a href="#about">About</a>
        <a href="#leadership">Leadership</a>
        <a href="#news">News</a>
        <a href="#gallery">Gallery</a>
        <a href="#contact" class="btn">Contact</a>
      </nav>

      <button class="hamburger" id="menuBtn" aria-label="Open menu">☰</button>
    </div>
  </header>

  <!-- Hero -->
  <section class="hero" id="home">
    <div class="overlay"></div>
    <div class="container wrap">
      <div>
        <span class="pill">Since 1991 • People-first support</span>
        <h2>Without Beard Our Leader <span class="highlight">Verum Monna.</span></h2>
        <p class="muted">AJP — support & mental care for the people. We give food, clothes and hope. Our beard is our mark; our leader's beard is our symbol of courage and unity.</p>

        <div class="cta">
          <a href="#news" class="btn" style="background:linear-gradient(90deg,var(--accent-1),var(--accent-2));border-color:transparent">Latest News</a>
          <a href="#contact" class="btn" style="border-color:rgba(255,159,28,.18)">Volunteer / Join</a>
        </div>

        <div id="latestNewsPeek" class="muted" style="margin-top:14px"></div>
      </div>

      <div class="card schedule" style="padding:18px">
        <h3 style="margin:0 0 10px">About AJP</h3>
        <p class="muted" style="margin:0 0 12px">Founded in <strong>1991</strong>, AJP is a grassroots organization focused on community support, mental care, food distribution and dignity for the poor. We are united by a symbol — the BEARD — which represents our identity and values.</p>

        <div style="display:grid;gap:10px;margin-top:12px">
          <div class="stat"><span class="chip">Founder</span> <strong style="margin-left:8px">Antony Jose Padammattumal</strong></div>
          <div class="stat"><span class="chip">Co-Leader</span> <strong style="margin-left:8px">Fadhil MS</strong></div>
          <div class="stat"><span class="chip">Supporter</span> <strong style="margin-left:8px">Steve Shine</strong></div>
        </div>

        <div style="margin-top:14px;display:flex;gap:10px;flex-wrap:wrap">
          <a class="btn" href="#leadership">Meet the Team</a>
          <a class="btn" href="#gallery">Gallery</a>
        </div>

      </div>
    </div>
  </section>

  <!-- About -->
  <section id="about">
    <div class="container">
      <div class="section-head">
        <h3>About AJP</h3>
        <p class="muted">People • Dignity • Beard</p>
      </div>

      <div class="grid cols-2">
        <div class="card" style="padding:20px">
          <p>AJP (since 1991) champions community support and mental care. We feed people, provide clothing, and run outreach services that restore dignity. The BEARD is our mark — a symbol of identity, unity and courage.</p>

          <ul style="line-height:1.9" class="muted">
            <li><strong>Founded:</strong> 1991</li>
            <li><strong>Main focus:</strong> Food distribution, mental care, clothing drives</li>
            <li><strong>Symbol:</strong> The Beard — our slogan: <em>Without Beard Our Leader Verum Monna.</em></li>
          </ul>

          <a class="btn" href="#contact">Get Involved</a>
        </div>

        <div class="grid cols-2">
          <div class="card" style="padding:18px">
            <div class="stat"><span class="chip">Mission</span><h4 style="margin:6px 0 0">Serve & Support</h4></div>
            <p class="muted">Relieve immediate need and build lasting care programs.</p>
          </div>
          <div class="card" style="padding:18px">
            <div class="stat"><span class="chip">Values</span><h4 style="margin:6px 0 0">Respect • Dignity</h4></div>
            <p class="muted">Humane, practical, and community-led.</p>
          </div>
          <div class="card" style="padding:18px">
            <div class="stat"><span class="chip">Identity</span><h4 style="margin:6px 0 0">The Beard</h4></div>
            <p class="muted">Our unmistakable mark of unity.</p>
          </div>
          <div class="card" style="padding:18px">
            <div class="stat"><span class="chip">Contact</span><h4 style="margin:6px 0 0">steveshine999@gmail.com</h4></div>
            <p class="muted">Call / Whatsapp: +91 8921370655</p>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Leadership -->
  <section id="leadership">
    <div class="container">
      <div class="section-head">
        <h3>Leadership</h3>
        <p class="muted">Meet the people who lead AJP</p>
      </div>

      <div class="grid cols-3">
        <article class="card leader-card" style="padding:12px">
          <img src="https://cdn.discordapp.com/attachments/1361326986131149063/1409146095195652127/Ajp_2.jpg?ex=68ac5111&is=68aaff91&hm=1f751725285f077453e4d4f787b4475dd9c625e1e2e401402bc28647cdc7e82d&" alt="Antony Jose Padammattumal">
          <div>
            <h4>Antony Jose Padammattumal</h4>
            <p class="muted">Leader • Founder (The Beard)</p>
            <p style="margin-top:8px;color:var(--muted)">"Without Beard Our Leader Verum Monna."</p>
          </div>
        </article>

        <article class="card leader-card" style="padding:12px">
          <img src="https://cdn.discordapp.com/attachments/1361326986131149063/1409148028463353938/Fadhil.jpg?ex=68ac52de&is=68ab015e&hm=f95eea1b35c07376d583fddba0aaf60f19eac2fc78ff093746c61e21b1b44433" alt="Fadhil MS">
          <div>
            <h4>Fadhil MS</h4>
            <p class="muted">Co-Leader • Main Supporter</p>
            <p class="muted" style="margin-top:8px">Support & coordination</p>
          </div>
        </article>

        <article class="card leader-card" style="padding:12px">
          <img src="https://cdn.discordapp.com/attachments/1361326986131149063/1409148341496975440/a32e85fca033a11b9526978f958478b1.jpg?ex=68ac5329&is=68ab01a9&hm=aa6a6043bfa03179aded5cbb3feaf85d2ab30c4a656860e4b5628418016dcf1e" alt="Steve Shine">
          <div>
            <h4>Steve Shine</h4>
            <p class="muted">Supporter • Webmaster</p>
          </div>
        </article>
      </div>
    </div>
  </section>

  <!-- News -->
  <section id="news">
    <div class="container">
      <div class="section-head">
        <h3>News & Announcements</h3>
        <p class="muted">Latest updates from AJP</p>
      </div>

      <!-- Composer -->
      <div class="card" style="padding:16px;margin-bottom:16px">
        <form id="newsForm" class="composer">
          <input type="text" name="title" placeholder="Post title (e.g., Food Drive at Market)" required>
          <textarea name="body" rows="3" placeholder="Write your announcement…" required></textarea>

          <div style="display:flex;gap:10px;align-items:center;flex-wrap:wrap;margin-top:8px">
            <input type="text" name="author" placeholder="Posted by (optional)" style="flex:1 1 240px">
            <button class="btn" type="submit">Post Update</button>
            <button class="btn" type="button" id="clearNews" title="Clear all saved posts" style="background:linear-gradient(180deg,rgba(255,59,87,.12),rgba(255,59,87,.04));border-color:rgba(255,59,87,.25)">Clear All</button>
          </div>

          <small class="muted" style="display:block;margin-top:8px">Local only: posts are saved in your browser (localStorage).</small>
        </form>
      </div>

      <!-- Feed -->
      <div id="newsFeed" class="grid cols-2"></div>
    </div>
  </section>

  <!-- Gallery -->
  <section id="gallery">
    <div class="container">
      <div class="section-head">
        <h3>Gallery</h3>
        <p class="muted">Moments from our work (click to enlarge)</p>
      </div>

      <div class="card" style="padding:14px;margin-bottom:12px">
        <form id="galleryForm" style="display:flex;gap:12px;align-items:center;flex-wrap:wrap">
          <input type="file" id="galleryInput" accept="image/*" multiple>
          <button type="button" class="btn" id="addToGallery">Add Selected Photos</button>
          <small class="muted">Photos stored locally in browser (no server).</small>
        </form>
      </div>

      <div class="gallery" id="galleryGrid" aria-live="polite">
        <!-- Preloaded -->
        <img src="https://cdn.discordapp.com/attachments/1361326986131149063/1409146094918701076/AJP_1.jpg?ex=68ac5111&is=68aaff91&hm=e72f4ef6b2efb953a57dff32022d298921d98c1882f012a114161066bff753e1&" alt="AJP banner" data-origin="starter">
        <img src="https://cdn.discordapp.com/attachments/1361326986131149063/1409146095195652127/Ajp_2.jpg?ex=68ac5111&is=68aaff91&hm=1f751725285f077453e4d4f787b4475dd9c625e1e2e401402bc28647cdc7e82d&" alt="Leader Antony" data-origin="starter">
        <img src="https://cdn.discordapp.com/attachments/1361326986131149063/1409148028463353938/Fadhil.jpg?ex=68ac52de&is=68ab015e&hm=f95eea1b35c07376d583fddba0aaf60f19eac2fc78ff093746c61e21b1b44433" alt="Fadhil" data-origin="starter">
        <img src="https://cdn.discordapp.com/attachments/1361326986131149063/1409148341496975440/a32e85fca033a11b9526978f958478b1.jpg?ex=68ac5329&is=68ab01a9&hm=aa6a6043bfa03179aded5cbb3feaf85d2ab30c4a656860e4b5628418016dcf1e" alt="Steve Shine" data-origin="starter">
        <img src="https://cdn.discordapp.com/attachments/1361326986131149063/1409150870922203278/poster.jpg?ex=68ac5584&is=68ab0404&hm=7b9fd4c97f0315627acb5af602c6d14fbf1b4d9ab3f4c6d502e5594fe95f2be3" alt="Poster 07-08-2025" data-origin="starter">
      </div>
    </div>
  </section>

  <!-- Contact -->
  <section id="contact">
    <div class="container info">
      <div class="card" style="padding:18px">
        <div class="section-head" style="margin-bottom:6px">
          <h3>Contact & Volunteer</h3>
          <p class="muted">Join our outreach or send queries</p>
        </div>

        <p class="muted">
          <strong>AJP — Antony Jose Padammattumal</strong><br>
          Founded 1991 • Community support & mental care<br>
          Email: <a href="mailto:steveshine999@gmail.com">steveshine999@gmail.com</a><br>
          Phone: <a href="tel:+918921370655">+91 8921370655</a>
        </p>

        <form id="msgForm" class="grid cols-2" style="gap:12px;margin-top:8px">
          <input class="card" name="name" placeholder="Your name" required style="padding:12px;border-radius:10px;border:1px solid rgba(255,255,255,.04);background:transparent;color:var(--txt)">
          <input class="card" name="email" placeholder="Email" type="email" required style="padding:12px;border-radius:10px;border:1px solid rgba(255,255,255,.04);background:transparent;color:var(--txt)">
          <input class="card" name="phone" placeholder="Phone (optional)" style="padding:12px;border-radius:10px;border:1px solid rgba(255,255,255,.04);background:transparent;color:var(--txt)">
          <input class="card" name="subject" placeholder="Subject" required style="padding:12px;border-radius:10px;border:1px solid rgba(255,255,255,.04);background:transparent;color:var(--txt)">
          <textarea class="card" name="message" placeholder="Your message" rows="4" required style="grid-column:1/-1;padding:12px;border-radius:10px;border:1px solid rgba(255,255,255,.04);background:transparent;color:var(--txt)"></textarea>
          <button class="btn" type="submit">Send Message</button>
          <small id="formNote" style="align-self:center" class="muted">Opens your email app (no server needed).</small>
        </form>
      </div>

      <div class="card" style="padding:12px">
        <iframe class="map" loading="lazy" allowfullscreen
          referrerpolicy="no-referrer-when-downgrade"
          src="https://www.google.com/maps?q=Kerala&output=embed"
          title="Map (approx)"></iframe>
      </div>
    </div>
  </section>

  <!-- Donate / Support CTA -->
  <section>
    <div class="container card" style="padding:16px;display:flex;flex-wrap:wrap;align-items:center;justify-content:space-between;gap:12px">
      <div>
        <h3 style="margin:0 0 6px;font-family:'Playfair Display',serif">Support AJP</h3>
        <p class="muted" style="margin:0">Your help fuels our outreach — food drives, clothing, and mental care programmes.</p>
      </div>
      <div style="display:flex;gap:10px;flex-wrap:wrap">
        <a class="btn" href="mailto:steveshine999@gmail.com" style="background:linear-gradient(90deg,var(--accent-1),var(--accent-2));border-color:transparent">Contact to Donate</a>
        <a class="btn" href="#contact">Volunteer</a>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer>
    <div class="container" style="display:flex;gap:12px;flex-wrap:wrap;align-items:center;justify-content:space-between">
      <div>© <span id="year"></span> AJP • All rights reserved</div>
      <div class="muted" style="display:flex;gap:12px;align-items:center;flex-wrap:wrap">
        <span>Website made by <strong>Steve Shine</strong></span>
        <span aria-hidden>•</span>
        <a href="mailto:steveshine999@gmail.com">steveshine999@gmail.com</a>
        <span aria-hidden>•</span>
        <a href="tel:+918921370655">+91 8921370655</a>
      </div>
    </div>
  </footer>

  <!-- Lightbox Modal -->
  <dialog id="lightbox" style="border:none;border-radius:12px;padding:0;background:#07060a;max-width:min(92vw,1000px)">
    <img id="lightImg" alt="Expanded image" style="width:100%;height:auto;border-radius:12px;display:block"/>
    <form method="dialog" style="position:absolute;top:8px;right:8px">
      <button class="btn" aria-label="Close">Close ✕</button>
    </form>
  </dialog>

  <script>
    // ---------- Mobile menu toggle ----------
    const menuBtn = document.getElementById('menuBtn');
    menuBtn?.addEventListener('click', () => {
      const nav = document.querySelector('.links');
      nav.style.display = nav.style.display === 'flex' ? 'none' : 'flex';
    });

    // ---------- Lightbox ----------
    const dlg = document.getElementById('lightbox');
    const lightImg = document.getElementById('lightImg');
    function openLightbox(src, alt){ lightImg.src = src; lightImg.alt = alt || 'Image'; dlg.showModal(); }
    document.getElementById('galleryGrid').addEventListener('click', (e)=>{
      const t = e.target;
      if(t.tagName === 'IMG') openLightbox(t.src, t.alt);
    });

    // ---------- Gallery uploads (localStorage) ----------
    const galleryInput = document.getElementById('galleryInput');
    const addToGalleryBtn = document.getElementById('addToGallery');
    const galleryGrid = document.getElementById('galleryGrid');
    const GALLERY_KEY = 'ajp_gallery_v1';

    function loadGallery(){
      try{
        const saved = JSON.parse(localStorage.getItem(GALLERY_KEY)||'[]');
        for(const url of saved){
          const img = document.createElement('img');
          img.src = url; img.alt = 'Uploaded photo';
          img.dataset.origin = 'local';
          galleryGrid.appendChild(img);
        }
      }catch(err){ console.warn('Gallery load error', err); }
    }

    function saveGallery(){
      const urls = [...galleryGrid.querySelectorAll('img')]
        .filter(img => img.dataset.origin === 'local')
        .map(img => img.src);
      localStorage.setItem(GALLERY_KEY, JSON.stringify(urls));
    }

    addToGalleryBtn.addEventListener('click', async ()=>{
      const files = [...(galleryInput.files||[])];
      if(!files.length) return alert('Please choose one or more images.');
      for(const f of files){
        if(!f.type.startsWith('image/')) continue;
        const url = await fileToDataURL(f);
        const img = document.createElement('img');
        img.src = url; img.alt = f.name; img.dataset.origin = 'local';
        galleryGrid.appendChild(img);
      }
      saveGallery();
      galleryInput.value = '';
      window.scrollTo({top: galleryGrid.offsetTop - 80, behavior:'smooth'});
    });

    function fileToDataURL(file){
      return new Promise((res, rej)=>{
        const r = new FileReader();
        r.onload = ()=>res(r.result); r.onerror = rej; r.readAsDataURL(file);
      });
    }

    // ---------- News posts (localStorage) ----------
    const NEWS_KEY = 'ajp_news_v1';
    const newsForm = document.getElementById('newsForm');
    const newsFeed = document.getElementById('newsFeed');
    const clearNewsBtn = document.getElementById('clearNews');
    const latestNewsPeek = document.getElementById('latestNewsPeek');

    function seedNewsIfEmpty(items){
      if(items.length === 0){
        // Seed with the four news items requested (use explicit dates)
        const posts = [
          {
            id: crypto.randomUUID ? crypto.randomUUID() : String(Date.now()+1),
            title: "Leader Participates — School Election",
            body: "Our dearest leader went for participating in school election. (Poster attached)",
            author: "AJP Office",
            ts: new Date('2025-08-07T10:00:00').getTime(),
            image: "https://cdn.discordapp.com/attachments/1361326986131149063/1409150870922203278/poster.jpg?ex=68ac5584&is=68ab0404&hm=7b9fd4c97f0315627acb5af602c6d14fbf1b4d9ab3f4c6d502e5594fe95f2be3"
          },
          {
            id: crypto.randomUUID ? crypto.randomUUID() : String(Date.now()+2),
            title: "Our Leader Has No Opponents — AJP",
            body: "Everyone fears the Beard — AJP: He Is The King.",
            author: "AJP Office",
            ts: new Date('2025-08-10T10:00:00').getTime()
          },
          {
            id: crypto.randomUUID ? crypto.randomUUID() : String(Date.now()+3),
            title: "Leader Selected — Official",
            body: "Our Leader Has Been Selected As Leader.",
            author: "AJP Office",
            ts: new Date('2025-08-14T10:00:00').getTime()
          },
          {
            id: crypto.randomUUID ? crypto.randomUUID() : String(Date.now()+4),
            title: "96 Meals Distributed",
            body: "Our leader gave 96 food packets to poor people on the roadside.",
            author: "AJP Outreach",
            ts: new Date('2025-08-18T10:00:00').getTime()
          }
        ];
        localStorage.setItem(NEWS_KEY, JSON.stringify(posts));
        return posts;
      }
      return items;
    }

    function loadNews(){
      let items = [];
      try{ items = JSON.parse(localStorage.getItem(NEWS_KEY)||'[]'); }catch(err){ items = []; }
      items = seedNewsIfEmpty(items);
      renderNews(items);
    }

    function renderNews(items){
      // newest first
      items.sort((a,b)=>b.ts - a.ts);
      newsFeed.innerHTML = '';
      for(const post of items){
        const card = document.createElement('article');
        card.className = 'post card';
        card.style.padding = '12px';
        card.innerHTML = `
          <h4>${escapeHTML(post.title)}</h4>
          <time>${new Date(post.ts).toLocaleString()}</time>
          ${post.image ? `<div style="margin:10px 0"><img src="${post.image}" alt="news image" style="width:100%;border-radius:8px;max-height:260px;object-fit:cover"></div>` : ''}
          <p class="muted" style="margin:6px 0 0">${escapeHTML(post.body)}</p>
          <div class="post-meta muted">
            <span>— ${escapeHTML(post.author||'AJP')}</span>
            <div style="margin-left:auto;display:flex;gap:8px">
              <button class="btn" data-del="${post.id}" title="Delete this post" style="padding:6px 10px;font-weight:600">Delete</button>
              <button class="btn" data-share="${post.id}" title="Share (copy link)" style="padding:6px 10px;font-weight:600">Copy Text</button>
            </div>
          </div>
        `;
        newsFeed.appendChild(card);
      }

      // Latest news peek in hero
      if(items[0]){
        latestNewsPeek.innerHTML = `Latest: <strong>${escapeHTML(items[0].title)}</strong> — ${escapeHTML(items[0].body)}`;
      }
    }

    newsFeed.addEventListener('click',(e)=>{
      const btnDel = e.target.closest('button[data-del]');
      const btnShare = e.target.closest('button[data-share]');
      if(btnDel){
        const id = btnDel.getAttribute('data-del');
        let items = JSON.parse(localStorage.getItem(NEWS_KEY)||'[]');
        items = items.filter(x=>x.id !== id);
        localStorage.setItem(NEWS_KEY, JSON.stringify(items));
        renderNews(items);
        return;
      }
      if(btnShare){
        const id = btnShare.getAttribute('data-share');
        const items = JSON.parse(localStorage.getItem(NEWS_KEY)||'[]');
        const post = items.find(x=>x.id===id);
        if(post){
          const text = `${post.title}\n\n${post.body}\n\n— ${post.author||'AJP'}`;
          navigator.clipboard?.writeText(text).then(()=> alert('Post text copied to clipboard'), ()=> alert('Copy failed'));
        }
      }
    });

    newsForm.addEventListener('submit',(e)=>{
      e.preventDefault();
      const fd = new FormData(newsForm);
      const title = (fd.get('title')||'').toString().trim();
      const body = (fd.get('body')||'').toString().trim();
      const author = (fd.get('author')||'').toString().trim();
      if(!title || !body) return alert('Please fill in title and body.');
      const post = { id: crypto.randomUUID ? crypto.randomUUID() : String(Date.now()), title, body, author, ts: Date.now() };
      const items = JSON.parse(localStorage.getItem(NEWS_KEY)||'[]');
      items.push(post);
      localStorage.setItem(NEWS_KEY, JSON.stringify(items));
      newsForm.reset();
      renderNews(items);
      window.location.hash = '#news';
    });

    clearNewsBtn.addEventListener('click',()=>{
      if(confirm('Delete all saved news posts from this browser?')){
        localStorage.removeItem(NEWS_KEY); loadNews();
      }
    });

    function escapeHTML(str){
      return String(str).replace(/[&<>"]/g, s => ({'&':'&amp;','<':'&lt;','>':'&gt;','"':'&quot;'}[s]));
    }

    // ---------- Contact form (mailto) ----------
    const form = document.getElementById('msgForm');
    form.addEventListener('submit', (e) => {
      e.preventDefault();
      const data = Object.fromEntries(new FormData(form));
      const body = encodeURIComponent(
        `Name: ${data.name}\nEmail: ${data.email}\nPhone: ${data.phone||''}\n\n${data.message}`
      );
      const subject = encodeURIComponent(data.subject || 'Volunteer enquiry — AJP');
      window.location.href = `mailto:steveshine999@gmail.com?subject=${subject}&body=${body}`;
    });

    // ---------- Footer year ----------
    document.getElementById('year').textContent = new Date().getFullYear();

    // ---------- Init ----------
    loadGallery();
    loadNews();
  </script>
</body>
</html>
