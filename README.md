<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Valarmathi | Portfolio</title>

  <!-- Google Font -->
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;800;900&display=swap" rel="stylesheet">

  <!-- Font Awesome -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css"/>

  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      font-family: 'Poppins', sans-serif;
      background: linear-gradient(120deg, #0f2027, #203a43, #2c5364);
      color: #fff;
    }

    /* NAVBAR */
    nav {
      position: fixed;
      top: 0;
      width: 100%;
      background: rgba(0,0,0,0.35);
      backdrop-filter: blur(10px);
      padding: 15px;
      text-align: center;
      z-index: 1000;
    }

    nav a {
      color: #fff;
      margin: 0 15px;
      text-decoration: none;
      font-weight: 500;
    }

    nav a:hover {
      color: #f093fb;
    }

    /* HEADER */
    header {
      min-height: 100vh;
      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
      background: linear-gradient(135deg, #1d2671, #c33764);
      padding-top: 80px;
    }

    .hero-box {
      background: rgba(255,255,255,0.15);
      padding: 80px;
      border-radius: 30px;
      backdrop-filter: blur(15px);
      box-shadow: 0 20px 60px rgba(0,0,0,0.4);
    }

    /* BIG NAME */
    .hero-name {
      font-size: 96px;
      font-weight: 900;
      letter-spacing: 8px;
      text-transform: uppercase;
      background: linear-gradient(
        90deg,
        #ffecd2,
        #fcb69f,
        #ff6a88,
        #8fd3f4,
        #a18cd1
      );
      background-size: 400% 400%;
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      animation: gradientMove 6s ease infinite, glowPulse 2.5s infinite alternate;
    }

    @keyframes gradientMove {
      0% { background-position: 0% 50%; }
      50% { background-position: 100% 50%; }
      100% { background-position: 0% 50%; }
    }

    @keyframes glowPulse {
      from { filter: drop-shadow(0 0 12px #ff6a88); }
      to { filter: drop-shadow(0 0 30px #8fd3f4); }
    }

    .subtitle {
      margin-top: 20px;
      font-size: 22px;
      opacity: 0.9;
    }

    /* SECTIONS */
    section {
      max-width: 1100px;
      margin: auto;
      padding: 80px 20px;
    }

    h2 {
      text-align: center;
      font-size: 36px;
      margin-bottom: 40px;
      color: #f093fb;
    }

    .card {
      background: rgba(255,255,255,0.08);
      padding: 30px;
      border-radius: 20px;
      box-shadow: 0 10px 40px rgba(0,0,0,0.3);
      margin-bottom: 25px;
    }

    .grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
      gap: 25px;
    }

    .skill-card {
      text-align: center;
      font-size: 20px;
    }

    .skill-card i {
      font-size: 50px;
      margin-bottom: 10px;
    }

    footer {
      text-align: center;
      padding: 30px;
      background: rgba(0,0,0,0.4);
    }

    /* MOBILE */
    @media (max-width: 600px) {
      .hero-name {s
        font-size: 52px;
        letter-spacing: 4px;
      }
      .hero-box {
        padding: 50px 30px;
      }
    }
  </style>
</head>

<body>

<nav>
  <a href="#home">Home</a>
  <a href="#education">Education</a>
  <a href="#skills">Skills</a>
  <a href="#certificates">Certificates</a>
  <a href="#contact">Contact</a>
</nav>

<!-- HEADER -->
<header id="home">
  <div class="hero-box">
    <h1 class="hero-name">
      <span id="typing"></span>
    </h1>
    <p class="subtitle">Aspiring Developer | Creative Thinker</p>
  </div>
</header>

<!-- EDUCATION -->
<section id="education">
  <h2>Education</h2>
  <div class="card">
    <p><strong>Degree:</strong> BCA</p>
    <p><strong>Institution:</strong> Sri Akilandeswari womens college ,Thiruvalluvar University</p>
    <p><strong>Year:</strong> 2022 – 2025</p>
  </div>
  <div class="card">
    <p><strong>Degree:</strong> MCA</p>
    <p><strong>Institution:</strong> Arcot Sri Mahalakshmi Women's Institute Of Management and Computer Applications college,Thiruvalluvar University</p>
    <p><strong>Year:</strong> 2025– 2027</p>
  </div>
</section>

<!-- SKILLS -->
<section id="skills">
  <h2>Skills</h2>
  <div class="grid">
    <div class="card skill-card">
      <i class="fa-brands fa-python" style="color:#3776ab;"></i>
      <p>Python</p>
    </div>
    <div class="card skill-card">
      <i class="fa-solid fa-database" style="color:#f29111;"></i>
      <p>SQL</p>
    </div>
    <div class="card skill-card">
      <i class="fa-brands fa-salesforce" style="color:#00a1e0;"></i>
      <p>Salesforce</p>
    </div>
  </div>
</section>

<!-- CERTIFICATES -->
<section id="certificates">
  <h2>Certificates</h2>
  <div class="grid">
    <div class="card">Data Analytics</div>
    <div class="card">Python framework</div>
    <div class="card">Salesforce Admin</div>
  </div>
</section>

<!-- CONTACT -->
<section id="contact">
  <h2>Contact</h2>
  <div class="card" style="text-align:center;">
    <p>Email: valar.kiruthi1@gmail.com</p>
    <p> Phone: 8015607017 </p>
  </div>
</section>

<footer>
  <p>© 2025 Valarmathi | All rigths are reserved</p>
</footer>

<script>
  const text = "VALARMATHI";
  let index = 0;

  function typeEffect() {
    if (index < text.length) {
      document.getElementById("typing").textContent += text.charAt(index);
      index++;
      setTimeout(typeEffect, 120);
    }
  }
  typeEffect();
</script>

</body>
</html>
