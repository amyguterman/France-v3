<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>France Travel Guide 2026</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;0,400;0,500;0,600;1,300;1,400&family=DM+Sans:wght@300;400;500&display=swap" rel="stylesheet">
<style>
  :root {
    --cream: #F7F3EE;
    --warm-white: #FDFBF8;
    --stone: #E8E2D9;
    --sage: #7A8C72;
    --sage-light: #C8D4C2;
    --terracotta: #B85C3A;
    --terracotta-light: #F2E0D8;
    --lavender: #7B6FA0;
    --lavender-light: #E4E0EF;
    --gold: #B8963A;
    --gold-light: #F5EDD3;
    --ink: #1C1917;
    --muted: #6B6560;
    --border: #DDD8D0;
    --shadow: 0 2px 16px rgba(28,25,23,0.08);
  }
  * { margin: 0; padding: 0; box-sizing: border-box; }
  body {
    font-family: 'DM Sans', sans-serif;
    background: var(--cream);
    color: var(--ink);
    font-size: 16px;
    line-height: 1.7;
  }

  /* HERO */
  .hero {
    background: var(--ink);
    min-height: 100vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    text-align: center;
    position: relative;
    overflow: hidden;
    padding: 4rem 2rem;
  }
  .hero-bg {
    position: absolute; inset: 0;
    background: 
      radial-gradient(ellipse 120% 80% at 30% 60%, rgba(123,111,160,0.18) 0%, transparent 60%),
      radial-gradient(ellipse 100% 70% at 75% 30%, rgba(184,92,58,0.12) 0%, transparent 55%),
      radial-gradient(ellipse 80% 60% at 50% 80%, rgba(122,140,114,0.15) 0%, transparent 50%);
    z-index: 0;
  }
  .hero-ornament {
    font-family: 'Cormorant Garamond', serif;
    font-size: 11px;
    letter-spacing: 0.35em;
    text-transform: uppercase;
    color: rgba(255,255,255,0.4);
    margin-bottom: 2.5rem;
    position: relative; z-index: 1;
  }
  .hero h1 {
    font-family: 'Cormorant Garamond', serif;
    font-weight: 300;
    font-size: clamp(3rem, 8vw, 6.5rem);
    color: #F7F3EE;
    line-height: 1.05;
    letter-spacing: -0.02em;
    position: relative; z-index: 1;
    margin-bottom: 0.5rem;
  }
  .hero h1 em {
    font-style: italic;
    color: rgba(247,243,238,0.65);
  }
  .hero-subtitle {
    font-family: 'Cormorant Garamond', serif;
    font-size: clamp(1.1rem, 2.5vw, 1.5rem);
    color: rgba(247,243,238,0.55);
    letter-spacing: 0.08em;
    margin-bottom: 3.5rem;
    position: relative; z-index: 1;
    font-weight: 300;
  }
  .hero-dates {
    display: flex;
    gap: 2rem;
    justify-content: center;
    flex-wrap: wrap;
    position: relative; z-index: 1;
    margin-bottom: 3rem;
  }
  .hero-date-pill {
    background: rgba(247,243,238,0.08);
    border: 0.5px solid rgba(247,243,238,0.18);
    border-radius: 100px;
    padding: 0.55rem 1.4rem;
    font-size: 13px;
    color: rgba(247,243,238,0.7);
    letter-spacing: 0.05em;
  }
  .hero-line {
    width: 1px;
    height: 80px;
    background: linear-gradient(to bottom, transparent, rgba(247,243,238,0.3), transparent);
    margin: 0 auto;
    position: relative; z-index: 1;
  }

  /* JOURNEY MAP STRIP */
  .journey-strip {
    background: var(--ink);
    padding: 2rem;
    overflow-x: auto;
    display: flex;
    justify-content: center;
  }
  .journey-strip-inner {
    display: flex;
    align-items: center;
    gap: 0;
    min-width: max-content;
    padding: 0.5rem 0;
  }
  .journey-city {
    text-align: center;
    position: relative;
  }
  .journey-city-name {
    font-family: 'Cormorant Garamond', serif;
    font-size: 15px;
    color: rgba(247,243,238,0.9);
    font-weight: 400;
    display: block;
    margin-bottom: 4px;
  }
  .journey-city-dates {
    font-size: 10px;
    color: rgba(247,243,238,0.4);
    letter-spacing: 0.05em;
    display: block;
  }
  .journey-dot {
    width: 8px; height: 8px;
    border-radius: 50%;
    margin: 8px auto;
  }
  .journey-dot.paris { background: var(--terracotta); }
  .journey-dot.provence { background: var(--lavender); }
  .journey-dot.london { background: var(--sage); }
  .journey-arrow {
    width: 80px;
    height: 1px;
    background: linear-gradient(to right, rgba(247,243,238,0.2), rgba(247,243,238,0.05));
    margin: 0 8px;
    position: relative;
    top: -4px;
  }
  .journey-arrow::after {
    content: '→';
    position: absolute;
    right: -4px;
    top: -9px;
    font-size: 11px;
    color: rgba(247,243,238,0.2);
  }

  /* NAV */
  .sticky-nav {
    position: sticky;
    top: 0;
    background: rgba(247,243,238,0.95);
    backdrop-filter: blur(8px);
    border-bottom: 0.5px solid var(--border);
    z-index: 100;
    padding: 0;
  }
  .nav-inner {
    max-width: 1100px;
    margin: 0 auto;
    display: flex;
    gap: 0;
    overflow-x: auto;
    scrollbar-width: none;
  }
  .nav-inner::-webkit-scrollbar { display: none; }
  .nav-link {
    font-size: 12px;
    letter-spacing: 0.08em;
    text-transform: uppercase;
    color: var(--muted);
    text-decoration: none;
    padding: 1rem 1.2rem;
    white-space: nowrap;
    border-bottom: 2px solid transparent;
    transition: color 0.2s, border-color 0.2s;
    font-weight: 500;
  }
  .nav-link:hover { color: var(--ink); border-color: var(--terracotta); }

  /* MAIN */
  .container {
    max-width: 900px;
    margin: 0 auto;
    padding: 0 1.5rem;
  }

  /* CHAPTER HEADERS */
  .chapter {
    padding: 5rem 0 2rem;
  }
  .chapter-eyebrow {
    font-size: 11px;
    letter-spacing: 0.3em;
    text-transform: uppercase;
    color: var(--terracotta);
    margin-bottom: 1.2rem;
    font-weight: 500;
  }
  .chapter-eyebrow.provence { color: var(--lavender); }
  .chapter-eyebrow.london { color: var(--sage); }
  .chapter-title {
    font-family: 'Cormorant Garamond', serif;
    font-size: clamp(2.2rem, 5vw, 3.5rem);
    font-weight: 300;
    line-height: 1.1;
    color: var(--ink);
    margin-bottom: 0.5rem;
    letter-spacing: -0.02em;
  }
  .chapter-title em { font-style: italic; color: var(--muted); }
  .chapter-desc {
    font-size: 15px;
    color: var(--muted);
    max-width: 600px;
    line-height: 1.8;
    margin-top: 1rem;
    padding-bottom: 2rem;
    border-bottom: 0.5px solid var(--border);
  }

  /* DAY CARDS */
  .day-block {
    margin: 2.5rem 0;
    display: grid;
    grid-template-columns: 100px 1fr;
    gap: 0 2rem;
  }
  @media (max-width: 600px) {
    .day-block { grid-template-columns: 1fr; gap: 0; }
  }
  .day-label {
    padding-top: 0.25rem;
  }
  .day-number {
    font-family: 'Cormorant Garamond', serif;
    font-size: 3rem;
    font-weight: 300;
    color: var(--stone);
    line-height: 1;
    display: block;
  }
  .day-name {
    font-size: 10px;
    letter-spacing: 0.15em;
    text-transform: uppercase;
    color: var(--muted);
    display: block;
    margin-top: 2px;
  }
  .day-date {
    font-size: 11px;
    color: var(--terracotta);
    font-weight: 500;
    display: block;
    margin-top: 4px;
  }
  .day-date.provence { color: var(--lavender); }
  .day-content {}

  /* ACTIVITY ITEMS */
  .activity-list {
    border-left: 1px solid var(--border);
    padding-left: 1.5rem;
    position: relative;
  }
  .activity-item {
    position: relative;
    padding: 0.9rem 0;
    border-bottom: 0.5px solid var(--stone);
  }
  .activity-item:last-child { border-bottom: none; }
  .activity-item::before {
    content: '';
    position: absolute;
    left: -1.58rem;
    top: 1.3rem;
    width: 8px;
    height: 8px;
    border-radius: 50%;
    border: 1.5px solid var(--border);
    background: var(--cream);
  }
  .activity-meta {
    display: flex;
    align-items: center;
    gap: 0.6rem;
    margin-bottom: 0.3rem;
    flex-wrap: wrap;
  }
  .activity-time {
    font-size: 11px;
    font-weight: 500;
    color: var(--muted);
    letter-spacing: 0.05em;
    min-width: 60px;
  }
  .activity-tag {
    font-size: 10px;
    letter-spacing: 0.08em;
    text-transform: uppercase;
    padding: 2px 8px;
    border-radius: 100px;
    font-weight: 500;
  }
  .tag-eat { background: var(--gold-light); color: #7A5A18; }
  .tag-site { background: var(--terracotta-light); color: #7A2E12; }
  .tag-sleep { background: var(--stone); color: var(--muted); }
  .tag-travel { background: #E8EEE6; color: #3A5530; }
  .tag-drink { background: var(--lavender-light); color: #3D2F70; }
  .tag-shop { background: #FEF3E2; color: #7A5010; }
  .tag-relax { background: #E6F0EC; color: #2A5040; }
  .reserved-badge {
    font-size: 10px;
    background: #E8F5E9;
    color: #2E7D32;
    padding: 2px 8px;
    border-radius: 100px;
    font-weight: 500;
    letter-spacing: 0.04em;
  }
  .call-badge {
    font-size: 10px;
    background: #FFF3E0;
    color: #E65100;
    padding: 2px 8px;
    border-radius: 100px;
    font-weight: 500;
    letter-spacing: 0.04em;
  }
  .optional-badge {
    font-size: 10px;
    background: var(--stone);
    color: var(--muted);
    padding: 2px 8px;
    border-radius: 100px;
    font-weight: 500;
    letter-spacing: 0.04em;
  }
  .activity-name {
    font-size: 15px;
    font-weight: 500;
    color: var(--ink);
    margin-bottom: 0.2rem;
  }
  .activity-location {
    font-size: 12px;
    color: var(--muted);
    margin-bottom: 0.3rem;
  }
  .activity-note {
    font-size: 13px;
    color: #5A5550;
    line-height: 1.6;
  }
  .activity-travel {
    font-size: 12px;
    color: var(--sage);
    font-weight: 500;
    margin-top: 0.3rem;
    display: flex;
    align-items: center;
    gap: 4px;
  }
  .activity-travel::before { content: '→'; }

  /* CONTEXT CARDS */
  .context-card {
    background: var(--warm-white);
    border: 0.5px solid var(--border);
    border-radius: 16px;
    padding: 1.75rem;
    margin: 2rem 0;
    box-shadow: var(--shadow);
  }
  .context-card.featured {
    background: var(--ink);
    border-color: transparent;
    color: rgba(247,243,238,0.85);
  }
  .context-card.featured .context-title { color: #F7F3EE; }
  .context-card.featured p { color: rgba(247,243,238,0.75); }
  .context-title {
    font-family: 'Cormorant Garamond', serif;
    font-size: 1.4rem;
    font-weight: 400;
    color: var(--ink);
    margin-bottom: 0.8rem;
    letter-spacing: -0.01em;
  }
  .context-card p {
    font-size: 14px;
    line-height: 1.8;
    color: #4A4540;
    margin-bottom: 0.7rem;
  }
  .context-card p:last-child { margin-bottom: 0; }

  /* PHOTO GRID */
  .photo-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 12px;
    margin: 2rem 0;
  }
  .photo-cell {
    border-radius: 10px;
    overflow: hidden;
    aspect-ratio: 4/3;
    background: var(--stone);
    position: relative;
  }
  .photo-cell img {
    width: 100%; height: 100%;
    object-fit: cover;
    display: block;
    transition: transform 0.4s ease;
  }
  .photo-cell:hover img { transform: scale(1.03); }
  .photo-caption {
    font-size: 11px;
    color: var(--muted);
    margin-top: 6px;
    letter-spacing: 0.03em;
  }

  /* ROUTE CARDS */
  .route-card {
    background: linear-gradient(135deg, #F0EDE8 0%, #E8E4DE 100%);
    border: 0.5px solid var(--border);
    border-radius: 12px;
    padding: 1.25rem 1.5rem;
    margin: 1.2rem 0;
    display: flex;
    align-items: flex-start;
    gap: 1rem;
  }
  .route-icon {
    font-size: 1.5rem;
    flex-shrink: 0;
    margin-top: 2px;
  }
  .route-title {
    font-weight: 500;
    font-size: 14px;
    color: var(--ink);
    margin-bottom: 3px;
  }
  .route-desc {
    font-size: 13px;
    color: var(--muted);
    line-height: 1.6;
  }
  .route-time {
    font-size: 11px;
    color: var(--sage);
    font-weight: 500;
    margin-top: 4px;
  }

  /* LOGISTICS BOX */
  .logistics-box {
    background: var(--warm-white);
    border: 0.5px solid var(--border);
    border-radius: 12px;
    padding: 1.5rem;
    margin: 1.5rem 0;
  }
  .logistics-title {
    font-size: 11px;
    letter-spacing: 0.2em;
    text-transform: uppercase;
    color: var(--lavender);
    margin-bottom: 1rem;
    font-weight: 500;
  }
  .logistics-row {
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
    padding: 0.6rem 0;
    border-bottom: 0.5px solid var(--stone);
    gap: 1rem;
    flex-wrap: wrap;
  }
  .logistics-row:last-child { border-bottom: none; }
  .logistics-label {
    font-size: 13px;
    color: var(--muted);
    font-weight: 400;
  }
  .logistics-value {
    font-size: 13px;
    font-weight: 500;
    color: var(--ink);
    text-align: right;
  }
  .logistics-value.confirmed { color: #2E7D32; }

  /* SECTION DIVIDER */
  .divider {
    display: flex;
    align-items: center;
    gap: 1.5rem;
    margin: 4rem 0 2rem;
  }
  .divider-line { flex: 1; height: 0.5px; background: var(--border); }
  .divider-text {
    font-family: 'Cormorant Garamond', serif;
    font-size: 1.1rem;
    font-style: italic;
    color: var(--muted);
    white-space: nowrap;
    font-weight: 300;
  }

  /* TIP CALLOUT */
  .tip {
    border-left: 3px solid var(--gold);
    padding: 0.8rem 1rem 0.8rem 1.25rem;
    background: var(--gold-light);
    border-radius: 0 8px 8px 0;
    margin: 1rem 0;
    font-size: 13px;
    color: #5A4010;
    line-height: 1.7;
  }
  .tip strong { font-weight: 500; color: #4A3008; }

  /* FOOTER */
  .footer {
    background: var(--ink);
    padding: 4rem 2rem;
    text-align: center;
    margin-top: 6rem;
  }
  .footer-title {
    font-family: 'Cormorant Garamond', serif;
    font-size: 2rem;
    color: rgba(247,243,238,0.8);
    font-weight: 300;
    margin-bottom: 0.8rem;
    font-style: italic;
  }
  .footer-sub {
    font-size: 13px;
    color: rgba(247,243,238,0.3);
    letter-spacing: 0.1em;
  }

  /* RESPONSIVE */
  @media (max-width: 768px) {
    .chapter { padding: 3rem 0 1.5rem; }
    .day-block { grid-template-columns: 1fr; }
    .day-label { display: flex; align-items: baseline; gap: 1rem; padding-bottom: 1rem; }
    .day-number { font-size: 2rem; }
    .activity-list { padding-left: 1rem; }
  }
</style>
</head>
<body>

<!-- HERO -->
<header class="hero">
  <div class="hero-bg"></div>
  <p class="hero-ornament">A Personal Travel Guide</p>
  <h1>La Belle <em>France</em></h1>
  <p class="hero-subtitle">Paris · Provence · London &nbsp;·&nbsp; June 2026</p>
  <div class="hero-dates">
    <span class="hero-date-pill">Paris — Jun 7–10</span>
    <span class="hero-date-pill">Provence — Jun 10–14</span>
    <span class="hero-date-pill">Return Paris — Jun 14</span>
    <span class="hero-date-pill">London — Jun 15+</span>
  </div>
  <div class="hero-line"></div>
</header>

<!-- JOURNEY STRIP -->
<div class="journey-strip">
  <div class="journey-strip-inner">
    <div class="journey-city">
      <span class="journey-city-name">Chicago</span>
      <div class="journey-dot" style="background:#555;"></div>
      <span class="journey-city-dates">Jun 7</span>
    </div>
    <div class="journey-arrow"></div>
    <div class="journey-city">
      <span class="journey-city-name">Paris</span>
      <div class="journey-dot paris"></div>
      <span class="journey-city-dates">Jun 7–10 &amp; Jun 14</span>
    </div>
    <div class="journey-arrow"></div>
    <div class="journey-city">
      <span class="journey-city-name">Avignon TGV</span>
      <div class="journey-dot" style="background:#C8A0D8;"></div>
      <span class="journey-city-dates">Jun 10</span>
    </div>
    <div class="journey-arrow"></div>
    <div class="journey-city">
      <span class="journey-city-name">Gordes</span>
      <div class="journey-dot provence"></div>
      <span class="journey-city-dates">Jun 10–14</span>
    </div>
    <div class="journey-arrow"></div>
    <div class="journey-city">
      <span class="journey-city-name">London</span>
      <div class="journey-dot" style="background:#7A8C72;"></div>
      <span class="journey-city-dates">Jun 15+</span>
    </div>
    <div class="journey-arrow"></div>
    <div class="journey-city">
      <span class="journey-city-name">Chicago</span>
      <div class="journey-dot" style="background:#555;"></div>
      <span class="journey-city-dates">Jun 15</span>
    </div>
  </div>
</div>

<!-- NAV -->
<nav class="sticky-nav">
  <div class="nav-inner">
    <a href="#paris" class="nav-link">Paris</a>
    <a href="#day1" class="nav-link">Day 1 — Arrival</a>
    <a href="#day2" class="nav-link">Day 2 — Grands Monuments</a>
    <a href="#day3" class="nav-link">Day 3 — Left Bank</a>
    <a href="#provence" class="nav-link">Provence</a>
    <a href="#day4" class="nav-link">Day 4 — Gordes</a>
    <a href="#day5" class="nav-link">Day 5 — Luberon</a>
    <a href="#day6" class="nav-link">Day 6 — Ochre Trail</a>
    <a href="#day7" class="nav-link">Day 7 — Saint-Rémy</a>
    <a href="#day8" class="nav-link">Day 8 — Return</a>
    <a href="#london" class="nav-link">London</a>
  </div>
</nav>

<!-- ===================== PARIS ===================== -->
<section id="paris">
<div class="container">

  <div class="chapter">
    <p class="chapter-eyebrow">Part One</p>
    <h2 class="chapter-title">Paris,<br><em>the luminous city</em></h2>
    <p class="chapter-desc">Three days in the French capital — beginning in the beating heart of Le Marais and spiraling outward through boulevards, grand museums, and candlelit bistros. Paris rewards those who walk slowly and eat often.</p>
  </div>

  <div class="context-card">
    <h3 class="context-title">Staying in the 11th Arrondissement</h3>
    <p>Hotel Le Mareuil sits in the 11th arrondissement, one of Paris's most effortlessly cool neighborhoods. Far from the tourist-facing polish of Saint-Germain, the 11th blends natural wine bars with Lebanese bakeries, vintage record shops with design studios. It borders Le Marais directly, which means you are ten minutes from Place des Vosges and twenty from the Seine — close enough to everything, yet pleasantly removed from the crowds.</p>
    <p>The neighborhood also puts you within easy Metro reach of every major site on this itinerary, making it an ideal base for a trip that moves between two very different Parises: the iconic monuments to the west, and the lived-in, neighborhood Paris right outside your door.</p>
  </div>

  <!-- DAY 1 -->
  <div id="day1" class="day-block">
    <div class="day-label">
      <span class="day-number">01</span>
      <span class="day-name">Sunday</span>
      <span class="day-date">June 7</span>
    </div>
    <div class="day-content">
      <div class="activity-list">

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-time">11:00 AM</span>
            <span class="activity-tag tag-travel">Travel</span>
          </div>
          <div class="activity-name">Arrive in Paris</div>
          <div class="activity-note">Touch down and take a breath. The first day is intentionally light — after a transatlantic flight, flexibility is everything. If bags are checked and energy allows, the afternoon ahead will be a gentle introduction to Paris at a true wanderer's pace.</div>
        </div>

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-time">1:00 PM</span>
            <span class="activity-tag tag-sleep">Hotel</span>
            <span class="reserved-badge">✓ Confirmed</span>
          </div>
          <div class="activity-name">Hotel Le Mareuil — Check In (3 PM)</div>
          <div class="activity-location">51 Rue De Malte, Paris 75011</div>
          <div class="activity-note">Drop bags early, freshen up, and resist the urge to over-plan. Check-in is officially 3 PM. The 11th is a strong food and wine base and a short walk to Le Marais.</div>
        </div>

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-tag tag-eat">Eat</span>
          </div>
          <div class="activity-name">Marché des Enfants Rouges</div>
          <div class="activity-note">One of Paris's oldest covered markets (dating to 1615), Marché des Enfants Rouges is the perfect jet-lagged first stop: colorful, casual, and packed with stalls serving everything from Chez Alain Miam Miam's legendary sandwiches to Japanese bento, Moroccan tagine, and fresh oysters. Get there before 5 PM — it closes early on Sundays and is closed Mondays. It reopens Tuesday.</div>
          <div class="activity-travel">10–15 min walk from hotel</div>
        </div>

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-time">2:00 PM</span>
            <span class="activity-tag tag-site">Explore</span>
          </div>
          <div class="activity-name">Le Marais + Place des Vosges</div>
          <div class="activity-note">Start with no reservations and no agenda: wander the arcades, browse boutiques and galleries, find a café under the chestnut trees. Place des Vosges — Paris's oldest planned square, built in 1612 — is one of those places that consistently exceeds expectations. Its symmetry, its reddish stone, the way it holds both tourists and locals without feeling crowded: it's the ideal first impression of Paris.</div>
          <div class="activity-travel">Hotel → Place des Vosges: ~25 min walk or 10–12 min Metro (Lines 1 or 8 from Bastille)</div>
        </div>

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-time">3:15 PM</span>
            <span class="activity-tag tag-site">Walk</span>
          </div>
          <div class="activity-name">Le Marais Walking Loop</div>
          <div class="activity-note">Suggested route: Place des Vosges → Rue des Francs-Bourgeois (fashion and home boutiques, free entry to Musée Carnavalet courtyards) → Hôtel de Ville → the Seine edge if energy holds. Keep it loose and romantic. This is the Paris of hidden courtyards, centuries-old hôtels particuliers, and unexpected archways. One to two miles at a slow pace.</div>
        </div>

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-tag tag-drink">Evening</span>
          </div>
          <div class="activity-name">Wine Bar — Light Dinner</div>
          <div class="activity-note">The 11th and Le Marais are Paris's natural wine heartland. Look for a casual bistronomie or wine bar for your first Parisian dinner: a glass of something orange, a tartine, a cheese plate. No pressure for a grand meal on night one.</div>
        </div>

      </div>
    </div>
  </div>

  <div class="divider"><div class="divider-line"></div><span class="divider-text">Promenons-nous</span><div class="divider-line"></div></div>

  <!-- DAY 2 -->
  <div id="day2" class="day-block">
    <div class="day-label">
      <span class="day-number">02</span>
      <span class="day-name">Monday</span>
      <span class="day-date">June 8</span>
    </div>
    <div class="day-content">
      <div class="activity-list">

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-time">8:30 AM</span>
            <span class="activity-tag tag-eat">Breakfast</span>
          </div>
          <div class="activity-name">Boulangerie Utopie</div>
          <div class="activity-note">A neighborhood gem beloved for its creative, seasonal viennoiserie. Think kouign-amann with unexpected fillings, croissants with a shattering butter crust, and sourdough loaves worth carrying home. Get there early — the good stuff goes fast. Walking distance from the hotel.</div>
        </div>

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-time">9:30 AM</span>
            <span class="activity-tag tag-travel">Transit</span>
          </div>
          <div class="activity-name">Transit to Trocadéro</div>
          <div class="activity-note">Head west before the crowds build. The Eiffel Tower experience is completely different — and far better — when seen first from the Trocadéro side, with the city stretching behind it.</div>
          <div class="activity-travel">11th arrondissement → Trocadéro: ~35 min Metro (Line 9 to Trocadéro) or 40 min taxi</div>
        </div>

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-time">10:15 AM</span>
            <span class="activity-tag tag-site">Viewpoint</span>
          </div>
          <div class="activity-name">Place du Trocadéro — Eiffel Tower View</div>
          <div class="activity-note">The finest Eiffel Tower photograph in Paris is not taken from the base — it's taken from the Trocadéro esplanade, where the tower frames itself perfectly against the sky, the Champ de Mars stretching behind it. The Jardins du Trocadéro below are lovely for a slow stroll. Unless rooftop views are a top priority, enjoying the tower from this vantage (rather than climbing it) gives you more time and far more atmosphere.</div>
          <div class="activity-travel">2–5 min walk from Trocadéro Metro exit</div>
        </div>

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-time">11:00 AM</span>
            <span class="activity-tag tag-eat">Café Stop</span>
          </div>
          <div class="activity-name">Carette, Trocadéro</div>
          <div class="activity-note">An institution on the Place du Trocadéro since 1927. The macarons are genuinely excellent, the hot chocolate is legendary, and the terrace people-watching is second to none. Treat it as the iconic and scenic experience it is — go early to beat the queues. Not a hidden gem, but a worthy one.</div>
          <div class="activity-travel">5–10 min walk from the Trocadéro viewpoint</div>
        </div>

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-time">11:45 AM</span>
            <span class="activity-tag tag-site">Monument</span>
          </div>
          <div class="activity-name">Arc de Triomphe</div>
          <div class="activity-note">Napoleon commissioned this monument in 1806, following his victory at Austerlitz, though it wasn't completed until 1836. At its center burns France's Eternal Flame, honoring the Unknown Soldier of World War I. Admire it from street level — or climb the 284 steps for a panoramic view down the twelve radiating avenues, with the Eiffel Tower behind you and La Défense ahead. The underground pedestrian tunnel to the island is the only safe way to reach it.</div>
          <div class="activity-travel">Carette/Trocadéro → Arc: ~20 min walk along Av. Kléber, or 10 min Metro (Line 6 to Charles de Gaulle–Étoile)</div>
        </div>

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-time">12:30 PM</span>
            <span class="activity-tag tag-site">Stroll</span>
          </div>
          <div class="activity-name">Brief Champs-Élysées Stroll</div>
          <div class="activity-note">A twenty-to-thirty minute walk down the grand boulevard — it's iconic, and worth experiencing at least once. It is, however, heavily commercial and not the most atmospheric part of Paris, so resist the urge to linger. The tree-lined median and the sheer scale of it are genuinely impressive.</div>
        </div>

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-time">1:00 PM</span>
            <span class="activity-tag tag-eat">Lunch</span>
          </div>
          <div class="activity-name">Lunch — Golden Triangle / 8th Arr.</div>
          <div class="activity-note">The streets behind the Champs-Élysées hide some excellent bistros and brasseries. Look for a classic French lunch: steak frites, croque monsieur, or a plat du jour with a glass of Burgundy.</div>
        </div>

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-time">3:00 PM</span>
            <span class="activity-tag tag-shop">Shopping</span>
          </div>
          <div class="activity-name">Shopping — Galeries Lafayette & Publicis Drugstore</div>
          <div class="activity-note">Galeries Lafayette Champs-Élysées is the smaller, sleeker sibling of the Opéra flagship — a curated department store strong on beauty, accessories, and French brands. Publicis Drugstore next door is a Parisian institution: part café, part bookshop, part pharmacy, with a great selection of French beauty products unavailable at home.</div>
        </div>

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-time">4:00 PM</span>
            <span class="activity-tag tag-sleep">Rest</span>
          </div>
          <div class="activity-name">Hotel Rest</div>
          <div class="activity-note">Reset after a long walking day. Decide later whether you need a full dinner or just wine and light bites. Montmartre at sunset is optional but lovely if energy holds.</div>
          <div class="activity-travel">North Marais/8th → 11th hotel: ~15–20 min taxi or Metro (Line 9, direction Montreuil)</div>
        </div>

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-time">5:00 PM</span>
            <span class="activity-tag tag-site">Optional</span>
            <span class="optional-badge">Optional</span>
          </div>
          <div class="activity-name">Montmartre — Drinks at Sunset</div>
          <div class="activity-note">If the legs are willing: Montmartre's steep, cobbled lanes and the white-domed Sacré-Cœur basilica make for an atmospheric late-afternoon wander. The neighborhood's artistic legacy — Picasso, Renoir, and Toulouse-Lautrec all lived and worked here — lingers in its village-like streets. The Lapin Agile and Place du Tertre have a certain touristy charm worth embracing, and there are genuinely good wine bars on the slopes.</div>
        </div>

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-time">8:00 PM</span>
            <span class="activity-tag tag-eat">Dinner</span>
            <span class="reserved-badge">✓ Reservation Confirmed</span>
          </div>
          <div class="activity-name">Restaurant Mieux</div>
          <div class="activity-location">21 Rue Saint-Lazare, 75009 Paris (9th arr.)</div>
          <div class="activity-note">A reservation-confirmed dinner in the lively 9th arrondissement, close to the grands boulevards. Mieux is a well-regarded modern French restaurant with a strong wine list — a proper first sit-down dinner in Paris.</div>
          <div class="activity-travel">Hotel → Mieux: ~20–25 min Metro or 15 min taxi</div>
        </div>

      </div>
    </div>
  </div>

  <div class="context-card">
    <h3 class="context-title">Arc de Triomphe &amp; Trocadéro — Practical Notes</h3>
    <p>The Arc de Triomphe rooftop is accessed via the underground tunnel from the Champs-Élysées — never try to cross the rond-point on foot. Tickets to climb are €13 for adults; book online to skip the queue. The viewpoint is open until 11 PM in summer, making it a spectacular evening option if you prefer it later in the day.</p>
    <p>The Trocadéro and Jardins du Trocadéro are always free and open. The Palais de Chaillot, which flanks the esplanade, houses the Cité de l'Architecture and the Musée de la Marine — both worth noting for a return visit.</p>
  </div>

  <div class="divider"><div class="divider-line"></div><span class="divider-text">La rive gauche</span><div class="divider-line"></div></div>

  <!-- DAY 3 -->
  <div id="day3" class="day-block">
    <div class="day-label">
      <span class="day-number">03</span>
      <span class="day-name">Tuesday</span>
      <span class="day-date">June 9</span>
    </div>
    <div class="day-content">
      <div class="activity-list">

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-time">9:00 AM</span>
            <span class="activity-tag tag-eat">Breakfast</span>
          </div>
          <div class="activity-name">Leisurely French Breakfast</div>
          <div class="activity-note">A slow morning with a proper café breakfast — café crème, a croissant, maybe a tartine with jam. The Marché des Enfants Rouges is open again today (Tuesday through Sunday), and this is a perfect morning to revisit if yesterday's market felt rushed.</div>
          <div class="activity-travel">Food tour is walkable within North Marais; minimal transit once started.</div>
        </div>

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-time">10:00 AM</span>
            <span class="activity-tag tag-site">Landmark</span>
          </div>
          <div class="activity-name">Notre-Dame de Paris — Free Timed Entry</div>
          <div class="activity-note">After the devastating 2019 fire and a five-year restoration, Notre-Dame reopened in December 2024 — and it is genuinely magnificent. The cathedral dates to 1163, when Bishop Maurice de Sully laid the foundation stone. The restored interior is now brighter and more vivid than it has been in centuries. Entry is free but requires a timed ticket reserved online (book 2 days in advance — slots fill quickly during June). Don't miss the opportunity to see it in this rare, freshly restored state.</div>
          <div class="activity-travel">Hotel → Notre-Dame: ~30–35 min Metro (Line 1 to Saint-Paul, then walk to Île de la Cité)</div>
        </div>

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-tag tag-site">Walk</span>
          </div>
          <div class="activity-name">Île Saint-Louis + Seine Walk</div>
          <div class="activity-note">Cross the Pont Saint-Louis from Notre-Dame onto the smaller, quieter Île Saint-Louis — a neighborhood so self-contained it feels like a village floating in the middle of Paris. The main street, Rue Saint-Louis en l'Île, is lined with small specialty shops, galleries, and Berthillon ice cream (the gold standard of Parisian gelato). From the quays, the views back toward Notre-Dame are among the loveliest in the city.</div>
          <div class="activity-travel">Notre-Dame → Île Saint-Louis: 15–20 min slow walk across the bridge</div>
        </div>

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-tag tag-eat">Lunch</span>
          </div>
          <div class="activity-name">Crêperie Little Breizh</div>
          <div class="activity-note">Recommended by Stephanie — a beloved crêperie in Saint-Germain serving authentic Breton galettes (buckwheat crêpes) with savory fillings like ham, egg, and comté, alongside sweet crêpes for dessert. Simple, delicious, and quintessentially French. A perfect lunch before the afternoon museum.</div>
        </div>

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-time">2:00 PM</span>
            <span class="activity-tag tag-site">Museum</span>
            <span class="reserved-badge">✓ Timed Entry at 2:00 PM</span>
          </div>
          <div class="activity-name">Musée d'Orsay — Renoir &amp; Impressionist Collection</div>
          <div class="activity-note">Housed in a magnificent 1900 Beaux-Arts railway station, the Musée d'Orsay holds the world's greatest collection of Impressionist and Post-Impressionist art. Monet's light-dappled canvases, Degas's backstage ballet scenes, Renoir's sun-saturated gatherings — they are all here, filling room after luminous room. The Renoir exhibit is a particular highlight this season. Your timed entry at 2 PM means you skip the long walk-up queues. Plan for two to three hours minimum; the building itself, with its ornate iron canopy and giant station clock, is half the experience.</div>
          <div class="activity-travel">Île Saint-Louis → Orsay: ~20 min walk along the Left Bank, or ~10 min Metro (RER C to Musée d'Orsay)</div>
        </div>

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-tag tag-site">Stroll</span>
          </div>
          <div class="activity-name">Walk by the Louvre &amp; Tuileries Gardens</div>
          <div class="activity-note">After Orsay, cross the Seine and stroll through the Jardin des Tuileries — Paris's formal royal garden, laid out by André Le Nôtre in 1664. In June, the fountains are on, the chairs are out by the ponds, and the light is golden. The view from the garden's eastern end toward the Louvre's pyramid is one of the city's great vistas. No need to go inside — this is a walk, not a museum visit.</div>
          <div class="activity-travel">Orsay → Tuileries: cross Pont Royal, ~5 min walk to garden entrance</div>
        </div>

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-tag tag-drink">Pre-Dinner</span>
          </div>
          <div class="activity-name">Wine — Les Amoureuses &amp; A Lot of Wine</div>
          <div class="activity-location">Near Hotel Le Mareuil, 11th arr.</div>
          <div class="activity-note">Two nearby natural wine bars worth knowing. Les Amoureuses has snacks and a genuinely excellent selection of small-producer wines. A Lot of Wine is more relaxed and casual. Either makes a perfect pre-dinner stop before your 7:30 PM reservation.</div>
          <div class="activity-travel">Return to hotel area: ~25–35 min taxi or Metro from Tuileries</div>
        </div>

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-time">7:30 PM</span>
            <span class="activity-tag tag-eat">Dinner</span>
            <span class="reserved-badge">✓ Reservation Confirmed</span>
          </div>
          <div class="activity-name">Dinner Option 1: Chez René</div>
          <div class="activity-note">A classic Parisian bistro on the Left Bank, Chez René has been serving traditional French cooking — boeuf bourguignon, sole meunière, tarte tatin — since 1957. The red-checked tablecloths, the chalked blackboard menu, the Beaujolais flowing freely: it is everything a French bistro dinner should be. Reservation confirmed.</div>
        </div>

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-time">7:30 PM</span>
            <span class="activity-tag tag-eat">Dinner</span>
            <span class="reserved-badge">✓ Reservation Confirmed</span>
          </div>
          <div class="activity-name">Dinner Option 2: Au Bourguignon du Marais</div>
          <div class="activity-note">An alternative reservation also confirmed — a warm, wine-focused bistro in Le Marais specializing in Burgundian cuisine. Excellent for those who want a shorter taxi ride home and a slightly more neighborhood feel. Both options are strong; choose based on mood and energy levels.</div>
        </div>

      </div>
    </div>
  </div>

  <div class="context-card featured">
    <h3 class="context-title">Practical Paris — Getting Around</h3>
    <p>The Metro is Paris's workhorse: fast, frequent, and cheap (a carnet of 10 tickets or a Navigo Easy card is the best value for 3–4 days). For later evenings or with luggage, taxis and Uber/Bolt are plentiful and straightforward from the app. Walking between arrondissements is almost always the most enjoyable option for daytime movement — Paris is smaller than it looks, and the streets between the monuments are often the best part of the trip.</p>
  </div>

</div>
</section>

<!-- ===================== PROVENCE ===================== -->
<section id="provence">
<div class="container">

  <div class="chapter">
    <p class="chapter-eyebrow provence">Part Two</p>
    <h2 class="chapter-title">Provence,<br><em>the perfumed south</em></h2>
    <p class="chapter-desc">Four days in the Luberon — one of the most beautiful corners of France. Hilltop villages built of golden stone, lavender fields edging toward bloom, Sunday markets overflowing with olives and rosé, and a sky that seems a shade bluer than anywhere else in the world.</p>
  </div>

  <div class="logistics-box">
    <div class="logistics-title">Travel Logistics — Paris → Gordes</div>
    <div class="logistics-row">
      <span class="logistics-label">TGV Train</span>
      <span class="logistics-value confirmed">✓ TGV INOUI #6107 — Confirmed</span>
    </div>
    <div class="logistics-row">
      <span class="logistics-label">Departs Paris Gare de Lyon</span>
      <span class="logistics-value">9:38 AM, Wednesday June 10</span>
    </div>
    <div class="logistics-row">
      <span class="logistics-label">Arrives Avignon TGV</span>
      <span class="logistics-value">~12:18 PM (2 hr 40 min)</span>
    </div>
    <div class="logistics-row">
      <span class="logistics-label">Rental Car — Hertz Automatic</span>
      <span class="logistics-value confirmed">✓ Confirmation #L6023264298</span>
    </div>
    <div class="logistics-row">
      <span class="logistics-label">Drive Avignon TGV → Gordes</span>
      <span class="logistics-value">~50 min (pick up car ~12:30 PM)</span>
    </div>
    <div class="logistics-row">
      <span class="logistics-label">Hotel — Le Jas de Gordes</span>
      <span class="logistics-value">955 Route des Moines, Gordes 84220</span>
    </div>
  </div>

  <div class="tip">
    <strong>Scenic drive note:</strong> The route from Avignon TGV station toward Gordes takes you through the heart of the Luberon Regional Nature Park — expect stone-wall villages, vineyard-striped hillsides, and a landscape that looks lifted from a Cézanne canvas. The D900 and D2 road via Coustellet and Maubec is the most beautiful approach to Gordes. Add 10 minutes but it is worth every one of them.
  </div>

  <div class="context-card">
    <h3 class="context-title">Gordes — The Crown of the Luberon</h3>
    <p>Gordes is routinely named one of France's most beautiful villages (Les Plus Beaux Villages de France), and it earns that designation without apology. Perched dramatically on a hillside of the Vaucluse Plateau, the village cascades in tiers of pale stone down toward the valley below, its 11th-century château anchoring the summit. In June, the surrounding landscape shifts from green to the first traces of purple as the lavender begins to stir.</p>
    <p>Le Jas de Gordes sits just outside the village on the Route des Moines, surrounded by stone terraces, lavender plantings, and a pool with views across the valley. It is a genuinely beautiful hotel — equal parts traditional Provençal mas and contemporary comfort. This will very likely be the best hotel of the trip.</p>
  </div>

  <!-- DAY 4 -->
  <div id="day4" class="day-block">
    <div class="day-label">
      <span class="day-number">04</span>
      <span class="day-name">Wednesday</span>
      <span class="day-date">June 10</span>
    </div>
    <div class="day-content">
      <div class="activity-list">

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-time">8:00 AM</span>
            <span class="activity-tag tag-travel">Travel</span>
          </div>
          <div class="activity-name">Check Out of Hotel Le Mareuil</div>
          <div class="activity-note">Morning TGV to Provence. Leave enough time to collect bags and get to Paris Gare de Lyon — allow at least 45 minutes from the hotel by Metro or taxi. Line 1 goes directly to Gare de Lyon.</div>
        </div>

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-time">9:38 AM</span>
            <span class="activity-tag tag-travel">TGV</span>
            <span class="reserved-badge">✓ TGV INOUI #6107</span>
          </div>
          <div class="activity-name">Paris Gare de Lyon → Avignon TGV</div>
          <div class="activity-note">Two hours and forty minutes on France's high-speed rail, reaching speeds over 300 km/h. The journey from Paris to Provence by TGV is one of those travel experiences that still feels slightly miraculous. Sit on the right side heading south for better views as you enter the Rhône Valley.</div>
        </div>

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-time">12:30 PM</span>
            <span class="activity-tag tag-travel">Car Rental</span>
            <span class="reserved-badge">✓ Hertz — Confirmed</span>
          </div>
          <div class="activity-name">Pick Up Rental Car at Avignon TGV</div>
          <div class="activity-note">Hertz is located directly at the Avignon TGV station. The car is automatic — essential for navigating narrow Provençal village roads with confidence. Note: Avignon TGV is separate from Avignon Centre station; make sure you're at the right terminal.</div>
        </div>

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-time">2:00 PM</span>
            <span class="activity-tag tag-travel">Drive</span>
          </div>
          <div class="activity-name">Avignon TGV → Gordes</div>
          <div class="activity-note">~50 minutes south through the Luberon. The most scenic route: take the D900 east toward L'Isle-sur-la-Sorgue, then the D2 south through Coustellet and Maubec, climbing up to Gordes. This approach gives you the classic Gordes-from-below reveal as you round the final bend.</div>
        </div>

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-time">3:00 PM</span>
            <span class="activity-tag tag-sleep">Hotel</span>
          </div>
          <div class="activity-name">Check In — Le Jas de Gordes</div>
          <div class="activity-location">955 Route des Moines, Gordes 84220</div>
          <div class="activity-note">Drop luggage, breathe in the lavender-tinged air, and take in the valley views. The pool will be extremely tempting — save it for later in the week when you need recovery time after village-hopping.</div>
        </div>

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-time">5:00 PM</span>
            <span class="activity-tag tag-site">Landmark</span>
          </div>
          <div class="activity-name">Abbaye de Sénanque — Lavender Fields</div>
          <div class="activity-note">The image of Sénanque Abbey — a medieval Cistercian monastery founded in 1148, its grey stone rising from a sea of lavender — is one of the defining images of Provence. In mid-June, the lavender is typically at early bloom or approaching peak; exact timing varies by year. Check the current bloom status at routes-lavande.com before visiting. The monks still live and pray here, and the atmosphere — the silence, the scent, the afternoon light on ancient stone — is genuinely moving. The shop sells the monks' own lavender honey, essential oils, and liqueurs.</div>
          <div class="activity-travel">Le Jas de Gordes → Sénanque: ~10 min drive (D177, sign-posted from Gordes)</div>
        </div>

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-time">7:15 PM</span>
            <span class="activity-tag tag-eat">Dinner</span>
            <span class="reserved-badge">✓ Reservation Confirmed</span>
          </div>
          <div class="activity-name">L'Outsider — Gordes</div>
          <div class="activity-note">A well-regarded restaurant in Gordes with a reservation already secured for your first evening in Provence. The terrace has views across the Luberon valley — a perfect setting for a first proper Provençal dinner: local lamb, herbed cheeses, and the area's excellent Luberon rosé.</div>
        </div>

      </div>
    </div>
  </div>

  <div class="divider"><div class="divider-line"></div><span class="divider-text">Les villages du Luberon</span><div class="divider-line"></div></div>

  <!-- DAY 5 -->
  <div id="day5" class="day-block">
    <div class="day-label">
      <span class="day-number">05</span>
      <span class="day-name">Thursday</span>
      <span class="day-date">June 11</span>
    </div>
    <div class="day-content">
      <div class="activity-list">

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-time">9:00 AM</span>
            <span class="activity-tag tag-shop">Market</span>
          </div>
          <div class="activity-name">Goult Thursday Market (8:00 AM – 12:30 PM)</div>
          <div class="activity-note">One of the Luberon's most authentic markets — less touristic than Lourmarin or L'Isle-sur-la-Sorgue, more genuinely local. In June the stalls are piled with early-season cherries, strawberries, and young garlic, alongside artisan olive oils, aged goat cheeses wrapped in chestnut leaves, and Provençal linen. This is the market for eating breakfast standing up with a paper coffee cup and a warm socca (chickpea pancake).</div>
          <div class="activity-travel">Gordes → Goult: ~15 min drive (D104 and D2 south)</div>
        </div>

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-time">12:00 PM</span>
            <span class="activity-tag tag-travel">Scenic Drive</span>
          </div>
          <div class="activity-name">Goult → Ménerbes</div>
          <div class="activity-note">A fifteen-minute drive southwest through the Luberon's northern ridge. Ménerbes is made famous by Peter Mayle's "A Year in Provence" — a sleepy hilltop village of golden ochre stone, ancient fortifications, and sweeping views south across the valley. Wander the main street and stop for a coffee at the village café.</div>
        </div>

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-time">1:00 PM</span>
            <span class="activity-tag tag-drink">Wine Tasting</span>
            <span class="reserved-badge">✓ Reservation Confirmed</span>
          </div>
          <div class="activity-name">Domaine de la Citadelle — Wine Tasting</div>
          <div class="activity-location">Ménerbes, Luberon</div>
          <div class="activity-note">Domaine de la Citadelle is one of the Luberon's most celebrated wine estates, producing both AOC Luberon whites and rosés and a remarkable collection of corkscrews displayed in their on-site museum (yes, really — it is genuinely charming). The tasting is confirmed, and the setting — vines curling around the château's old stone walls — is exactly what you'd imagine Provençal wine tasting to look like. The rosé is particularly worth bringing home.</div>
        </div>

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-time">3:00 PM</span>
            <span class="activity-tag tag-travel">Scenic Drive</span>
          </div>
          <div class="activity-name">Ménerbes → Bonnieux</div>
          <div class="activity-note">Continue east on the D109. Bonnieux is one of the Luberon's most dramatically situated villages — perched on a cliff edge above the valley, its upper village connected by steep medieval lanes to a Romanesque church with sweeping views. The village holds a small dog-collar museum (a quirky local gem), and the panorama from the upper church terrace takes in the full sweep of the Luberon valley toward Lacoste and Gordes.</div>
          <div class="activity-travel">15 min drive, D3 east from Ménerbes</div>
        </div>

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-tag tag-travel">Drive</span>
          </div>
          <div class="activity-name">Bonnieux → Lourmarin</div>
          <div class="activity-note">Continue twenty minutes south through the Combe de Lourmarin — the only pass cutting through the Luberon massif, a dramatic gorge of rock walls and scrub oak that opens suddenly onto the southern Luberon plain. Lourmarin is the most chic and internationally known of the Luberon villages, home to the château where Albert Camus is buried and a bustling market-town energy that feels slightly more cosmopolitan than the northern ridge villages.</div>
          <div class="activity-travel">20 min drive, D943 south through the Combe</div>
        </div>

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-time">3:30 PM</span>
            <span class="activity-tag tag-shop">Shopping</span>
          </div>
          <div class="activity-name">Lourmarin — Wander, Shop &amp; Snack</div>
          <div class="activity-note">Lourmarin rewards slow wandering. Standout finds include local ceramicist Pierre Busson at his Atelier Buisson Kessler, Le Village de Pierre et Céline (design and home goods), Les Commissions du Moulin (local olive oil — worth taking a bottle home), Boutique l'Écrin, and Polette Lourmarin. The Friday market (held the morning after your visit) is Lourmarin's most famous, but the village's permanent boutiques are excellent in their own right.</div>
        </div>

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-time">7:00 PM</span>
            <span class="activity-tag tag-eat">Dinner</span>
            <span class="call-badge">📞 Call to Book</span>
          </div>
          <div class="activity-name">Bouchon — Lourmarin (4.8⭐, 450+ reviews)</div>
          <div class="activity-note">A beloved Lourmarin restaurant with exceptional reviews. Call ahead to reserve — this is one of the best-regarded tables in the southern Luberon. Provençal market cooking at its most refined: local lamb, seasonal vegetables, and an excellent local wine list. The sort of dinner you will still be talking about when you get home.</div>
        </div>

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-time">7:15 PM</span>
            <span class="activity-tag tag-eat">Dinner Alt.</span>
            <span class="call-badge">📞 Call to Book</span>
          </div>
          <div class="activity-name">Le Mas — Gordes (Michelin, 4.8⭐)</div>
          <div class="activity-note">Elegant countryside dinner near your hotel — a Michelin-listed option for the more formal evening. Chef Alexis Osmont's cooking is rooted in Provençal tradition but carefully contemporary. Perfect if you want a special occasion dinner closer to the hotel at Le Jas de Gordes.</div>
        </div>

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-time">9:00 PM</span>
            <span class="activity-tag tag-travel">Return</span>
          </div>
          <div class="activity-name">Lourmarin → Gordes</div>
          <div class="activity-note">The evening drive back through the Luberon: 35 minutes north through the Combe de Lourmarin and up to Gordes. The night sky here, away from city lights, is genuinely spectacular on clear evenings.</div>
          <div class="activity-travel">35 min drive; same D943 north through the Combe de Lourmarin</div>
        </div>

      </div>
    </div>
  </div>

  <div class="divider"><div class="divider-line"></div><span class="divider-text">Les ocres de Roussillon</span><div class="divider-line"></div></div>

  <!-- DAY 6 -->
  <div id="day6" class="day-block">
    <div class="day-label">
      <span class="day-number">06</span>
      <span class="day-name">Friday</span>
      <span class="day-date">June 12</span>
    </div>
    <div class="day-content">
      <div class="activity-list">

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-time">10:00 AM</span>
            <span class="activity-tag tag-travel">Drive</span>
          </div>
          <div class="activity-name">Gordes → Roussillon</div>
          <div class="activity-note">A twenty-minute drive northeast through the vineyards and cherry orchards of the Apt basin. In June, the cherry trees will be heavy with fruit, and the ochre-tinted soil begins to appear along the roadside as you approach Roussillon.</div>
          <div class="activity-travel">20 min drive, D2 northeast toward Apt, then D104 to Roussillon</div>
        </div>

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-time">10:30 AM</span>
            <span class="activity-tag tag-site">Walk</span>
          </div>
          <div class="activity-name">Sentier des Ocres — The Ochre Trail</div>
          <div class="activity-note">This is one of Provence's most extraordinary natural experiences. Roussillon sits atop the largest ochre deposit in the world — seventeen different shades of red, orange, amber, and yellow stain the cliffs and pathways of the Sentier des Ocres into something that looks more like the American Southwest than southern France. The short trail (30–45 min for the main loop) winds through formations of sculpted ochre stone, offering views across the Luberon that are genuinely breathtaking. Wear shoes you don't mind staining — the ochre dust is beautiful and extremely persistent.</div>
        </div>

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-tag tag-site">Viewpoint</span>
          </div>
          <div class="activity-name">Belvédère Basso — Ochre Valley Viewpoint</div>
          <div class="activity-note">A spectacular viewpoint at the edge of Roussillon with panoramic views across the ochre valley — GPS coordinates saved in your itinerary. An unmissable photograph and a grounding moment to take in the scale and color of the landscape.</div>
        </div>

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-time">12:30 PM</span>
            <span class="activity-tag tag-eat">Lunch</span>
          </div>
          <div class="activity-name">Lunch in Roussillon Village</div>
          <div class="activity-note">The village itself is lovely — buildings painted in coordinating shades of ochre by municipal decree, so the entire village glows in the afternoon light. Lunch at one of the village terraces overlooking the valley is the obvious choice. Look for a simple plat du jour: salade niçoise, grilled lamb, or a Provençal tart.</div>
        </div>

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-tag tag-shop">Explore</span>
          </div>
          <div class="activity-name">Wander Roussillon Village</div>
          <div class="activity-note">The village has a handful of excellent art galleries and craft shops — many artists are drawn here by the extraordinary light. The local pottery and ochre-pigmented artwork make for distinctive and genuinely non-generic souvenirs.</div>
        </div>

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-time">2:30 PM</span>
            <span class="activity-tag tag-drink">Optional</span>
            <span class="optional-badge">Optional</span>
          </div>
          <div class="activity-name">Wine Tasting — Area Domaines</div>
          <div class="activity-note">The area around Roussillon has several excellent domaines worth a tasting if the afternoon allows. AOC Luberon wines — particularly the whites and rosés — are underrated and delicious.</div>
        </div>

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-tag tag-travel">Optional Scenic Route</span>
            <span class="optional-badge">Optional</span>
          </div>
          <div class="activity-name">Scenic Loop: Roussillon → Bonnieux → Apt → Gordes</div>
          <div class="activity-note">If time and energy allow: the drive via Bonnieux and Apt adds about 60 minutes but takes you through the heart of the Luberon lavender country, through cherry orchards and thyme-scented garrigue. The D943 between Apt and Bonnieux is particularly beautiful in June.</div>
          <div class="activity-travel">~60 min total scenic loop vs. ~20 min direct return</div>
        </div>

        <div class="activity-item">
          <div class="activity-tag tag-relax">Afternoon</div>
          <div class="activity-name">Pool Time — Le Jas de Gordes</div>
          <div class="activity-note">The hotel pool with views across the Luberon valley. This is the afternoon for it. Sun, rosé, and the sound of cicadas.</div>
        </div>

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-time">7:00 PM</span>
            <span class="activity-tag tag-eat">Dinner</span>
          </div>
          <div class="activity-name">La Trinquette — Gordes (4.7⭐, 566 reviews)</div>
          <div class="activity-note">A modern tasting menu restaurant in Gordes — the evening's most elegant option. Highly rated and locally respected, La Trinquette offers a contemporary take on Provençal ingredients in a more refined format. Worth a reservation if you haven't yet dined here.</div>
        </div>

      </div>
    </div>
  </div>

  <div class="divider"><div class="divider-line"></div><span class="divider-text">Les Alpilles</span><div class="divider-line"></div></div>

  <!-- DAY 7 -->
  <div id="day7" class="day-block">
    <div class="day-label">
      <span class="day-number">07</span>
      <span class="day-name">Saturday</span>
      <span class="day-date">June 13</span>
    </div>
    <div class="day-content">
      <div class="activity-list">

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-time">11:00 AM</span>
            <span class="activity-tag tag-travel">Day Trip</span>
          </div>
          <div class="activity-name">Drive to Saint-Rémy-de-Provence</div>
          <div class="activity-note">A fifty-minute drive southwest into the Alpilles — a jagged chain of white limestone hills that rises abruptly from the flat Crau plain. Saint-Rémy is the most refined and cosmopolitan of the Alpilles towns: beautifully preserved, gently upmarket, and filled with excellent shops, galleries, and restaurants. Van Gogh voluntarily committed himself to the Saint-Paul-de-Mausole asylum here in 1889, and produced over 150 paintings during his year in Saint-Rémy — the views of olive groves and cypress trees you see from the road are exactly what he painted.</div>
          <div class="activity-travel">50 min drive: D2 south from Gordes toward Cavaillon, then D99 west toward Saint-Rémy</div>
        </div>

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-time">12:30 PM</span>
            <span class="activity-tag tag-eat">Lunch</span>
            <span class="reserved-badge">✓ Reservation Confirmed</span>
          </div>
          <div class="activity-name">L'Aile ou la Cuisse — Saint-Rémy-de-Provence</div>
          <div class="activity-note">A confirmed lunch reservation at one of Saint-Rémy's best-regarded tables. Excellent traditional French cooking in the heart of the old town — the kind of long, unhurried Saturday lunch that Provence is made for. Order the local lamb if it's on the menu, and do not skip the cheese course.</div>
        </div>

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-time">3:00 PM</span>
            <span class="activity-tag tag-shop">Explore</span>
          </div>
          <div class="activity-name">Saint-Rémy Wandering — Boutiques &amp; Cafés</div>
          <div class="activity-note">Saint-Rémy has the best shopping of any Provençal village on this itinerary: exceptional home goods, local ceramics, Provençal fabric and linens, high-quality food products (truffle oil, lavender soap, local honey). The Rue Carnot and Boulevard Mirabeau are the main shopping streets. The town's weekly market on Wednesday mornings is legendary — but Saturday afternoon is quiet enough to be deeply pleasant.</div>
        </div>

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-time">5:00 PM</span>
            <span class="activity-tag tag-travel">Return</span>
          </div>
          <div class="activity-name">Saint-Rémy → Gordes</div>
          <div class="activity-note">Fifty-minute return drive. Consider a brief stop at Les Antiques on the D5 just south of Saint-Rémy — a remarkably well-preserved Roman mausoleum and triumphal arch from the 1st century BC, standing alone in an olive field at the edge of town. A five-minute stop that adds genuine historical weight to the day.</div>
          <div class="activity-travel">50 min drive; reverse the morning route via D99 and D2</div>
        </div>

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-time">8:00 PM</span>
            <span class="activity-tag tag-eat">Dinner</span>
          </div>
          <div class="activity-name">Dinner — Gordes Village</div>
          <div class="activity-note">A final evening in Gordes — your last dinner in Provence. Options include Le Teston (casual, 04 32 50 21 74) for a relaxed evening, or Le Mas for something more special. Alternatively, the hotel itself may offer dining with those extraordinary valley views as the sun sets over the Luberon.</div>
        </div>

      </div>
    </div>
  </div>

  <div class="divider"><div class="divider-line"></div><span class="divider-text">Au revoir, Provence</span><div class="divider-line"></div></div>

  <!-- DAY 8 -->
  <div id="day8" class="day-block">
    <div class="day-label">
      <span class="day-number">08</span>
      <span class="day-name">Sunday</span>
      <span class="day-date">June 14</span>
    </div>
    <div class="day-content">
      <div class="activity-list">

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-time">7:00 AM</span>
            <span class="activity-tag tag-travel">Early Start</span>
          </div>
          <div class="activity-name">Gordes → Avignon TGV — Return Rental Car</div>
          <div class="activity-note">An early departure to return the car and catch the TGV. Allow 45–55 minutes for the drive, plus 20–30 minutes for the Hertz car return process. The Avignon TGV station is modern and easy to navigate; coffee and croissants are available at the station.</div>
          <div class="activity-travel">45–55 min drive: reverse of arrival route via D2 and D900 toward Avignon TGV</div>
        </div>

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-time">9:41 AM</span>
            <span class="activity-tag tag-travel">TGV</span>
            <span class="reserved-badge">✓ TGV INOUI #6112</span>
          </div>
          <div class="activity-name">Avignon → Paris Gare de Lyon</div>
          <div class="activity-note">TGV INOUI #6112, arriving Paris at 12:29 PM. A comfortable return journey — a good moment for a Provence debrief over coffee in the dining car.</div>
        </div>

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-time">12:29 PM</span>
            <span class="activity-tag tag-travel">Arrive Paris</span>
          </div>
          <div class="activity-name">Arrive Paris Gare de Lyon</div>
          <div class="activity-note">Back in Paris for one final afternoon and evening. The Marché des Enfants Rouges closes at 5 PM on Sundays — if you're quick from the station, it's reachable in time for a late lunch (about 35–40 min by Metro, Line 1 east then Line 8 north).</div>
        </div>

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-tag tag-eat">Late Lunch</span>
          </div>
          <div class="activity-name">Marché des Enfants Rouges (closes 5 PM Sunday)</div>
          <div class="activity-note">A fond return to where the trip began. The market will close at 5 PM — arrive by 4:30 PM for a last sandwich from Chez Alain Miam Miam or a bowl of something warm from one of the market's international stalls.</div>
        </div>

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-time">2:00 PM</span>
            <span class="activity-tag tag-sleep">Hotel</span>
          </div>
          <div class="activity-name">Check In — Ibis Paris Bastille Faubourg 11ème</div>
          <div class="activity-note">A comfortable base for the final night in Paris, right in the familiar 11th arrondissement. The Bastille neighborhood has excellent evening options — particularly for wine bars and casual restaurants.</div>
        </div>

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-time">6:00 PM</span>
            <span class="activity-tag tag-eat">Dinner</span>
          </div>
          <div class="activity-name">Final Paris Dinner</div>
          <div class="activity-note">One last Parisian dinner. The Bastille area and Place de la Bastille are well-served by bistros ranging from casual to refined. Consider a return to a neighborhood favorite, or simply follow your nose toward the best-looking chalkboard.</div>
        </div>

        <div class="activity-item">
          <div class="activity-meta">
            <span class="activity-time">8:00 PM</span>
            <span class="activity-tag tag-site">Evening</span>
          </div>
          <div class="activity-name">Seine River Cruise</div>
          <div class="activity-note">A perfect final-evening activity: Paris illuminated from the water. The Bateaux-Mouches and Bateaux Parisiens run evening cruises from around 8 PM, passing beneath all the great bridges — Pont de l'Alma, Pont Neuf, Pont des Arts — with the Eiffel Tower sparkling its light show at the top of each hour. One hour on the Seine at night is a genuinely lovely way to say goodbye to Paris.</div>
          <div class="activity-travel">Bastille → Seine embarkation points: ~20–30 min Metro or taxi</div>
        </div>

      </div>
    </div>
  </div>

</div>
</section>

<!-- ===================== LONDON ===================== -->
<section id="london">
<div class="container">

  <div class="chapter">
    <p class="chapter-eyebrow london">Epilogue</p>
    <h2 class="chapter-title">London,<br><em>a brief crossing</em></h2>
    <p class="chapter-desc">A few days across the Channel — Eurostar from Gare du Nord, arrival at St Pancras, and a city that couldn't be more different from Paris while sharing many of the same pleasures.</p>
  </div>

  <div class="logistics-box">
    <div class="logistics-title">London Travel Logistics</div>
    <div class="logistics-row">
      <span class="logistics-label">Eurostar — Paris Gare du Nord</span>
      <span class="logistics-value confirmed">Departs 10:12 AM, Mon June 15</span>
    </div>
    <div class="logistics-row">
      <span class="logistics-label">Arrives London St Pancras</span>
      <span class="logistics-value">11:30 AM (local time)</span>
    </div>
    <div class="logistics-row">
      <span class="logistics-label">Hotel — Moxy London Piccadilly Circus</span>
      <span class="logistics-value">Check in 3:00 PM</span>
    </div>
    <div class="logistics-row">
      <span class="logistics-label">Hotel — CitizenM London Bankside</span>
      <span class="logistics-value">Check in 2:00 PM, July 16</span>
    </div>
    <div class="logistics-row">
      <span class="logistics-label">Visa Application</span>
      <span class="logistics-value confirmed">#GBRORDP0UVW1DPMDJV0JCECO78IUINW</span>
    </div>
    <div class="logistics-row">
      <span class="logistics-label">Flight Home — Chicago</span>
      <span class="logistics-value">Departs Mon June 15, 12:00 PM</span>
    </div>
  </div>

  <div class="context-card">
    <h3 class="context-title">London Highlights — Bankside &amp; Beyond</h3>
    <p>The CitizenM Bankside puts you in one of London's most walkable and culturally rich neighborhoods. From the hotel: Tate Modern is a three-minute walk, the Millennium Bridge leads directly across the Thames to the dome of St. Paul's, and the South Bank promenade stretches east toward Borough Market and west toward Waterloo. The 12th Knot rooftop bar at the Sea Containers hotel has some of the best Thames views in London — a natural nightcap destination.</p>
    <p>Don't miss: Borough Market (one of the world's great food markets, open Thursday through Saturday), Dishoom in Covent Garden or Shoreditch (the Bombay café-style breakfast is legendary — queue worth it), and Fortnum &amp; Mason on Piccadilly for tea, preserves, and the most beautiful food hall in Britain.</p>
  </div>

  <div class="route-card">
    <div class="route-icon">🚶</div>
    <div>
      <div class="route-title">The Bankside Walk — A Perfect London Afternoon</div>
      <div class="route-desc">CitizenM Bankside → Tate Modern (free, world-class) → Millennium Bridge (pause for the St Paul's view) → St Paul's Cathedral → back south along the river → Sea Containers / South Bank promenade → 12th Knot or Lyaness bar for a nightcap.</div>
      <div class="route-time">~2–3 hours at a comfortable pace · All walking · No Metro needed</div>
    </div>
  </div>

</div>
</section>

<!-- RESERVATIONS SUMMARY -->
<section style="background: var(--warm-white); border-top: 0.5px solid var(--border); border-bottom: 0.5px solid var(--border); padding: 4rem 0; margin: 3rem 0;">
<div class="container">
  <p style="font-size: 11px; letter-spacing: 0.2em; text-transform: uppercase; color: var(--sage); margin-bottom: 1.5rem; font-weight: 500;">Complete Reservation Summary</p>
  <h3 style="font-family: 'Cormorant Garamond', serif; font-size: 2rem; font-weight: 300; margin-bottom: 2rem; color: var(--ink);">Everything Already Booked</h3>

  <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(260px, 1fr)); gap: 12px;">

    <div style="background: #EDF7ED; border: 0.5px solid #A5D6A7; border-radius: 12px; padding: 1.2rem;">
      <div style="font-size: 10px; font-weight: 600; letter-spacing: 0.1em; text-transform: uppercase; color: #2E7D32; margin-bottom: 0.5rem;">✓ Confirmed</div>
      <div style="font-weight: 500; font-size: 14px; color: var(--ink); margin-bottom: 2px;">Hotel Le Mareuil</div>
      <div style="font-size: 12px; color: var(--muted);">Paris, Jun 7–10 · 11th arrondissement</div>
    </div>

    <div style="background: #EDF7ED; border: 0.5px solid #A5D6A7; border-radius: 12px; padding: 1.2rem;">
      <div style="font-size: 10px; font-weight: 600; letter-spacing: 0.1em; text-transform: uppercase; color: #2E7D32; margin-bottom: 0.5rem;">✓ Confirmed</div>
      <div style="font-weight: 500; font-size: 14px; color: var(--ink); margin-bottom: 2px;">TGV INOUI #6107</div>
      <div style="font-size: 12px; color: var(--muted);">Paris Gare de Lyon → Avignon, Jun 10 · 9:38 AM</div>
    </div>

    <div style="background: #EDF7ED; border: 0.5px solid #A5D6A7; border-radius: 12px; padding: 1.2rem;">
      <div style="font-size: 10px; font-weight: 600; letter-spacing: 0.1em; text-transform: uppercase; color: #2E7D32; margin-bottom: 0.5rem;">✓ Confirmed</div>
      <div style="font-weight: 500; font-size: 14px; color: var(--ink); margin-bottom: 2px;">Hertz Rental Car</div>
      <div style="font-size: 12px; color: var(--muted);">Avignon TGV · Automatic · #L6023264298</div>
    </div>

    <div style="background: #EDF7ED; border: 0.5px solid #A5D6A7; border-radius: 12px; padding: 1.2rem;">
      <div style="font-size: 10px; font-weight: 600; letter-spacing: 0.1em; text-transform: uppercase; color: #2E7D32; margin-bottom: 0.5rem;">✓ Confirmed</div>
      <div style="font-weight: 500; font-size: 14px; color: var(--ink); margin-bottom: 2px;">Le Jas de Gordes</div>
      <div style="font-size: 12px; color: var(--muted);">Gordes, Jun 10–14 · 955 Route des Moines</div>
    </div>

    <div style="background: #EDF7ED; border: 0.5px solid #A5D6A7; border-radius: 12px; padding: 1.2rem;">
      <div style="font-size: 10px; font-weight: 600; letter-spacing: 0.1em; text-transform: uppercase; color: #2E7D32; margin-bottom: 0.5rem;">✓ Confirmed</div>
      <div style="font-weight: 500; font-size: 14px; color: var(--ink); margin-bottom: 2px;">Restaurant Mieux</div>
      <div style="font-size: 12px; color: var(--muted);">Paris · Mon Jun 8 · 8:00 PM</div>
    </div>

    <div style="background: #EDF7ED; border: 0.5px solid #A5D6A7; border-radius: 12px; padding: 1.2rem;">
      <div style="font-size: 10px; font-weight: 600; letter-spacing: 0.1em; text-transform: uppercase; color: #2E7D32; margin-bottom: 0.5rem;">✓ Confirmed</div>
      <div style="font-weight: 500; font-size: 14px; color: var(--ink); margin-bottom: 2px;">Musée d'Orsay</div>
      <div style="font-size: 12px; color: var(--muted);">Timed entry · Tue Jun 9 · 2:00 PM</div>
    </div>

    <div style="background: #EDF7ED; border: 0.5px solid #A5D6A7; border-radius: 12px; padding: 1.2rem;">
      <div style="font-size: 10px; font-weight: 600; letter-spacing: 0.1em; text-transform: uppercase; color: #2E7D32; margin-bottom: 0.5rem;">✓ Confirmed</div>
      <div style="font-weight: 500; font-size: 14px; color: var(--ink); margin-bottom: 2px;">Chez René (or Au Bourguignon du Marais)</div>
      <div style="font-size: 12px; color: var(--muted);">Paris · Tue Jun 9 · 7:30 PM</div>
    </div>

    <div style="background: #EDF7ED; border: 0.5px solid #A5D6A7; border-radius: 12px; padding: 1.2rem;">
      <div style="font-size: 10px; font-weight: 600; letter-spacing: 0.1em; text-transform: uppercase; color: #2E7D32; margin-bottom: 0.5rem;">✓ Confirmed</div>
      <div style="font-weight: 500; font-size: 14px; color: var(--ink); margin-bottom: 2px;">L'Outsider — Gordes</div>
      <div style="font-size: 12px; color: var(--muted);">Wed Jun 10 · 7:15 PM</div>
    </div>

    <div style="background: #EDF7ED; border: 0.5px solid #A5D6A7; border-radius: 12px; padding: 1.2rem;">
      <div style="font-size: 10px; font-weight: 600; letter-spacing: 0.1em; text-transform: uppercase; color: #2E7D32; margin-bottom: 0.5rem;">✓ Confirmed</div>
      <div style="font-weight: 500; font-size: 14px; color: var(--ink); margin-bottom: 2px;">Domaine de la Citadelle Wine Tasting</div>
      <div style="font-size: 12px; color: var(--muted);">Ménerbes · Thu Jun 11 · 1:00 PM</div>
    </div>

    <div style="background: #EDF7ED; border: 0.5px solid #A5D6A7; border-radius: 12px; padding: 1.2rem;">
      <div style="font-size: 10px; font-weight: 600; letter-spacing: 0.1em; text-transform: uppercase; color: #2E7D32; margin-bottom: 0.5rem;">✓ Confirmed</div>
      <div style="font-weight: 500; font-size: 14px; color: var(--ink); margin-bottom: 2px;">L'Aile ou la Cuisse — Saint-Rémy</div>
      <div style="font-size: 12px; color: var(--muted);">Sat Jun 13 · Lunch · 12:30 PM</div>
    </div>

    <div style="background: #EDF7ED; border: 0.5px solid #A5D6A7; border-radius: 12px; padding: 1.2rem;">
      <div style="font-size: 10px; font-weight: 600; letter-spacing: 0.1em; text-transform: uppercase; color: #2E7D32; margin-bottom: 0.5rem;">✓ Confirmed</div>
      <div style="font-weight: 500; font-size: 14px; color: var(--ink); margin-bottom: 2px;">TGV INOUI #6112</div>
      <div style="font-size: 12px; color: var(--muted);">Avignon → Paris · Sun Jun 14 · 9:41 AM</div>
    </div>

  </div>

  <div style="margin-top: 2rem; padding: 1.2rem; background: #FFF8E7; border: 0.5px solid #FFD54F; border-radius: 12px;">
    <p style="font-size: 11px; font-weight: 600; letter-spacing: 0.08em; text-transform: uppercase; color: #E65100; margin-bottom: 0.5rem;">Still To Book</p>
    <p style="font-size: 13px; color: #5D4037; line-height: 1.7;">
      • <strong>Notre-Dame tickets</strong> — Reserve timed entry online 2 days ahead (notredamedeparis.fr/en)<br>
      • <strong>Bouchon, Lourmarin</strong> — Call to reserve (4.8⭐, fills up fast in June)<br>
      • <strong>Le Mas, Gordes</strong> — Call to reserve if preferred over Bouchon<br>
      • <strong>Seine River Cruise</strong> — Book online same day or 1–2 days ahead (Bateaux-Mouches or Bateaux Parisiens)
    </p>
  </div>

</div>
</section>

<!-- FOOTER -->
<footer class="footer">
  <p class="footer-title">Bon voyage</p>
  <p class="footer-sub">France · June 2026 · A personal guide</p>
</footer>

</body>
</html>
