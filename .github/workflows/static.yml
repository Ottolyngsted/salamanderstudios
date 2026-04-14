<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Salamander Studios</title>
  <style>
  :root {
    --bg: #8EA08B;
    --bg-deep: #758570;
    --bg-soft: #DADADA;
    --panel: rgba(122, 110, 96, 0.84);
    --panel-strong: rgba(98, 87, 74, 0.92);
    --text: #ffffff;
    --muted: #ffffff;
    --green: #ffffff;
    --green-soft: #ffffff;
    --green-deep: #ffffff;
    --blue: #ffffff;
    --slate: #6C7A8E;
    --red: #FF5C5C;
    --gold: #FFD700;
    --border: rgba(247, 241, 232, 0.14);
    --shadow: 0 18px 34px rgba(74, 60, 46, 0.18);
    --radius: 6px;
    --max-width: 1180px;
    --accent: #ffffff;
  }

  * {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
  }

  html {
    scroll-behavior: smooth;
  }

  body {
    font-family: Arial, Helvetica, sans-serif;
    color: var(--text);
    min-height: 100vh;
    line-height: 1.6;
    position: relative;
    overflow-x: hidden;
    background: #000;
  }

  .background-video {
    position: fixed;
    inset: 0;
    width: 100%;
    height: 100%;
    object-fit: cover;
    z-index: -3;
    pointer-events: none;
  }

  body::before,
  body::after {
    content: "";
    position: fixed;
    inset: 0;
    pointer-events: none;
  }

  body::before {
    z-index: -2;
    background: rgba(0, 0, 0, 0.42);
  }

  body::after {
    z-index: -1;
    background:
      radial-gradient(circle at 15% 20%, rgba(255,255,255,0.05), transparent 18%),
      radial-gradient(circle at 85% 14%, rgba(255,255,255,0.04), transparent 16%),
      radial-gradient(circle at 50% 80%, rgba(255,255,255,0.03), transparent 20%);
    filter: blur(30px);
    opacity: 0.4;
  }

  a {
    color: inherit;
    text-decoration: none;
  }

  .site-header,
  main,
  .site-footer {
    position: relative;
    z-index: 1;
  }

  .site-header {
    position: sticky;
    top: 0;
    z-index: 100;
    backdrop-filter: blur(18px);
    -webkit-backdrop-filter: blur(18px);
    background: transparent;
    border-bottom: 1px solid rgba(247, 244, 234, 0.14);
  }

  .nav {
    max-width: var(--max-width);
    margin: 0 auto;
    padding: 18px 24px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 20px;
  }

  .brand {
    font-size: 1.15rem;
    font-weight: bold;
    letter-spacing: 0.04em;
  }

  .brand span {
    color: var(--accent);
  }

  .nav-links {
    display: flex;
    gap: 14px;
    flex-wrap: wrap;
  }

  .nav-link,
  .button,
  .card-link,
  .site-card {
    transition: 0.3s ease;
  }

  .nav-link {
    padding: 10px 14px;
    border-radius: 4px;
    color: var(--text);
    border: 1px solid transparent;
    background: rgba(247, 244, 234, 0.05);
    backdrop-filter: blur(4px);
    -webkit-backdrop-filter: blur(4px);
    white-space: nowrap;
  }

  .nav-link:hover,
  .nav-link.active {
    color: #4b3f34;
    border-color: rgba(247, 244, 234, 0.18);
    background: linear-gradient(135deg, rgba(247, 244, 234, 0.92), rgba(183, 200, 164, 0.74));
  }

  main {
    max-width: var(--max-width);
    margin: 0 auto;
    padding: 36px 24px 64px;
  }

  .page {
    display: none;
    animation: fadeIn 0.5s ease;
  }

  .page.active {
    display: block;
  }

  @keyframes fadeIn {
    from {
      opacity: 1;
      transform: translateY(0);
    }
    to {
      opacity: 1;
      transform: translateY(0);
    }
  }

  .hero {
    min-height: 72vh;
    display: grid;
    grid-template-columns: 1.1fr 0.9fr;
    gap: 28px;
    align-items: center;
  }

  .hero-copy,
  .hero-panel,
  .content-panel,
  .info-card,
  .feature-card,
  .project-card,
  .site-card,
  .card-link {
    background: transparent;
    border: 0 solid rgba(247, 241, 232, 0.14);
    border-radius: var(--radius);
    box-shadow:
      inset 0 1px 0 rgba(255,255,255,0.20),
      inset 0 -1px 0 rgba(255,255,255,0.05),
      var(--shadow);
    backdrop-filter: blur(14px) saturate(1.06);
    -webkit-backdrop-filter: blur(100px) saturate(1.06);
    position: relative;
    overflow: hidden;
    isolation: isolate;
  }

  .hero-copy::after,
  .hero-panel::before,
  .content-panel::before,
  .info-card::before,
  .feature-card::before,
  .project-card::before,
  .site-card::before,
  .card-link::before {
    content: "";
    position: absolute;
    inset: 0;
    background:
      linear-gradient(115deg,
        rgba(255,255,255,0) 16%,
        rgba(255,255,255,0.16) 30%,
        rgba(194,217,204,0.12) 42%,
        rgba(255,255,255,0.05) 56%,
        rgba(255,255,255,0) 72%);
    mix-blend-mode: screen;
    opacity: 0.7;
    pointer-events: none;
    transform: translateX(-4%);
    z-index: 0;
  }

  .hero-copy > *,
  .hero-panel > *,
  .content-panel > *,
  .info-card > *,
  .feature-card > *,
  .project-card > *,
  .site-card > *,
  .card-link > * {
    position: relative;
    z-index: 1;
  }

  .hero-copy {
    padding: 42px;
  }

  .hero-copy::before {
    content: "";
    position: absolute;
    width: 240px;
    height: 240px;
    right: -80px;
    top: -80px;
    border-radius: 50%;
    background: radial-gradient(circle, rgba(247, 244, 234, 0.12), transparent 62%);
    filter: blur(8px);
    pointer-events: none;
    z-index: 0;
  }

  .eyebrow {
    display: inline-block;
    font-size: 0.85rem;
    text-transform: uppercase;
    letter-spacing: 0.14em;
    color: #eef3e7;
    margin-bottom: 16px;
  }

  h1, h2, h3 {
    line-height: 1.1;
  }

  h1 {
    font-size: clamp(2.6rem, 5vw, 5rem);
    margin-bottom: 20px;
    color: var(--accent);
    text-shadow: 0 6px 18px rgba(71, 96, 53, 0.08);
  }

  .hero-copy p,
  .section-intro,
  .site-card p,
  .info-card p,
  .feature-card p,
  .project-card p,
  .project-card li,
  .card-link p {
    color: var(--accent);
    font-size: 1.05rem;
    text-shadow: 0 1px 2px rgba(0, 0, 0, 0.26);
  }

  .hero-copy p,
  .section-intro,
  .site-card p {
    max-width: 62ch;
  }

  .hero-actions {
    display: flex;
    gap: 14px;
    margin-top: 28px;
    flex-wrap: wrap;
  }

  .button {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    min-width: 160px;
    padding: 14px 20px;
    border-radius: 4px;
    border: 1px solid rgba(247, 244, 234, 0.16);
    font-weight: bold;
    cursor: pointer;
    color: var(--accent);
    background:
      linear-gradient(135deg, rgba(255,255,255,0.16), rgba(255,255,255,0.04)),
      url("Button_background.png") center center / cover no-repeat;
    box-shadow:
      inset 0 1px 0 rgba(255, 255, 255, 0.22),
      inset 0 -1px 0 rgba(255, 255, 255, 0.06),
      0 14px 24px rgba(71, 96, 53, 0.14);
    position: relative;
    overflow: hidden;
    isolation: isolate;
    text-shadow: 0 1px 2px rgba(0, 0, 0, 0.28);
    backdrop-filter: blur(4px) saturate(1.08);
    -webkit-backdrop-filter: blur(4px) saturate(1.08);
  }

  .button::before {
    content: "";
    position: absolute;
    inset: 0;
    background:
      linear-gradient(115deg,
        rgba(255,255,255,0) 18%,
        rgba(255,255,255,0.16) 32%,
        rgba(194,217,204,0.12) 42%,
        rgba(255,255,255,0.05) 56%,
        rgba(255,255,255,0) 72%);
    mix-blend-mode: screen;
    opacity: 0.8;
    pointer-events: none;
    transform: translateX(-6%);
  }

  .button::after,
  .content-panel::after,
  .card-link::after,
  .info-card::after,
  .feature-card::after,
  .project-card::after,
  .site-card::after {
    content: "";
    position: absolute;
    inset: 1px;
    border-radius: inherit;
    border: 1px solid rgba(255,255,255,0.10);
    background: linear-gradient(180deg, rgba(255,255,255,0.08), rgba(255,255,255,0));
    pointer-events: none;
  }

  .button.primary {
    border: 1px solid rgba(255, 255, 255, 0.12);
  }

  .button:not(.primary) {
    border: 1px solid rgba(247, 244, 234, 0.14);
  }

  .button:hover,
  .card-link:hover,
  .site-card:hover {
    transform: translateY(-3px);
  }

  .button:hover,
  .card-link:hover,
  .feature-card:hover,
  .project-card:hover,
  .site-card:hover,
  .info-card:hover {
    filter: saturate(1.05) brightness(1.04);
  }

  .button:hover {
    box-shadow:
      inset 0 1px 0 rgba(255, 255, 255, 0.28),
      inset 0 -1px 0 rgba(255, 255, 255, 0.08),
      0 18px 28px rgba(71, 96, 53, 0.18);
  }

  .hero-panel {
    padding: 22px;
    display: grid;
    gap: 18px;
  }

  .hero-panel::after {
    content: "";
    position: absolute;
    left: -40px;
    bottom: -60px;
    width: 220px;
    height: 220px;
    border-radius: 50%;
    background: radial-gradient(circle, rgba(255, 255, 255, 0.10), transparent 66%);
    filter: blur(10px);
    pointer-events: none;
    z-index: 0;
  }

  .info-card,
  .site-card {
    padding: 22px;
  }

  .info-card h3,
  .site-card h3 {
    margin-bottom: 10px;
    font-size: 1.15rem;
  }

  .card-grid,
  .feature-grid,
  .project-grid,
  .site-grid {
    display: grid;
    gap: 20px;
  }

  .card-grid {
    margin-top: 34px;
    grid-template-columns: repeat(3, minmax(0, 1fr));
  }

  .site-grid,
  .feature-grid,
  .project-grid {
    grid-template-columns: repeat(3, minmax(0, 1fr));
    margin-top: 26px;
  }

  .card-link {
    display: block;
    padding: 26px;
    min-height: 220px;
  }

  .card-link h3 {
    font-size: 1.55rem;
    margin-bottom: 14px;
    color: #fff7ef;
  }

  .card-link p {
    max-width: 30ch;
  }

  .card-arrow {
    margin-top: 22px;
    display: inline-block;
    font-weight: bold;
    color: var(--accent);
    text-shadow: 0 1px 2px rgba(0, 0, 0, 0.26);
  }

  .content-panel {
    padding: 42px;
    margin-top: 16px;
  }

  .page-header {
    margin-bottom: 26px;
  }

  .page-header h2 {
    font-size: clamp(2rem, 4vw, 3.4rem);
    margin-bottom: 12px;
    color: var(--accent);
  }

  .feature-card,
  .project-card {
    padding: 24px;
  }

  .feature-card h3,
  .project-card h3,
  .info-card h3,
  .site-card h3 {
    margin-bottom: 12px;
    font-size: 1.2rem;
    color: #fff7ef;
  }

  .project-card ul {
    margin-top: 16px;
    padding-left: 18px;
  }

  .back-link,
  .site-link {
    display: inline-flex;
    align-items: center;
    gap: 8px;
    margin-top: 28px;
    color: #c2d9cc;
    font-weight: bold;
    text-shadow: 0 1px 2px rgba(0, 0, 0, 0.26);
  }

  .site-card:hover .site-link,
  .back-link:hover,
  .card-link:hover .card-arrow {
    color: #e4f2ea;
  }

  .site-footer {
    max-width: var(--max-width);
    margin: 0 auto;
    padding: 0 24px 36px;
    color: #c2d9cc;
    position: relative;
    z-index: 1;
    text-shadow: 0 1px 2px rgba(0, 0, 0, 0.26);
  }

  /* tablet */
  @media (max-width: 960px) {
    .nav {
      padding: 16px 18px;
      align-items: flex-start;
      flex-direction: column;
    }

    .nav-links {
      width: 100%;
      gap: 10px;
      overflow-x: auto;
      flex-wrap: nowrap;
      padding-bottom: 4px;
      scrollbar-width: none;
    }

    .nav-links::-webkit-scrollbar {
      display: none;
    }

    .hero {
      grid-template-columns: 1fr 1fr;
      gap: 18px;
      min-height: auto;
    }

    .hero-copy,
    .content-panel {
      padding: 28px;
    }

    .hero-panel,
    .info-card,
    .feature-card,
    .project-card,
    .site-card,
    .card-link {
      padding: 20px;
    }

    .card-grid,
    .feature-grid,
    .project-grid,
    .site-grid {
      grid-template-columns: repeat(2, minmax(0, 1fr));
      gap: 16px;
    }

    h1 {
      font-size: clamp(2.1rem, 5vw, 3.6rem);
    }

    .page-header h2 {
      font-size: clamp(1.8rem, 4vw, 2.8rem);
    }
  }

  /* mobile */
  @media (max-width: 640px) {
    main {
      padding: 20px 14px 40px;
    }

    .site-footer {
      padding: 0 14px 24px;
    }

    .hero {
      grid-template-columns: 1fr;
      gap: 14px;
    }

    .card-grid,
    .feature-grid,
    .project-grid,
    .site-grid {
      grid-template-columns: 1fr;
      gap: 14px;
    }

    .hero-copy,
    .content-panel,
    .hero-panel,
    .info-card,
    .feature-card,
    .project-card,
    .site-card,
    .card-link {
      padding: 18px;
    }

    .hero-actions {
      flex-direction: column;
      gap: 10px;
    }

    .button {
      width: 100%;
      min-width: 0;
      padding: 13px 16px;
    }

    .card-link {
      min-height: auto;
    }

    .nav-link {
      padding: 9px 12px;
      font-size: 0.95rem;
    }

    .eyebrow {
      font-size: 0.72rem;
      letter-spacing: 0.11em;
      margin-bottom: 10px;
    }

    h1 {
      font-size: clamp(1.9rem, 9vw, 2.8rem);
      margin-bottom: 14px;
    }

    .page-header h2 {
      font-size: clamp(1.5rem, 7vw, 2.2rem);
      margin-bottom: 10px;
    }

    .hero-copy p,
    .section-intro,
    .site-card p,
    .info-card p,
    .feature-card p,
    .project-card p,
    .project-card li,
    .card-link p {
      font-size: 0.98rem;
    }
  }
</style>
</head>
<body>
  <video id="backgroundVideo" class="background-video" autoplay muted loop playsinline>
    <source id="backgroundVideoSource" src="Background_Video2.mp4" type="video/mp4">
    Your browser does not support the video tag.
  </video>

  <header class="site-header">
    <nav class="nav">
      <a href="#home" class="brand nav-trigger" data-page="home">Salamander<span>Studios</span></a>
      <div class="nav-links">
        <a href="#home" class="nav-link nav-trigger active" data-page="home">Home</a>
        <a href="#design-work" class="nav-link nav-trigger" data-page="design-work">Design work</a>
        <a href="#websites" class="nav-link nav-trigger" data-page="websites">Websites</a>
        <a href="#solutions" class="nav-link nav-trigger" data-page="solutions">Solutions</a>
      </div>
    </nav>
  </header>

  <main>
    <section id="home" class="page active">
      <div class="hero">
        <div class="hero-copy">
          <span class="eyebrow">3D, design, websites, and creative solutions</span>
          <h1>Creative work across 3D, design, websites, and visual solutions.</h1>
          <p>
            I do all types of work from setup and website structure to PoS materials, logos, fonts, videos, images, branding, and creative visual concepts. This front page puts the 3D work first and guides visitors into design work, websites, and tailored solutions.
          </p>
          <div class="hero-actions">
            <a href="#design-work" class="button primary nav-trigger" data-page="design-work">Explore work</a>
            <a href="#websites" class="button nav-trigger" data-page="websites">View websites</a>
          </div>
        </div>

        <div class="hero-panel">
          <div class="info-card">
            <h3>Featured 3D work</h3>
            <p>The front page uses the main background video, while Design work switches to the furniture video.</p>
          </div>
          <div class="info-card">
            <h3>Design and furniture</h3>
            <p>The cards and content stay layered on top while each section keeps its own background atmosphere.</p>
          </div>
          <div class="info-card">
            <h3>From idea to delivery</h3>
            <p>I can handle the full process from setup and concept direction to finished websites, visual assets, and presentation.</p>
          </div>
        </div>
      </div>

      <div class="content-panel">
        <div class="page-header">
          <span class="eyebrow">Front page video</span>
          <h2>3D work in motion</h2>
          <p class="section-intro">
            The front page video fills the entire page in the background, stays muted, loops continuously, and changes automatically when visitors enter Design work.
          </p>
        </div>
      </div>

      <div class="card-grid">
        <a href="#design-work" class="card-link nav-trigger" data-page="design-work">
          <h3>Design work</h3>
          <p>Furniture visuals, logos, fonts, PoS materials, campaigns, images, video, and complete visual design.</p>
          <span class="card-arrow">Open page</span>
        </a>

        <a href="#websites" class="card-link nav-trigger" data-page="websites">
          <h3>Websites</h3>
          <p>Live references including Hedestrik.dk, Zeuthenfurniture.dk, and Galleri-zeuthen.dk.</p>
          <span class="card-arrow">Open page</span>
        </a>

        <a href="#solutions" class="card-link nav-trigger" data-page="solutions">
          <h3>Solutions</h3>
          <p>From setup and structure to finished design systems and custom digital presentations.</p>
          <span class="card-arrow">Open page</span>
        </a>
      </div>
    </section>

    <section id="design-work" class="page">
      <div class="content-panel">
        <div class="page-header">
          <span class="eyebrow">Design work</span>
          <h2>Design across furniture, branding, PoS, and visual storytelling</h2>
          <p class="section-intro">
            This page presents the wider design side of the work: visual identity, product presentation, furniture-related visuals, point-of-sale materials, videos, imagery, and creative concepts.
          </p>
        </div>

        <div class="feature-grid">
          <article class="feature-card">
            <h3>Brand identity</h3>
            <p>Logo design, typography, fonts, and visual direction built to give every brand or project a distinct identity.</p>
          </article>
          <article class="feature-card">
            <h3>PoS and campaign material</h3>
            <p>Point-of-sale design, launch materials, signage, product visuals, and assets for physical and digital use.</p>
          </article>
          <article class="feature-card">
            <h3>Images and video</h3>
            <p>Creative production across still imagery, video, motion, and layout presentation that supports the full concept.</p>
          </article>
        </div>

        <a href="#home" class="back-link nav-trigger" data-page="home">Back to front page</a>
      </div>
    </section>

    <section id="websites" class="page">
      <div class="content-panel">
        <div class="page-header">
          <span class="eyebrow">Websites</span>
          <h2>Websites built with structure, design, and clear presentation</h2>
          <p class="section-intro">
            Alongside design work, I also build and shape websites from the initial setup and overall structure to the final visual presentation and content flow.
          </p>
        </div>

        <div class="site-grid">
          <a class="site-card" href="https://hedestrik.dk" target="_blank" rel="noopener noreferrer">
            <h3>Hedestrik.dk</h3>
            <p>A live website reference showing practical setup, design presentation, and business-focused web structure.</p>
            <span class="site-link">Visit site</span>
          </a>

          <a class="site-card" href="https://zeuthenfurniture.dk" target="_blank" rel="noopener noreferrer">
            <h3>Zeuthenfurniture.dk</h3>
            <p>A furniture-focused website that fits naturally with design, styling, and product presentation work.</p>
            <span class="site-link">Visit site</span>
          </a>

          <a class="site-card" href="https://galleri-zeuthen.dk" target="_blank" rel="noopener noreferrer">
            <h3>Galleri-zeuthen.dk</h3>
            <p>A gallery-oriented website reference showing visual presentation, identity, and a more curated digital atmosphere.</p>
            <span class="site-link">Visit site</span>
          </a>
        </div>

        <a href="#home" class="back-link nav-trigger" data-page="home">Back to front page</a>
      </div>
    </section>

    <section id="solutions" class="page">
      <div class="content-panel">
        <div class="page-header">
          <span class="eyebrow">Solutions</span>
          <h2>End-to-end creative and digital solutions</h2>
          <p class="section-intro">
            I work across the full process not only the final design, but also the setup, content structure, presentation, and practical digital solutions around it.
          </p>
        </div>

        <div class="project-grid">
          <article class="project-card">
            <h3>Setup and foundation</h3>
            <p>I can help from the earliest stage of a project, creating the right direction and digital structure.</p>
            <ul>
              <li>Website setup</li>
              <li>Content structure</li>
              <li>Creative direction</li>
            </ul>
          </article>
          <article class="project-card">
            <h3>Design in all forms</h3>
            <p>The work can cover both visual and functional needs, depending on the project and client.</p>
            <ul>
              <li>Logos and fonts</li>
              <li>PoS materials</li>
              <li>Images and video</li>
            </ul>
          </article>
          <article class="project-card">
            <h3>Tailored delivery</h3>
            <p>Each solution is shaped around the client whether it is a website, gallery experience, furniture presentation, or full visual identity.</p>
            <ul>
              <li>Flexible scope</li>
              <li>Visual consistency</li>
              <li>End-to-end execution</li>
            </ul>
          </article>
        </div>

        <a href="#home" class="back-link nav-trigger" data-page="home">Back to front page</a>
      </div>
    </section>
  </main>

  <footer class="site-footer">
    <p>© 2026 Salamander Studios. Built with HTML, CSS, and JavaScript.</p>
  </footer>

  <script>
    const pages = document.querySelectorAll('.page');
    const navLinks = document.querySelectorAll('.nav-trigger');
    const navMenuLinks = document.querySelectorAll('.nav-link');

    const backgroundVideo = document.getElementById('backgroundVideo');
    const backgroundVideoSource = document.getElementById('backgroundVideoSource');

    const videoMap = {
      home: 'Background_Video2.mp4',
      'design-work': 'Furniture.mp4',
      websites: 'background_websites.mp4',
      solutions: 'Background_Video2.mp4'
    };

    function updateBackgroundVideo(pageId) {
      const nextVideo = videoMap[pageId] || videoMap.home;
      const currentVideo = backgroundVideoSource.getAttribute('src');

      if (currentVideo !== nextVideo) {
        backgroundVideoSource.setAttribute('src', nextVideo);
        backgroundVideo.load();

        const playPromise = backgroundVideo.play();
        if (playPromise !== undefined) {
          playPromise.catch(() => {});
        }
      }
    }

    function showPage(pageId) {
      pages.forEach((page) => {
        page.classList.toggle('active', page.id === pageId);
      });

      navMenuLinks.forEach((link) => {
        link.classList.toggle('active', link.dataset.page === pageId);
      });

      updateBackgroundVideo(pageId);
      window.scrollTo({ top: 0, behavior: 'smooth' });
    }

    function getPageFromHash() {
      const hash = window.location.hash.replace('#', '');
      const validPages = ['home', 'design-work', 'websites', 'solutions'];
      return validPages.includes(hash) ? hash : 'home';
    }

    navLinks.forEach((link) => {
      link.addEventListener('click', (event) => {
        const pageId = link.dataset.page;
        if (!pageId) return;

        event.preventDefault();
        history.pushState(null, '', `#${pageId}`);
        showPage(pageId);
      });
    });

    window.addEventListener('popstate', () => {
      showPage(getPageFromHash());
    });

    backgroundVideo.muted = true;
    backgroundVideo.loop = true;
    backgroundVideo.playsInline = true;

    showPage(getPageFromHash());
  </script>
</body>
</html>
