<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Business Analytics Portfolio</title>
  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; scroll-behavior: smooth; }
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background: #f5f7fa;
      color: #333;
      transition: background 0.3s, color 0.3s;
    }
    body.dark { background: #1c1c1c; color: #eee; }
    body.dark nav, body.dark footer { background: #111; }
    body.dark .card { background: #2a2a2a; color: #eee; }
    body.dark h2, body.dark .card-content h3 { color: #ffda47; }

    nav {
      background: #004aad;
      padding: 15px 40px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      position: sticky;
      top: 0;
      z-index: 1000;
    }
    nav h2 { color: white; }
    nav ul { list-style: none; display: flex; gap: 20px; }
    nav ul li a {
      color: white; text-decoration: none; font-weight: bold; transition: 0.3s;
    }
    nav ul li a:hover { color: #ffda47; }

    .btn {
      background: white;
      color: #004aad;
      border: none;
      padding: 8px 16px;
      border-radius: 20px;
      cursor: pointer;
      font-weight: bold;
      transition: 0.3s;
    }
    .btn:hover { background: #ffda47; color: #000; }

    .hero {
      text-align: center;
      padding: 70px 20px;
      background: linear-gradient(to right, #004aad, #0073e6);
      color: white;
    }
    .hero img {
      width: 150px; height: 150px;
      border-radius: 50%; border: 4px solid white;
      margin-bottom: 20px;
    }
    .hero h1 { font-size: 2.5em; }
    .hero p { font-size: 1.1em; }

    .personal-statement {
      max-width: 800px;
      margin: 20px auto 0;
      font-size: 1.05em;
      line-height: 1.6;
      text-align: justify;
      background: #ffffff; 
      color: #000;         
      padding: 20px;
      border-radius: 12px;
      page-break-inside: avoid;
    }

    section {
      max-width: 1100px;
      margin: auto;
      padding: 60px 20px;
    }
    h2 { color: #004aad; margin-bottom: 20px; text-align: center; font-size: 2em; }

    .card-container {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 20px;
    }
    .card {
      background: white;
      border-radius: 12px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.1);
      overflow: hidden;
      transition: transform 0.3s, box-shadow 0.3s;
    }
    .card:hover { transform: translateY(-5px); box-shadow: 0 6px 16px rgba(0,0,0,0.15); }
    .card img { width: 100%; height: 180px; object-fit: cover; }
    .card-content { padding: 20px; }
    .card-content h3 { color: #004aad; margin-bottom: 10px; }
    .card-content p { font-size: 0.95em; }

    .skills {
      display: flex; flex-wrap: wrap; justify-content: center;
      gap: 15px; margin-top: 20px;
    }
    .skill {
      background: #004aad; color: white;
      padding: 10px 20px; border-radius: 20px; font-size: 0.9em;
    }

    footer {
      background: #004aad; color: white;
      text-align: center; padding: 20px; margin-top: 40px;
    }
  </style>
</head>
<body>

  <nav>
    <h2>My Portfolio</h2>
    <ul>
      <li><a href="#about">About</a></li>
      <li><a href="#achievements">Achievements</a></li>
      <li><a href="#projects">Projects</a></li>
      <li><a href="#skills">Skills</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
    <div>
      <button class="btn" onclick="toggleDarkMode()">🌙 Dark</button>
      <button class="btn" onclick="downloadPDF()">⬇️ PDF</button>
    </div>
  </nav>

  <section class="hero" id="about">
    <h1>Maxx Reinhart Leong</h1>
    <p>Prospective Business Analytics Student | Passionate about Data & Decision-Making</p>
    <p>Email: maxxleong904@gmail.com | Phone: +62 811-631-0905</p>

    <div class="personal-statement">
      <p>
        I am currently pursuing my education as a senior high 3 student in Methodist Charles Wesley, Medan.
        I have a strong interest in business and technology, and i am pursuing a furture in Business Analytics.
        Through out my academic journey, I have consistently ranked in the top 1-3 of my class. I also have a
        strong sense of leadership and able to work with everyone well.
      </p>
    </div>
  </section>

    <section id="education">
    <h2>Education</h2>
    <div class="card-container">
      <div class="card">
        <div class="card-content">
          <h3>Senior High School(2023-2026) –</h3>
          <p>Methodist Charles Wesley</p>
          <h3>Junior High School(2020-2023) –</h3>
          <p>Methodist Charles Wesley</p>
          <h3>Primary(2014-2020) –</h3>
          <p>Singapore International Academy</p>
        </div>
      </div>
    </section>
  <section id="achievements">
    <h2>Academic Achievements</h2>
    <div class="card-container">
      <div class="card">
        <div class="card-content">
          <h3>The 2nd Top Achiever of Junior High Level 2023 Methodist Charles Wesley –</h3>
          <p>Developed critical thinking and problem solving skills.</p>
        </div>
      </div>
      <div class="card">
        <div class="card-content">
          <h3>2nd place in Esports Mobile Legends</h3>
          <p>Developed leadership and critical thinking.</p>
        </div>
      </div>
    </div>
  </section>

  <section id="projects">
    <h2>Projects & Research</h2>
    <div class="card-container">
      <div class="card">
        <div class="card-content">
          <h3>Data Analysis From Kaggle</h3>
          <p>Analyzed company data to identify SWOT of a company.</p>
        </div>
      </div>
    </div>
  </section>

  <section id="skills">
    <h2>Skills & Certifications</h2>
    <div class="skills">
      <div class="skill">Python</div>
      <div class="skill">SQL</div>
      <div class="skill">PHP</div>
      <div class="skill">MS Word</div>
      <div class="skill">MS Excel</div>
      <div class="skill">MS Powerpoint</div>
      <div class="skill">IELTS Certified</div>
      <div class="skill">HSK</div>
    </div>
  </section>

  <section id="contact">
    <h2>Contact</h2>
    <p style="text-align:center;">
      Email: maxxleong904@gmail.com | Phone: +62 811-631-0905 <br>
    </p>
  </section>

  <footer>
    <p>© 2025 Maxx Reinhart Leong | Student Portfolio</p>
  </footer>

  <script src="https://cdnjs.cloudflare.com/ajax/libs/html2pdf.js/0.9.3/html2pdf.bundle.min.js"></script>
  <script>
    function toggleDarkMode() {
      document.body.classList.toggle('dark');
      const btn = document.querySelectorAll('.btn')[0];
      btn.textContent = document.body.classList.contains('dark') ? "☀️ Light" : "🌙 Dark";
    }

    function downloadPDF() {
      const element = document.body;
      const opt = {
        margin: 0.5,
        filename: 'Student_Portfolio.pdf',
        image: { type: 'jpeg', quality: 1 },
        html2canvas: { scale: 3, useCORS: true }, 
        jsPDF: { unit: 'in', format: 'letter', orientation: 'portrait' }
      };
      html2pdf().set(opt).from(element).save();
    }
  </script>
</body>
</html>

