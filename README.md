<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>EduPlatform - Learn, Grow, Succeed</title>
  <link href="https://fonts.googleapis.com/css?family=Inter:400,600&display=swap" rel="stylesheet"/>
  <style>
    :root {
      --primary: #2867b2;
      --accent: #ffe066;
      --light: #f7fafc;
      --dark: #22223b;
      --success: #42b883;
      --border: #e2e8f0;
    }
    * { box-sizing: border-box; }
    body {
      margin: 0;
      font-family: 'Inter', Arial, sans-serif;
      background: var(--light);
      color: var(--dark);
      line-height: 1.6;
    }
    header {
      background: var(--primary);
      color: #fff;
      padding: 0;
      margin-bottom: 0;
    }
    .navbar {
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 1rem 2rem;
      max-width: 1200px;
      margin: auto;
    }
    .logo {
      font-size: 1.7rem;
      font-weight: 700;
      letter-spacing: 1px;
    }
    nav ul {
      list-style: none;
      display: flex;
      gap: 1.5rem;
      padding: 0;
      margin: 0;
    }
    nav a {
      color: #fff;
      text-decoration: none;
      font-weight: 600;
      transition: color 0.2s;
    }
    nav a:hover { color: var(--accent); }
    .hero {
      padding: 3rem 1rem 2rem 1rem;
      text-align: center;
      background: linear-gradient(90deg, var(--primary) 70%, var(--success) 100%);
      color: #fff;
    }
    .hero h1 {
      font-size: 2.6rem;
      margin: 0 0 1rem;
      font-weight: 700;
    }
    .hero p {
      font-size: 1.25rem;
      margin-bottom: 2rem;
    }
    .hero .cta-btn {
      background: var(--accent);
      color: var(--dark);
      padding: 0.9em 2em;
      border: none;
      border-radius: 30px;
      font-size: 1.1rem;
      font-weight: 600;
      box-shadow: 0 2px 10px #0001;
      cursor: pointer;
      transition: background 0.2s;
      margin: 0.2rem;
    }
    .hero .cta-btn:hover { background: #ffd23f; }
    .sections {
      max-width: 1200px;
      margin: 2rem auto;
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
      gap: 2rem;
      padding: 0 1rem;
    }
    .card {
      background: #fff;
      border-radius: 14px;
      box-shadow: 0 2px 8px #0002;
      padding: 1.5rem 1.2rem;
      text-align: left;
      border: 1px solid var(--border);
      display: flex;
      flex-direction: column;
      min-height: 260px;
    }
    .card h2 {
      font-size: 1.3rem;
      margin-bottom: 0.6em;
      color: var(--primary);
    }
    .card .card-action {
      margin-top: auto;
      text-align: right;
    }
    .card .link {
      color: var(--success);
      font-weight: 600;
      text-decoration: none;
    }
    .card .link:hover { text-decoration: underline; }
    .dashboard {
      background: var(--primary);
      color: #fff;
      border-radius: 14px;
      box-shadow: 0 2px 8px #0002;
      padding: 1.5rem 1.2rem;
      min-height: 260px;
      display: flex;
      flex-direction: column;
    }
    .dashboard h2 {
      color: var(--accent);
      margin-bottom: 0.6em;
    }
    .progress-bar-bg {
      background: #fff2;
      border-radius: 10px;
      height: 16px;
      width: 100%;
      margin: 0.5em 0;
    }
    .progress-bar {
      background: var(--accent);
      height: 100%;
      border-radius: 10px;
      width: 60%;
      transition: width 0.4s;
    }
    .dashboard .profile-link {
      color: var(--accent);
      text-decoration: underline;
      margin-top: auto;
      align-self: flex-end;
    }
    /* Responsive */
    @media (max-width: 700px) {
      .navbar { flex-direction: column; gap: 1rem; }
      .sections { grid-template-columns: 1fr; }
    }
    /* Forums, polls, comments preview */
    .community-tools {
      display: flex;
      gap: 1.5rem;
      flex-wrap: wrap;
      margin-top: 1.5rem;
    }
    .community-tool {
      background: #fff;
      border: 1px solid var(--border);
      border-radius: 10px;
      padding: 1em;
      flex: 1;
      min-width: 180px;
      box-shadow: 0 1px 4px #0001;
    }
    .community-tool h3 {
      font-size: 1.1em;
      color: var(--primary);
      margin: 0 0 0.5em;
    }
    footer {
      background: #22223b;
      color: #fff;
      text-align: center;
      padding: 2em 1em 1em 1em;
      margin-top: 3em;
    }
    .footer-links {
      display: flex;
      justify-content: center;
      gap: 2em;
      flex-wrap: wrap;
      margin-bottom: 1em;
    }
    .footer-links a {
      color: #ffe066;
      text-decoration: none;
      font-size: 1em;
      margin: 0 0.4em;
    }
    .footer-links a:hover { text-decoration: underline; }
  </style>
</head>
<body>
  <header>
    <div class="navbar">
      <div class="logo">EduPlatform</div>
      <nav>
        <ul>
          <li><a href="#">Courses</a></li>
          <li><a href="#">Articles</a></li>
          <li><a href="#">Videos</a></li>
          <li><a href="#">Quizzes</a></li>
          <li><a href="#">Community</a></li>
          <li><a href="#">Login/Register</a></li>
        </ul>
      </nav>
    </div>
    <section class="hero">
      <h1>Modern Learning for Everyone</h1>
      <p>Engaging courses, interactive tools, and a vibrant community for students & teachers. Track your progress, join discussions, and unlock your potential!</p>
      <button class="cta-btn">Browse Courses</button>
      <button class="cta-btn">Join Now</button>
    </section>
  </header>
  <main>
    <div class="sections">
      <div class="dashboard">
        <h2>Welcome, [Your Name]</h2>
        <div>Learning Progress</div>
        <div class="progress-bar-bg">
          <div class="progress-bar" style="width:60%"></div>
        </div>
        <div style="font-size:0.95em; margin:0.5em 0 1em 0;">
          3 Courses in progress<br>Last completed: "Introduction to Science"
        </div>
        <a href="#" class="profile-link">Go to your dashboard</a>
      </div>
      <div class="card">
        <h2>Courses</h2>
        <p>Explore a variety of interactive courses in math, science, language, and more. Filter by grade or interest.</p>
        <div class="card-action">
          <a href="#" class="link">See all courses →</a>
        </div>
      </div>
      <div class="card">
        <h2>Articles</h2>
        <p>Read expert-written articles, tips, and guides to help you and your students thrive.</p>
        <div class="card-action">
          <a href="#" class="link">Browse articles →</a>
        </div>
      </div>
      <div class="card">
        <h2>Videos</h2>
        <p>Watch engaging video lessons from top educators and subject experts.</p>
        <div class="card-action">
          <a href="#" class="link">Watch videos →</a>
        </div>
      </div>
      <div class="card">
        <h2>Quizzes</h2>
        <p>Test your knowledge and track your progress with fun, interactive quizzes.</p>
        <div class="card-action">
          <a href="#" class="link">Take a quiz →</a>
        </div>
      </div>
    </div>
    <div class="sections" style="margin-top:0;">
      <div class="card" style="grid-column: span 2;">
        <h2>Community & Tools</h2>
        <div class="community-tools">
          <div class="community-tool">
            <h3>Forums</h3>
            <p>Ask questions, help others, and join discussions with peers and teachers.</p>
            <a href="#" class="link">Visit Forum</a>
          </div>
          <div class="community-tool">
            <h3>Comments</h3>
            <p>Share your thoughts and feedback on courses, videos, and articles.</p>
          </div>
          <div class="community-tool">
            <h3>Polls</h3>
            <p>Participate in polls & surveys. Shape the learning community!</p>
            <a href="#" class="link">Take a Poll</a>
          </div>
        </div>
      </div>
    </div>
  </main>
  <footer>
    <div class="footer-links">
      <a href="#">About</a> |
      <a href="#">Contact</a> |
      <a href="#">FAQ</a> |
      <a href="#">Privacy Policy</a>
    </div>
    <div>© 2025 EduPlatform. All rights reserved.</div>
  </footer>
</body>
</html>
