# andika-suherman.github.ioportofolio
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Andika Suherman | Portfolio</title>

  <style>
    * {
      scroll-behavior: smooth;
    }

    body {
      font-family: Arial, Helvetica, sans-serif;
      margin: 0;
      background: #f5f7fa;
      color: #333;
      line-height: 1.6;
    }

    /* ===== NAVBAR ===== */
    nav {
      position: fixed;
      top: 0;
      width: 100%;
      background: #0f172a;
      padding: 12px 20px;
      z-index: 1000;
    }

    nav ul {
      list-style: none;
      display: flex;
      justify-content: center;
      gap: 25px;
      margin: 0;
      padding: 0;
    }

    nav a {
      color: #cbd5f5;
      text-decoration: none;
      font-weight: bold;
      transition: color 0.3s;
    }

    nav a:hover {
      color: #38bdf8;
    }

    /* ===== HEADER ===== */
    header {
      background: #0f172a;
      color: #fff;
      padding: 120px 20px 80px;
      text-align: center;
    }

    header img {
      width: 140px;
      height: 140px;
      border-radius: 50%;
      object-fit: cover;
      border: 4px solid #fff;
      margin-bottom: 20px;
    }

    header h1 {
      margin: 0;
      font-size: 34px;
    }

    header p {
      margin-top: 10px;
      font-size: 18px;
      color: #cbd5f5;
    }

    /* ===== SECTIONS ===== */
    section {
      max-width: 1000px;
      margin: auto;
      padding: 90px 20px;
      opacity: 0;
      transform: translateY(50px);
      transition: all 0.9s ease;
    }

    section.show {
      opacity: 1;
      transform: translateY(0);
    }

    h2 {
      color: #0f172a;
      border-bottom: 3px solid #2563eb;
      display: inline-block;
      padding-bottom: 5px;
      margin-bottom: 25px;
    }

    .card {
      background: #fff;
      padding: 25px;
      border-radius: 12px;
      box-shadow: 0 8px 20px rgba(0,0,0,0.08);
      margin-bottom: 20px;
      transition: transform 0.3s, box-shadow 0.3s;
    }

    .card:hover {
      transform: translateY(-6px);
      box-shadow: 0 14px 30px rgba(0,0,0,0.12);
    }

    ul {
      padding-left: 20px;
    }

    .skills {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
      gap: 20px;
    }

    footer {
      background: #0f172a;
      color: #cbd5f5;
      text-align: center;
      padding: 25px;
    }

    a {
      color: #2563eb;
      text-decoration: none;
    }
  </style>
</head>

<body>

<!-- ===== NAVBAR ===== -->
<nav>
  <ul>
    <li><a href="#home">Home</a></li>
    <li><a href="#about">About</a></li>
    <li><a href="#experience">Experience</a></li>
    <li><a href="#projects">Projects</a></li>
    <li><a href="#skills">Skills</a></li>
    <li><a href="#contact">Contact</a></li>
  </ul>
</nav>

<!-- ===== HOME ===== -->
<header id="home">
  <img src="profile.jpg" alt="Andika Suherman">
  <h1>Andika Suherman</h1>
  <p>Electrical Engineer | IoT & System Development</p>
</header>

<section id="about">
  <h2>About Me</h2>
  <div class="card">
    Fresh graduate in Electrical Engineering from Universitas Al Azhar Indonesia with internship experience
    at the National Research and Innovation Agency (BRIN). Experienced in IoT-based system development,
    data analysis, and digital system implementation. Highly motivated to support digital transformation
    and technological innovation.
  </div>
</section>

<section id="experience">
  <h2>Experience</h2>

  <div class="card">
    <strong>National Research and Innovation Agency (BRIN)</strong><br>
    Technology Division Intern (Aug 2023 – Feb 2024)
    <ul>
      <li>Charging Station System development</li>
      <li>Battery Swap Station optimization</li>
      <li>LoRa-based communication systems</li>
    </ul>
  </div>

  <div class="card">
    <strong>Centre for International Education – UAI</strong><br>
    Physics Laboratory Assistant (Apr 2025 – May 2025)
    <ul>
      <li>Prepared physics lab equipment</li>
      <li>Cambridge-standard practical experiments</li>
      <li>Assisted 20+ students</li>
    </ul>
  </div>
</section>

<section id="projects">
  <h2>Projects</h2>
  <div class="card">
    <ul>
      <li><strong>IoT-Based Health Measurement System</strong> – Final thesis</li>
      <li><strong>LoRa Communication System</strong> – Research project</li>
      <li><strong>Product Defect Detection</strong> – MATLAB image processing</li>
    </ul>
  </div>
</section>

<section id="skills">
  <h2>Skills</h2>
  <div class="card skills">
    <div>
      <strong>Hard Skills</strong>
      <ul>
        <li>MATLAB</li>
        <li>Arduino IDE</li>
        <li>Python</li>
        <li>Multisim</li>
        <li>Microsoft Office</li>
        <li>VS Code</li>
        <li>Canva</li>
      </ul>
    </div>
    <div>
      <strong>Soft Skills</strong>
      <ul>
        <li>Problem Solving</li>
        <li>Team Work</li>
        <li>Critical Thinking</li>
        <li>Leadership</li>
        <li>Time Management</li>
      </ul>
    </div>
  </div>
</section>

<section id="contact">
  <h2>Contact</h2>
  <div class="card">
    📧 <a href="mailto:andikasuherman0017@gmail.com">andikasuherman0017@gmail.com</a><br>
    📱 0814-1342-7075<br>
    🔗 <a href="https://www.linkedin.com/in/andikasuherman13" target="_blank">
      linkedin.com/in/andikasuherman13
    </a>
  </div>
</section>

<footer>
  © 2025 Andika Suherman | Portfolio Website
</footer>

<!-- ===== SCROLL ANIMATION SCRIPT ===== -->
<script>
  const sections = document.querySelectorAll("section");

  const observer = new IntersectionObserver(
    entries => {
      entries.forEach(entry => {
        if (entry.isIntersecting) {
          entry.target.classList.add("show");
        }
      });
    },
    { threshold: 0.15 }
  );

  sections.forEach(section => {
    observer.observe(section);
  });
</script>

</body>
</html>
