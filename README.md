<!-- Paste this into your README.md -->
<style>
  /* Reset & base */
  .bento { 
    box-sizing: border-box;
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial;
    color: #000;
    background: #fff;
    max-width: 900px;
    margin: 0 auto;
    padding: 24px;
  }

  /* Grid: large tile on the left, three stacked tiles on the right */
  .bento-grid {
    display: grid;
    grid-template-columns: 2fr 1fr;
    grid-template-rows: auto auto auto;
    gap: 16px;
  }

  .card {
    border: 1px solid #000;
    padding: 18px;
    border-radius: 8px;
    background: #fff;
  }

  .hero {
    grid-row: 1 / span 3; /* spans all rows on the left */
    display: flex;
    flex-direction: column;
    justify-content: center;
    gap: 8px;
  }

  h1, h2 {
    margin: 0;
    font-weight: 700;
  }

  h1 { font-size: 22px; }
  h2 { font-size: 14px; margin-bottom: 8px; }

  p, li {
    margin: 0;
    font-size: 13px;
    line-height: 1.4;
  }

  ul { padding-left: 16px; margin-top: 8px; }

  .meta {
    color: #000;
    opacity: 0.85;
    font-size: 13px;
  }

  .links a {
    color: #000;
    text-decoration: none;
    border-bottom: 1px dashed #000;
    font-size: 13px;
  }

  /* Small helper for compact lists */
  .compact-list li { margin-bottom: 6px; }

  /* Responsive: stack on narrow screens */
  @media (max-width: 720px) {
    .bento-grid {
      grid-template-columns: 1fr;
      grid-template-rows: auto;
    }
    .hero { grid-row: auto; }
  }
</style>

<div class="bento">
  <div class="bento-grid">
    <!-- Large left tile: About / Summary -->
    <div class="card hero">
      <div>
        <h1>Neil Pascual</h1>
        <p class="meta">Web Developer — building clean, user-first web apps</p>
      </div>
      <div style="margin-top:12px;">
        <p>A pragmatic developer focused on readable code, simple design, and reliable user experiences. Strong experience with React, Node.js, and relational databases.</p>
      </div>
      <div style="margin-top:12px;" class="links">
        <p class="meta">Email: <a href="mailto:neilpascual@example.com">neilpascual@example.com</a></p>
        <p class="meta">GitHub: <a href="https://github.com/neilpascual" target="_blank">github.com/neilpascual</a></p>
      </div>
    </div>
    <!-- Top-right tile: Experience -->
    <div class="card">
      <h2>Experience</h2>
      <ul class="compact-list">
        <li><strong>Frontend Developer</strong> — Freelance / Project-based<br><span class="meta">2023 – Present</span></li>
        <li style="margin-top:8px;"><strong>Intern Developer</strong> — [Company / Project]<br><span class="meta">2022 – 2023</span></li>
      </ul>
    </div>
    <!-- Middle-right tile: Skills -->
    <div class="card">
      <h2>Skills</h2>
      <ul class="compact-list">
        <li><strong>Frontend:</strong> React, JavaScript (ES6+), HTML, CSS, Tailwind</li>
        <li><strong>Backend:</strong> Node.js, Express</li>
        <li><strong>DB:</strong> MySQL, Sequelize</li>
        <li><strong>Tools:</strong> Git, VS Code, Postman</li>
      </ul>
    </div>
    <!-- Bottom-right tile: Projects (short) -->
    <div class="card">
      <h2>Selected Projects</h2>
      <ul class="compact-list">
        <li><strong>Test App</strong> — Quiz & timed-test platform for applicants.<br><a href="#" class="meta">View repo</a></li>
        <li style="margin-top:8px;"><strong>Suitelifer</strong> — Property management / booking system.<br><a href="#" class="meta">View repo</a></li>
      </ul>
    </div>
  </div>
</div>
