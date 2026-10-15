<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="Portofolio Syaly Darma Prayoga di bidang teknologi informasi, cyber security, networking, dan teknik.">
  <meta name="theme-color" content="#0b1220">
  <title>Syaly Darma Prayoga | Portofolio</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&display=swap" rel="stylesheet">
  <style>
    :root {
      --bg: #0b1220;
      --surface: #111c2e;
      --surface-light: #17243a;
      --text: #edf3fc;
      --muted: #aab8cc;
      --accent: #60a5fa;
      --accent-strong: #3b82f6;
      --border: rgba(180, 200, 230, .15);
      --radius: 18px;
      --shadow: 0 18px 45px rgba(0, 0, 0, .22);
      --content-width: 1120px;
    }
    * { box-sizing: border-box; }
    html { scroll-behavior: smooth; scroll-padding-top: 88px; }
    body {
      margin: 0;
      font-family: "Inter", Arial, sans-serif;
      background: var(--bg);
      color: var(--text);
      line-height: 1.7;
    }
    img { display: block; max-width: 100%; }
    a { color: inherit; text-decoration: none; }
    button { font: inherit; }
    .container { width: min(var(--content-width), calc(100% - 40px)); margin-inline: auto; }
    .site-header {
      position: sticky; top: 0; z-index: 100;
      background: rgba(11, 18, 32, .9);
      border-bottom: 1px solid var(--border);
      backdrop-filter: blur(16px);
    }
    .nav { min-height: 76px; display: flex; align-items: center; justify-content: space-between; gap: 24px; }
    .brand { font-weight: 800; letter-spacing: -.04em; font-size: 1.08rem; }
    .brand span { color: var(--accent); }
    .nav-links { display: flex; align-items: center; gap: 28px; padding: 0; margin: 0; list-style: none; }
    .nav-links a { color: var(--muted); font-size: .92rem; transition: color .2s ease; }
    .nav-links a:hover, .nav-links a:focus-visible { color: var(--accent); }
    .menu-toggle { display: none; border: 1px solid var(--border); color: var(--text); background: var(--surface); border-radius: 10px; padding: 8px 12px; cursor: pointer; }
    .hero {
      position: relative; overflow: hidden; min-height: 590px; display: grid; align-items: center;
      background: radial-gradient(ellipse at 80% 20%, rgba(59,130,246,.2), transparent 42%),
                  radial-gradient(ellipse at 10% 90%, rgba(14,165,233,.12), transparent 38%), var(--bg);
    }
    .hero::after { content: ""; position: absolute; inset: 0; pointer-events: none; background-image: linear-gradient(rgba(255,255,255,.025) 1px, transparent 1px), linear-gradient(90deg, rgba(255,255,255,.025) 1px, transparent 1px); background-size: 42px 42px; mask-image: linear-gradient(to bottom, black, transparent); }
    .hero-content { position: relative; z-index: 1; padding-block: 100px 90px; max-width: var(--content-width); }
    .eyebrow { margin: 0 0 12px; color: var(--accent); font-size: .76rem; font-weight: 800; letter-spacing: .18em; text-transform: uppercase; }
    h1, h2, h3, p { margin-top: 0; }
    h1 { max-width: 850px; margin-bottom: 18px; font-size: clamp(2.5rem, 6vw, 4.7rem); line-height: 1.1; letter-spacing: -.065em; }
    h1 span { color: var(--accent); }
    .hero-subtitle { color: #d7e4f5; font-size: clamp(1rem, 2vw, 1.2rem); font-weight: 600; }
    .hero-copy { max-width: 670px; color: var(--muted); font-size: 1.04rem; }
    .hero-actions { display: flex; flex-wrap: wrap; gap: 12px; margin-top: 30px; }
    .button { display: inline-flex; justify-content: center; align-items: center; gap: 8px; min-height: 46px; padding: 11px 19px; border: 1px solid transparent; border-radius: 11px; font-size: .92rem; font-weight: 700; transition: transform .2s ease, background .2s ease; }
    .button:hover { transform: translateY(-2px); }
    .button-primary { background: var(--accent-strong); color: white; }
    .button-primary:hover { background: #2563eb; }
    .button-outline { border-color: var(--border); background: rgba(255,255,255,.025); }
    .button-outline:hover { background: var(--surface-light); }
    .section { padding-block: 88px; }
    .section-muted { background: #0e1727; border-block: 1px solid rgba(180,200,230,.07); }
    .section-heading { max-width: 680px; margin: 0 auto 42px; text-align: center; }
    .section-heading h2 { margin-bottom: 10px; font-size: clamp(2rem, 4vw, 2.8rem); line-height: 1.2; letter-spacing: -.045em; }
    .section-heading > p:last-child { margin-bottom: 0; color: var(--muted); }
    .about-grid { display: grid; grid-template-columns: minmax(250px, .8fr) 1.2fr; gap: 54px; align-items: center; }
    .about-photo { overflow: hidden; border: 1px solid var(--border); border-radius: var(--radius); background: var(--surface); box-shadow: var(--shadow); }
    .about-photo img { width: 100%; height: 430px; object-fit: cover; object-position: center; }
    .about-text h3 { margin-bottom: 14px; font-size: 1.45rem; }
    .about-text > p { color: var(--muted); }
    .info-grid { display: grid; grid-template-columns: repeat(2, minmax(0, 1fr)); gap: 18px; margin: 28px 0; }
    .info-item { padding: 14px 16px; background: var(--surface); border: 1px solid var(--border); border-radius: 12px; }
    .info-item small { display: block; margin-bottom: 4px; color: var(--muted); }
    .info-item strong { font-size: .94rem; overflow-wrap: anywhere; }
    .cards { display: grid; gap: 20px; }
    .three-cols { grid-template-columns: repeat(3, minmax(0, 1fr)); }
    .skill-card, .project-card, .contact-card { border: 1px solid var(--border); border-radius: var(--radius); background: var(--surface); }
    .skill-card { padding: 28px; transition: transform .2s ease, border-color .2s ease; }
    .skill-card:hover, .project-card:hover { transform: translateY(-4px); border-color: rgba(96,165,250,.5); }
    .skill-icon { display: grid; place-items: center; width: 48px; height: 48px; margin-bottom: 20px; border-radius: 14px; color: var(--accent); background: rgba(96,165,250,.12); font-size: 1.5rem; }
    .skill-card h3, .project-info h3 { margin-bottom: 10px; font-size: 1.15rem; }
    .skill-card p, .project-info p { margin-bottom: 0; color: var(--muted); font-size: .94rem; }
    .project-filters { display: flex; flex-wrap: wrap; justify-content: center; gap: 10px; margin: -12px 0 32px; }
    .filter { padding: 9px 15px; border: 1px solid var(--border); border-radius: 999px; color: var(--muted); background: transparent; cursor: pointer; font-size: .88rem; }
    .filter:hover, .filter.active { color: white; border-color: var(--accent-strong); background: var(--accent-strong); }
    .project-grid { display: grid; grid-template-columns: repeat(3, minmax(0, 1fr)); gap: 22px; align-items: stretch; }
    .project-card { overflow: hidden; padding: 14px; transition: transform .2s ease, border-color .2s ease; }
    .project-card[hidden] { display: none; }
    .project-card img { width: 100%; height: 205px; object-fit: cover; border-radius: 12px; background: var(--surface-light); }
    .project-info { padding: 18px 6px 8px; }
    .project-info small { display: inline-block; margin-bottom: 9px; color: var(--accent); font-size: .7rem; font-weight: 800; letter-spacing: .12em; }
    .project-info p { min-height: 96px; }
    .project-info a { display: inline-block; margin-top: 18px; color: var(--accent); font-size: .9rem; font-weight: 700; }
    .project-info a:hover { color: white; }
    .stats { padding-block: 38px; background: #101d31; border-block: 1px solid var(--border); }
    .stats-grid { display: grid; grid-template-columns: repeat(3, 1fr); gap: 24px; text-align: center; }
    .stats-grid strong { display: block; color: var(--accent); font-size: 1.8rem; letter-spacing: -.04em; }
    .stats-grid span { color: var(--muted); font-size: .9rem; }
    .contact-wrap { display: grid; grid-template-columns: .9fr 1.1fr; gap: 50px; align-items: start; }
    .align-left { margin: 0; text-align: left; }
    .contact-card { padding: 26px; }
    .contact-card p { display: grid; grid-template-columns: 110px minmax(0, 1fr); gap: 14px; margin-bottom: 0; padding: 15px 0; border-bottom: 1px solid var(--border); }
    .contact-card p:first-child { padding-top: 0; }
    .contact-card p:last-child { padding-bottom: 0; border-bottom: 0; }
    .contact-card span { color: var(--muted); }
    .contact-card a { color: var(--accent); overflow-wrap: anywhere; }
    .contact-card a:hover { text-decoration: underline; }
    .footer { padding-block: 25px; border-top: 1px solid var(--border); }
    .footer-inner { display: flex; flex-wrap: wrap; align-items: center; justify-content: space-between; gap: 14px; }
    .footer p { margin: 0; color: var(--muted); font-size: .85rem; }
    .footer-inner > a:last-child { color: var(--muted); font-size: .85rem; }
    .footer-inner > a:last-child:hover { color: var(--accent); }
    :focus-visible { outline: 3px solid var(--accent); outline-offset: 3px; }
    @media (max-width: 850px) {
      .about-grid, .contact-wrap { grid-template-columns: 1fr; gap: 32px; }
      .about-photo { max-width: 480px; margin-inline: auto; width: 100%; }
      .about-photo img { height: 400px; }
      .three-cols, .project-grid { grid-template-columns: repeat(2, minmax(0, 1fr)); }
      .contact-wrap .section-heading { margin-bottom: 0; }
    }
    @media (max-width: 620px) {
      .container { width: min(var(--content-width), calc(100% - 30px)); }
      .nav { min-height: 68px; }
      .menu-toggle { display: inline-flex; }
      .nav-links { display: none; position: absolute; top: 68px; left: 0; right: 0; padding: 16px 20px 20px; background: #0b1220; border-bottom: 1px solid var(--border); flex-direction: column; align-items: stretch; gap: 0; }
      .nav-links.open { display: flex; }
      .nav-links a { display: block; padding: 11px 5px; }
      .hero { min-height: 540px; }
      .hero-content { padding-block: 80px; }
      .section { padding-block: 66px; }
      .section-heading { margin-bottom: 30px; }
      .three-cols, .project-grid, .info-grid { grid-template-columns: 1fr; }
      .project-info p { min-height: 0; }
      .stats-grid { grid-template-columns: 1fr; gap: 22px; }
      .contact-card { padding: 20px; }
      .contact-card p { grid-template-columns: 1fr; gap: 3px; }
      .footer-inner { flex-direction: column; align-items: flex-start; }
    }
    @media (prefers-reduced-motion: reduce) {
      html { scroll-behavior: auto; }
      *, *::before, *::after { transition-duration: .01ms !important; animation-duration: .01ms !important; }
    }
  </style>
</head>
<body>
  <header class="site-header">
    <nav class="nav container" aria-label="Navigasi utama">
      <a class="brand" href="#home" aria-label="Syaly Darma Prayoga - beranda">YOGA BUKAN AGOY</a>
      <button class="menu-toggle" type="button" aria-label="Buka navigasi" aria-expanded="false" aria-controls="nav-links">☰</button>
      <ul class="nav-links" id="nav-links">
        <li><a href="#home">Beranda</a></li>
        <li><a href="#about">Tentang</a></li>
        <li><a href="#services">Keahlian</a></li>
        <li><a href="#portfolio">Proyek</a></li>
        <li><a href="#contact">Kontak</a></li>
      </ul>
    </nav>
  </header>

  <main>
    <section class="hero" id="home">
      <div class="container hero-content">
        <p class="eyebrow">Portofolio Profesional</p>
        <h1>Halo, saya <span>Syaly Darma Prayoga</span></h1>
        <p class="hero-subtitle">IT Enthusiast · Cyber Security · Networking · MEP &amp; Electrical</p>
        <p class="hero-copy">Menggabungkan minat di bidang teknologi informasi dengan pengalaman teknis untuk membantu membangun solusi yang aman, efektif, dan bermanfaat.</p>
        <div class="hero-actions">
          <a class="button button-primary" href="#portfolio">Lihat Proyek <span aria-hidden="true">↗</span></a>
          <a class="button button-outline" href="#contact">Hubungi Saya</a>
        </div>
      </div>
    </section>

    <section class="section container about" id="about">
      <div class="section-heading">
        <p class="eyebrow">Kenali Saya</p>
        <h2>Tentang Saya</h2>
        <p>Saya adalah seorang mahasiswa Teknik Informatika yang memiliki minat pada bidang cyber security dan juga memiliki pengalaman di bidang mechanical electrical dan plumbing yang ingin terus mengembangkan skill dan pengetahuan</p>
      </div>
      <div class="about-grid">
        <div class="about-photo">
          <img src="foto full body.jpeg" alt="Foto Syaly Darma Prayoga" loading="lazy">
        </div>
        <div class="about-text">
          <h3>IT &amp; Technical Enthusiast</h3>
          <p>Saya memiliki minat pada teknologi informasi, khususnya Cyber Security dan Networking, serta pengalaman praktik di bidang mekanikal, elektrikal, cctv , dan sistem pendingin. Saya senang mempelajari hal baru, menganalisis masalah, dan mencari solusi yang dapat diterapkan secara langsung.</p>
          <div class="info-grid">
            <div class="info-item"><small>Nama</small><strong>Syaly Darma Prayoga</strong></div>
            <div class="info-item"><small>Fokus</small><strong>IT &amp; Teknik</strong></div>
            <div class="info-item"><small>Bidang</small><strong>Cyber Security &amp; MEP</strong></div>
            <div class="info-item"><small>Domisili</small><strong>Depok, Jawa Barat</strong></div>
          </div>
          <a class="button button-primary" href="#contact">Diskusi Proyek</a>
        </div>
      </div>
    </section>

    <section class="section section-muted" id="services">
      <div class="container">
        <div class="section-heading">
          <p class="eyebrow">Bidang yang Ditekuni</p>
          <h2>Keahlian &amp; Minat</h2>
          <p>Bidang yang terus saya kembangkan melalui pembelajaran dan pengalaman praktik.</p>
        </div>
        <div class="cards three-cols">
          <article class="skill-card">
            <div class="skill-icon" aria-hidden="true">⌘</div>
            <h3>Cyber Security</h3>
            <p>Pemahaman dasar keamanan sistem, pengenalan kerentanan, serta pengujian keamanan secara etis pada sistem yang memiliki izin, dan melaporkan hasil pengujian.</p>
          </article>
          <article class="skill-card">
            <div class="skill-icon" aria-hidden="true">⌁</div>
            <h3>Networking &amp; IT</h3>
            <p>Dasar jaringan komputer, troubleshooting, konfigurasi jaringan, serta pemahaman perangkat dan sistem komputer.</p>
          </article>
          <article class="skill-card">
            <div class="skill-icon" aria-hidden="true">ϟ</div>
            <h3>MEP &amp; Electrical</h3>
            <p>Pengalaman praktik instalasi dan troubleshooting kelistrikan, mekanikal, plumbing, cctv, serta sistem pendingin.</p>
          </article>
        </div>
      </div>
    </section>

    <section class="section container" id="portfolio">
      <div class="section-heading">
        <p class="eyebrow">Evidence</p>
        <h2>KEAHLIAN SAYA</h2>
        <p>Beberapa bidang proyek dan praktik yang relevan dengan minat serta pengalaman saya.</p>
      </div>
      <div class="project-filters" role="group" aria-label="Filter proyek">
        <button class="filter active" type="button" data-filter="all" aria-pressed="true">Semua</button>
        <button class="filter" type="button" data-filter="security" aria-pressed="false">Cyber Security</button>
        <button class="filter" type="button" data-filter="network" aria-pressed="false">Networking</button>
        <button class="filter" type="button" data-filter="technical" aria-pressed="false">Teknik</button>
      </div>
      <div class="project-grid">
        <article class="project-card" data-category="security">
          <img src="testing.png" alt="Dokumentasi pengujian keamanan siber" loading="lazy">
          <div class="project-info">
            <small>CYBER SECURITY</small>
            <h3>Penetration Testing</h3>
            <p>Laporan hasil pengujian, tujuan pengujian, metode, dan temuan keamanan pada website atau aplikasi yang diizinkan.</p>
            <a href="#contact">Tanyakan proyek <span aria-hidden="true">↗</span></a>
          </div>
        </article>
        <article class="project-card" data-category="network">
          <img src="topologi.jpg" alt="Ilustrasi topologi jaringan komputer" loading="lazy">
          <div class="project-info">
            <small>NETWORKING</small>
            <h3>Perancangan Jaringan</h3>
            <p>Perencanaan topologi jaringan, pembagian alamat IP, konfigurasi perangkat, dan pengujian konektivitas jaringan.</p>
            <a href="#contact">Tanyakan proyek <span aria-hidden="true">↗</span></a>
          </div>
        </article>
        <article class="project-card" data-category="technical">
          <img src="gambarkerja.jpeg" alt="Dokumentasi pekerjaan instalasi dan troubleshooting teknis" loading="lazy">
          <div class="project-info">
            <small>MEP / ELECTRICAL</small>
            <h3>Instalasi & Troubleshooting</h3>
            <p>Berpengalaman dalam pekerjaan MEP yang mencakup mekanikal, elektrikal, plumbing, cctv. Terbiasa melakukan instalasi, pengecekan, perawatan rutin, dan troubleshooting untuk memastikan peralatan serta sistem tetap berfungsi dengan baik, aman, dan optimal.</p>
            <a href="#contact">Tanyakan proyek <span aria-hidden="true">↗</span></a>
          </div>
        </article>
      </div>
    </section>

    <section class="stats" aria-label="Ringkasan portofolio">
      <div class="container stats-grid">
        <div><strong>IT</strong><span>Teknologi Informasi</span></div>
        <div><strong>MEP</strong><span>Pengalaman Teknis</span></div>
        <div><strong>∞</strong><span>Semangat Belajar</span></div>
      </div>
    </section>
  <section class="section section-muted" id="contact">
      <div class="container contact-wrap">
        <div class="section-heading align-">
          <p class="eyebrow">Mari Terhubung</p>
          <h2>Hubungi Saya</h2>
          <p>Terbuka untuk diskusi, kolaborasi, dan kesempatan kerja yang relevan.</p>
        </div>
        <div class="contact-card">
          <p><span>Email</span><a href="mailto:syalydarmaprayoga19@gmail.com">syalydarmaprayoga19@gmail.com</a></p>
          <p><span>LinkedIn</span><a href="https://www.linkedin.com/in/drmapryga/" target="_blank" rel="noopener noreferrer">linkedin.com/in/drmapryga</a></p>
          <p><span>Instagram</span><a href="https://www.instagram.com/drmapryga_/" target="_blank" rel="noopener noreferrer">instagram.com/drmapryga_</a></p>
          <p><span>Domisili</span><strong>Depok, Jawa Barat, Indonesia</strong></p>
        </div>
      </div>
    </section>
  </main>

  <footer class="footer">
    <div class="container footer-inner">
      <a class="brand" href="#home">Thanks Bray Salam Kenal...</span></a>
      <p>© <span id="year"></span> Syaly Darma Prayoga</p>
      <a href="#home">Kembali ke atas ↑</a>
    </div>
  </footer>

  <script>
    // Tahun pada footer diperbarui otomatis.
    document.getElementById("year").textContent = new Date().getFullYear();

    // Navigasi responsif untuk perangkat mobile.
    const menuToggle = document.querySelector(".menu-toggle");
    const navLinks = document.querySelector(".nav-links");

    menuToggle.addEventListener("click", () => {
      const isOpen = navLinks.classList.toggle("open");
      menuToggle.setAttribute("aria-expanded", String(isOpen));
      menuToggle.setAttribute("aria-label", isOpen ? "Tutup navigasi" : "Buka navigasi");
      menuToggle.textContent = isOpen ? "×" : "☰";
    });

    navLinks.querySelectorAll("a").forEach((link) => {
      link.addEventListener("click", () => {
        navLinks.classList.remove("open");
        menuToggle.setAttribute("aria-expanded", "false");
        menuToggle.setAttribute("aria-label", "Buka navigasi");
        menuToggle.textContent = "☰";
      });
    });

    // Filter proyek berdasarkan kategori.
    const filterButtons = document.querySelectorAll(".filter");
    const projectCards = document.querySelectorAll(".project-card");

    filterButtons.forEach((button) => {
      button.addEventListener("click", () => {
        const selectedFilter = button.dataset.filter;

        filterButtons.forEach((item) => {
          const isActive = item === button;
          item.classList.toggle("active", isActive);
          item.setAttribute("aria-pressed", String(isActive));
        });

        projectCards.forEach((card) => {
          card.hidden = selectedFilter !== "all" && card.dataset.category !== selectedFilter;
        });
      });
    });
  </script>
</body>
</html>
