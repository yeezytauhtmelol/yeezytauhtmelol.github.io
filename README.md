<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Your Name</title>
  <!-- Google Fonts -->
  <link href="https://fonts.googleapis.com/css2?family=Inter&family=Playfair+Display&display=swap" rel="stylesheet">
  <style>
    /* Reset & base styles */
    * { margin: 0; padding: 0; box-sizing: border-box; }
    body { font-family: 'Inter', sans-serif; line-height: 1.6; background: #f9f9f9; color: #111; }

    /* Header & nav */
    header { position: sticky; top:0; background: #fff; padding: 15px 20px; box-shadow: 0 2px 5px rgba(0,0,0,0.1); }
    nav ul { display: flex; justify-content: center; list-style: none; }
    nav li { margin: 0 15px; }
    nav a { text-decoration: none; color: #111; font-weight: 500; }

    /* Hero Section */
    .hero { height: 100vh; display: flex; flex-direction: column; justify-content: center; align-items: center; text-align: center; background: linear-gradient(135deg, #f0f0f0, #d0d0d0); }
    .hero h1 { font-family: 'Playfair Display', serif; font-size: 3rem; margin-bottom: 15px; }
    .hero p { font-size: 1.25rem; color: #555; }

    /* Sections */
    section { padding: 80px 20px; max-width: 900px; margin: auto; }

    h2 { font-family: 'Playfair Display', serif; font-size: 2rem; margin-bottom: 20px; text-align: center; }

    /* Contact Form */
    form { display: flex; flex-direction: column; gap: 15px; }
    input, textarea { padding: 10px; font-size: 1rem; border: 1px solid #ccc; border-radius: 5px; }
    button { padding: 12px; font-size: 1rem; border: none; border-radius: 5px; background: #111; color: #fff; cursor: pointer; transition: 0.3s; }
    button:hover { background: #444; }

    /* Footer */
    footer { text-align: center; padding: 20px; background: #111; color: #fff; }

    /* Smooth scroll */
    html { scroll-behavior: smooth; }

    /* Responsive */
    @media(max-width:600px){ .hero h1 { font-size:2.2rem; } .hero p { font-size:1rem; } }
  </style>
</head>
<body>

  <!-- Header -->
  <header>
    <nav>
      <ul>
        <li><a href="#about">About Me</a></li>
        <li><a href="#portfolio">Portfolio</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>

  <!-- Hero Section -->
  <section class="hero">
    <h1>Hello, I'm Jim</h1>
    <p>Welcome to my personal website.</p>
  </section>

  <!-- About Section -->
  <section id="about">
    <h2>About Me</h2>
    <p>I love tcc, I am apart of the true crime community. I love movies like elephant, zero day etc.</p>
  </section>

  <!-- Portfolio Section -->
  <section id="portfolio">
    <h2>Portfolio</h2>
    <p><iframe src="https://discord.com/widget?id=1478169703259181189&theme=dark" width="350" height="500" allowtransparency="true" frameborder="0" sandbox="allow-popups allow-popups-to-escape-sandbox allow-same-origin allow-scripts"></iframe></p>
  </section>

  <!-- Contact Section -->
  <section id="contact">
    <h2>Contact Me</h2>
    <form onsubmit="submitForm(event)">
      <input type="text" placeholder="Your Name" required>
      <input type="email" placeholder="Your Email" required>
      <textarea placeholder="Your Message" rows="5" required></textarea>
      <button type="submit">Send</button>
    </form>
    <p id="response" style="margin-top:10px;color:green;"></p>
  </section>

  <!-- Footer -->
  <footer>
    © 2026 Jim | Follow me on social media
  </footer>

  <script>
    function submitForm(e){
      e.preventDefault();
      document.getElementById('response').innerText = "Thank you! Your message has been sent.";
      e.target.reset();
    }
  </script>
</body>
</html>
