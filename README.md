# <!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>Bulls Nakhra | USF Bollywood Fusion Dance Team</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <style>
    :root {
      --green: #0c4b3b;
      --gold: #c79b28;
      --dark: #1f2730;
      --light: #e8f0df; /* soft greenish-light background */
      --card: #f8f5eb;
      --accent: #c06070;
      --max-width: 1100px;
      --radius: 10px;
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
      background: var(--light);
      color: var(--dark);
      line-height: 1.6;
    }

    a {
      color: inherit;
      text-decoration: none;
    }

    header {
      background: #ffffff;
      border-bottom: 1px solid rgba(0,0,0,0.08);
      position: sticky;
      top: 0;
      z-index: 100;
    }

    .nav {
      max-width: var(--max-width);
      margin: 0 auto;
      padding: 0.75rem 1.25rem;
      display: flex;
      align-items: center;
      justify-content: space-between;
    }

    .logo {
      font-weight: 800;
      letter-spacing: 0.08em;
      text-transform: uppercase;
      font-size: 0.9rem;
      display: flex;
      align-items: center;
      gap: 0.4rem;
      color: var(--dark);
    }

    .logo span {
      background: var(--green);
      color: #ffffff;
      padding: 0.15rem 0.35rem;
      border-radius: 999px;
      font-size: 0.7rem;
    }

    .nav-links {
      display: flex;
      gap: 1.25rem;
      font-size: 0.85rem;
    }

    .nav-links a {
      opacity: 0.8;
      transition: opacity 0.2s, transform 0.2s;
    }

    .nav-links a:hover {
      opacity: 1;
      transform: translateY(-1px);
    }

    .hero {
      max-width: var(--max-width);
      margin: 0 auto;
      padding: 2.5rem 1.25rem 2rem;
      display: grid;
      grid-template-columns: minmax(0, 1.6fr) minmax(0, 1.2fr);
      gap: 2.5rem;
      align-items: center;
    }

    .hero-tag {
      text-transform: uppercase;
      letter-spacing: 0.12em;
      font-size: 0.7rem;
      color: var(--green);
      font-weight: 600;
      margin-bottom: 0.75rem;
    }

    .hero h1 {
      font-size: 2.3rem;
      line-height: 1.1;
      margin-bottom: 1rem;
      color: #1b242c;
    }

    .hero h1 span {
      color: var(--gold);
    }

    .hero-text {
      font-size: 0.95rem;
      opacity: 0.95;
      margin-bottom: 1.5rem;
    }

    .hero-buttons {
      display: flex;
      gap: 0.75rem;
      flex-wrap: wrap;
      margin-bottom: 1.5rem;
    }

    .btn {
      border-radius: 999px;
      padding: 0.6rem 1.3rem;
      font-size: 0.85rem;
      border: none;
      cursor: pointer;
      display: inline-flex;
      align-items: center;
      gap: 0.4rem;
      font-weight: 600;
      transition: transform 0.2s, box-shadow 0.2s, background 0.2s, color 0.2s;
      text-decoration: none;
      font-family: inherit;
    }

    .btn-primary {
      background: var(--green);
      color: #ffffff;
      box-shadow: 0 8px 18px rgba(0,0,0,0.18);
    }

    .btn-primary:hover {
      transform: translateY(-1px);
      box-shadow: 0 10px 22px rgba(0,0,0,0.22);
    }

    .btn-outline {
      background: transparent;
      border: 1px solid rgba(0,0,0,0.18);
      color: var(--dark);
    }

    .btn-outline:hover {
      background: rgba(0,0,0,0.03);
    }

    .hero-meta {
      display: flex;
      flex-wrap: wrap;
      gap: 1rem;
      font-size: 0.8rem;
      opacity: 0.9;
    }

    .hero-meta span {
      display: inline-flex;
      align-items: center;
      gap: 0.3rem;
    }

    .hero-card {
      background: var(--card);
      border-radius: var(--radius);
      padding: 1.4rem 1.6rem;
      border: 1px solid rgba(0,0,0,0.06);
      box-shadow: 0 16px 30px rgba(0,0,0,0.06);
    }

    .hero-card h2 {
      font-size: 1.05rem;
      margin-bottom: 0.7rem;
      color: #222b34;
    }

    .hero-card p {
      font-size: 0.85rem;
      opacity: 0.95;
      margin-bottom: 0.8rem;
    }

    .hero-badges {
      display: flex;
      flex-wrap: wrap;
      gap: 0.5rem;
      margin-top: 0.4rem;
    }

    .badge {
      font-size: 0.75rem;
      padding: 0.25rem 0.6rem;
      border-radius: 999px;
      border: 1px solid rgba(0,0,0,0.14);
      opacity: 0.9;
      background: #f1ecdf;
    }

    main {
      background: var(--light);
    }

    section {
      max-width: var(--max-width);
      margin: 0 auto;
      padding: 2rem 1.25rem;
      border-top: 1px solid rgba(0,0,0,0.04);
    }

    section:nth-of-type(odd) {
      background: #f3efe5;
    }

    .section-header {
      margin-bottom: 1.2rem;
    }

    .section-header h2 {
      font-size: 1.35rem;
      margin-bottom: 0.25rem;
      color: #1f2730;
    }

    .section-header p {
      font-size: 0.85rem;
      opacity: 0.85;
    }

    .two-column {
      display: grid;
      grid-template-columns: minmax(0, 1.3fr) minmax(0, 1.1fr);
      gap: 2rem;
      align-items: flex-start;
    }

    .about-text p {
      font-size: 0.9rem;
      margin-bottom: 0.7rem;
      opacity: 0.95;
    }

    .stat-grid {
      display: grid;
      grid-template-columns: repeat(3, minmax(0, 1fr));
      gap: 0.75rem;
      margin-top: 1rem;
    }

    .stat {
      background: #ffffff;
      border-radius: var(--radius);
      padding: 0.7rem 0.8rem;
      border: 1px solid rgba(0,0,0,0.06);
      text-align: left;
      box-shadow: 0 6px 14px rgba(0,0,0,0.04);
    }

    .stat-number {
      font-size: 1rem;
      font-weight: 700;
      color: var(--green);
    }

    .stat-label {
      font-size: 0.75rem;
      opacity: 0.85;
    }

    .values-list {
      list-style: none;
      font-size: 0.9rem;
    }

    .values-list li {
      margin-bottom: 0.6rem;
    }

    .values-list span {
      font-weight: 600;
      color: var(--green);
    }

    .grid-3 {
      display: grid;
      grid-template-columns: repeat(3, minmax(0, 1fr));
      gap: 1rem;
    }

    .card {
      background: #ffffff;
      border-radius: var(--radius);
      border: 1px solid rgba(0,0,0,0.06);
      padding: 0.9rem;
      font-size: 0.85rem;
      box-shadow: 0 8px 18px rgba(0,0,0,0.04);
    }

    .card h3 {
      font-size: 0.95rem;
      margin-bottom: 0.4rem;
      color: #232b34;
    }

    .card p {
      font-size: 0.82rem;
      opacity: 0.94;
    }

    .highlight {
      color: var(--gold);
      font-weight: 600;
    }

    .callout {
      background: #f1ecdf;
      border-radius: var(--radius);
      padding: 1rem;
      font-size: 0.85rem;
      border: 1px solid rgba(0,0,0,0.06);
    }

    .callout strong {
      color: var(--green);
    }

    .footer {
      max-width: var(--max-width);
      margin: 0 auto;
      padding: 1.5rem 1.25rem 2rem;
      font-size: 0.75rem;
      display: flex;
      flex-wrap: wrap;
      justify-content: space-between;
      gap: 0.75rem;
      opacity: 0.8;
      color: #444b52;
    }

    .footer a {
      text-decoration: underline;
      text-decoration-thickness: 1px;
      text-underline-offset: 2px;
    }

    @media (max-width: 800px) {
      .hero {
        grid-template-columns: minmax(0, 1fr);
      }

      .hero {
        padding-top: 1.75rem;
      }

      .hero h1 {
        font-size: 2rem;
      }

      .two-column,
      .grid-3 {
        grid-template-columns: minmax(0, 1fr);
      }

      .stat-grid {
        grid-template-columns: repeat(2, minmax(0, 1fr));
      }

      .nav-links {
        display: none;
      }
    }

    @media (max-width: 500px) {
      .stat-grid {
        grid-template-columns: minmax(0, 1fr);
      }
    }
  </style>
</head>
<body>
  <header>
    <div class="nav">
      <div class="logo">
        <span>USF</span> Bulls Nakhra
      </div>
      <nav class="nav-links">
        <a href="#about">About</a>
        <a href="#culture">Culture</a>
        <a href="#performances">Performances</a>
        <a href="#join">Join</a>
        <a href="#leadership">Leadership</a>
        <a href="#contact">Contact</a>
      </nav>
    </div>
  </header>

  <main>
    <!-- HERO -->
    <section class="hero">
      <div>
        <div class="hero-tag">USF Bollywood Fusion Dance</div>
        <h1>
          Where <span>Bollywood</span> meets<br />
          community, competition, and story.
        </h1>
        <p class="hero-text">
          Bulls Nakhra is the University of South Florida’s premier competitive co‑ed Bollywood fusion dance team,
          blending the energy of Bollywood with contemporary and global styles to create dynamic, story‑driven performances
          on stage and in the community.
        </p>
        <div class="hero-buttons">
          <a href="#join" class="btn btn-primary">Join the Team</a>
          <a href="#contact" class="btn btn-outline">Book a Performance</a>
        </div>
        <div class="hero-meta">
          <span>🎭 Competitive Bollywood Fusion</span>
          <span>🌎 Multicultural & Inclusive</span>
          <span>🤝 Performance & Outreach</span>
        </div>
      </div>

      <div class="hero-card">
        <h2>More than a dance team.</h2>
        <p>
          We are a cultural and artistic home for dancers of all backgrounds, dedicated to technical excellence, creative
          expression, and celebrating South Asian heritage through movement.
        </p>
        <p>
          Beyond competition, Bulls Nakhra strives to build community on campus and beyond, collaborating with campus
          organizations and non-profits, performing at multicultural events, and using dance as a platform for
          representation, advocacy, and belonging.
        </p>
        <div class="hero-badges">
          <div class="badge">Bollywood • Bhangra • Semi • Fusion</div>
          <div class="badge">USF Student Organization</div>
          <div class="badge">Performance & Competition Team</div>
        </div>
      </div>
    </section>

    <!-- ABOUT -->
    <section id="about">
      <div class="section-header">
        <h2>About Bulls Nakhra</h2>
        <p>Who we are, what we do, and why we dance.</p>
      </div>
      <div class="two-column">
        <div class="about-text">
          <p>
            Bulls Nakhra brings together students from across disciplines and backgrounds who share a love for
            Bollywood, fusion, and storytelling through movement. We take pride in crafting sets that balance
            technical choreography, clean formations, and expressive performance.
          </p>
          <p>
            Our members train in a range of styles—from Bollywood and semi‑classical to hip‑hop and other global
            influences—allowing us to experiment with creative concepts and narratives that feel both rooted and fresh.
          </p>
          <p>
            Whether we are on a competition stage, at a cultural showcase, or performing for a cause, our goal is the
            same: to bring people together, represent South Asian culture with pride, and leave audiences feeling the
            joy we feel when we dance.
          </p>
          <div class="callout">
            <strong>Our mission:</strong> Use dance as a space for cultural celebration, discipline, and community care—on
            and off the stage.
          </div>
        </div>
        <div>
          <div class="stat-grid">
            <div class="stat">
              <div class="stat-number">20+ </div>
              <div class="stat-label">Active members (co‑ed, all levels)</div>
            </div>
            <div class="stat">
              <div class="stat-number">15+ </div>
              <div class="stat-label">Routines taught & performed each year</div>
            </div>
            <div class="stat">
              <div class="stat-number">Multiple</div>
              <div class="stat-label">Campus & community collaborations</div>
            </div>
          </div>
          <ul class="values-list" style="margin-top:1rem;">
            <li><span>We train hard:</span> Clean lines, stamina, and accountability to the team.</li>
            <li><span>We lead with heart:</span> Supportive, inclusive rehearsals where dancers can grow.</li>
            <li><span>We give back:</span> Performances and events that uplift causes and communities.</li>
          </ul>
        </div>
      </div>
    </section>

    <!-- CULTURE -->
    <section id="culture">
      <div class="section-header">
        <h2>Team Culture & Values</h2>
        <p>How we move together, on and off the stage.</p>
      </div>
      <div class="grid-3">
        <div class="card">
          <h3>Community & Belongings</h3>
          <p>
            Rehearsals are as much about connection as they are about choreography. We invest in bonding, mentorship, and
            a team culture where everyone feels seen, valued, and supported.
          </p>
        </div>
        <div class="card">
          <h3>Growth & Excellence</h3>
          <p>
            From first‑time performers to experienced dancers, we challenge each other to grow through feedback, reps, and
            intentional practice—always balancing high standards with encouragement.
          </p>
        </div>
        <div class="card">
          <h3>Representation & Advocacy</h3>
          <p>
            As a South Asian–rooted team, we treat our culture with respect while staying open to fusion and collaboration.
            We use performances and events to highlight stories, causes, and voices that matter.
          </p>
        </div>
      </div>
    </section>

    <!-- PERFORMANCES -->
    <section id="performances">
      <div class="section-header">
        <h2>Performances & Events</h2>
        <p>From campus stages to community spotlights.</p>
      </div>
      <div class="two-column">
        <div>
          <p style="font-size:0.9rem; margin-bottom:0.7rem;">
            Bulls Nakhra performs at a wide range of events throughout the year, including:
          </p>
          <ul class="values-list">
            <li><span>Signature events:</span> Naach 'n Nachos, Multicultural Fair (in partnership with DesiBullZ and GUYSA), Galentines, Senior Send‑Off, and Grand Callbacks.</li>
            <li><span>Campus programs:</span> Cultural nights, showcases, and collaborations with USF student organizations.</li>
            <li><span>Community outreach:</span> Performances and appearances that support causes, representation, and multicultural engagement.</li>
          </ul>
          <p style="font-size:0.9rem; margin-top:0.7rem;">
            We also hold weekly practices to prepare for performances, refine choreography, and build the chemistry that shows up on stage.
          </p>
        </div>
        <div class="callout">
          <strong>Interested in booking Bulls Nakhra?</strong><br />
          We can tailor performances in length and style (Bollywood, semi‑classical, fusion, concept pieces) to fit your
          event. Reach out through the contact section below with your date, venue, and vision.
        </div>
      </div>
    </section>

    <!-- JOIN -->
    <section id="join">
      <div class="section-header">
        <h2>Join Bulls Nakhra</h2>
        <p>For dancers who want more than just choreography.</p>
      </div>
      <div class="two-column">
        <div>
          <p style="font-size:0.9rem; margin-bottom:0.7rem;">
            We hold auditions at the beginning of the academic year and occasionally mid‑year, depending on team needs.
            Dancers of all experience levels and backgrounds are welcome to audition.
          </p>
          <ul class="values-list">
            <li><span>Who we’re looking for:</span> Committed, coachable dancers who care about both performance and community.</li>
            <li><span>What to expect:</span> Choreography to learn, across styles, plus a chance to show your personality and presence.</li>
            <li><span>Time commitment:</span> Regular rehearsals, tech runs, and performances throughout the semester.</li>
          </ul>
        </div>
        <div class="callout">
          <strong>Stay connected:</strong><br />
          Follow us on social media for audition announcements, performance clips, and behind‑the‑scenes looks at team life.<br /><br />
          Instagram: <em>@bullsnakhra</em><br />
          TikTok: <em>@bullsnakhra</em><br />
          BullsConnect: Search for “Bulls Nakhra”
        </div>
      </div>
    </section>

    <!-- LEADERSHIP -->
    <section id="leadership">
      <div class="section-header">
        <h2>Leadership</h2>
        <p>The team behind the team.</p>
      </div>
      <div class="two-column">
        <div>
          <p style="font-size:0.9rem;">
            Bulls Nakhra is guided by a dedicated leadership team that balances artistic vision, organization,
            and community care.
          </p>
          <ul class="values-list" style="margin-top:0.7rem;">
            <li><span>Advisor:</span> Arsheya Kak</li>
            <li><span>Captains:</span> Aditi Turkar, Khushi Shah, and Meenakshi Sankaran</li>
          </ul>
        </div>
        <div class="callout">
          <strong>What leadership means to us:</strong><br />
          Holding our dancers to a high standard while creating a supportive, inclusive space where everyone can grow,
          experiment, and find their voice on stage.
        </div>
      </div>
    </section>

    <!-- CONTACT -->
    <section id="contact">
      <div class="section-header">
        <h2>Contact & Bookings</h2>
        <p>We’d love to dance with you.</p>
      </div>
      <div class="two-column">
        <div>
          <p style="font-size:0.9rem; margin-bottom:0.6rem;">
            For bookings, collaborations, or questions about the team, reach out using the details below:
          </p>
          <ul class="values-list">
            <li><span>Email:</span> bullsnakhra@gmail.com</li>
            <li><span>Instagram DMs:</span> @bullsnakhra</li>
            <li><span>BullsConnect:</span> Message our e‑board through the Bulls Nakhra page</li>
          </ul>
          <p style="font-size:0.9rem; margin-top:0.7rem;">
            We’re happy to discuss performance requests, workshops, and multicultural programming ideas.
          </p>
        </div>
        <div class="callout">
          <strong>Want to support the team?</strong><br />
          Ask us about sponsorships, donations, or partnership opportunities to help fund costumes, travel, and
          competition fees, and to keep South Asian arts thriving at USF.
        </div>
      </div>
    </section>
  </main>

  <footer class="footer">
    <div>© Bulls Nakhra – University of South Florida.</div>
    <div>Site content managed by the Bulls Nakhra Executive Board.</div>
  </footer>
</body>
</html>
