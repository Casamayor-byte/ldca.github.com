<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>LDCA Trucks Trading</title>
  <style>
    * {
      box-sizing: border-box;
    }
    body {
      margin: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background: url('https://i.imgur.com/qEMbS7c.jpg') no-repeat center center fixed;
      background-size: cover;
      color: white;
      min-height: 100vh;
    }
    header {
      background-color: rgba(0, 0, 0, 0.884);
      padding: 10px 20px;
      display: flex;
      align-items: center;
      justify-content: space-between;
      position: sticky;
      top: 0;
      z-index: 1000;
    }
    .logo img {
      height: 50px;
    }
    nav {
      position: relative;
    }
    .nav-links {
      display: flex;
      gap: 20px;
    }
    nav a {
      color: white;
      text-decoration: none;
      font-weight: bold;
      transition: color 0.3s;
    }
    nav a:hover {
      color: #0f5132;
    }
    .menu-btn {
      display: none;
      font-size: 1.5rem;
      color: white;
      cursor: pointer;
    }
    @media (max-width: 768px) {
      .nav-links {
        position: absolute;
        top: 60px;
        right: 0;
        background-color: #111;
        flex-direction: column;
        width: 200px;
        display: none;
        padding: 10px;
        border-radius: 5px;
      }
      .nav-links.show {
        display: flex;
      }
      .menu-btn {
        display: block;
      }
    }
    section {
      max-width: 1100px;
      margin: 30px auto;
      padding: 40px 20px;
      background-color: rgba(0, 0, 0, 0.75);
      border-radius: 12px;
    }
    h1, h2, h3 {
      color: #0f5132;
    }
    .hero {
      text-align: center;
      padding: 60px 20px;
    }
    .truck-gallery {
      display: grid;
      gap: 20px;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    }
    .truck-card {
      background: #111;
      border: 1px solid #0f5132;
      border-radius: 8px;
      overflow: hidden;
      transition: transform 0.3s;
    }
    .truck-card:hover {
      transform: translateY(-5px);
    }
    .truck-card img {
      width: 100%;
      height: 200px;
      object-fit: cover;
      display: block;
    }
    .truck-card h3 {
      margin: 10px;
      color: white;
      text-align: center;
    }
    #faqs {
      max-width: 1100px;
      margin: 30px auto;
      padding: 20px;
      background-color: rgba(0,0,0,0.75);
      border-radius: 12px;
      color: white;
    }
    .faq-item {
      margin-bottom: 15px;
      border-bottom: 1px solid #0f5132;
    }
    .faq-question {
      width: 100%;
      background: none;
      border: none;
      color: #0f5132;
      font-weight: bold;
      font-size: 1.1rem;
      text-align: left;
      padding: 12px 10px;
      cursor: pointer;
      outline: none;
      transition: background-color 0.3s ease;
    }
    .faq-question:hover {
      background-color: rgba(15, 81, 50, 0.1);
    }
    .faq-answer {
      max-height: 0;
      overflow: hidden;
      transition: max-height 0.4s ease;
      padding: 0 10px;
      color: #ddd;
    }
    .faq-answer p {
      margin: 10px 0;
    }
    #contact ul {
      list-style: none;
      padding: 0;
    }
    #contact ul li {
      margin-bottom: 8px;
    }
    #contact h3 {
      margin-top: 30px;
      color: #0f5132;
    }
    footer {
      text-align: center;
      padding: 20px;
      background-color: rgba(0, 0, 0, 0.85);
      margin-top: 50px;
      color: white;
    }
  </style>
</head>
<body>
<header>
  <div class="logo">
    <img src="https://i.imgur.com/yTLZoKA.png" alt="LDCA Logo" />
  </div>
  <nav>
    <span class="menu-btn" onclick="toggleMenu()">☰</span>
    <div class="nav-links" id="navLinks">
      <a href="#home">Home</a>
      <a href="#about">About</a>
      <a href="#faqs">FAQs</a>
      <a href="#services">Trucks</a>
      <a href="#contact">Contact</a>
    </div>
  </nav>
</header>

<section id="home" class="hero">
  <h1>Japan Surplus Trucks for Your Business</h1>
  <p>Quality, reliability, and value — tailored just for you.</p>
</section>

<section id="about">
  <h2>About LDCA Trucks Trading</h2>
  <p>
    LDCA Trucks Trading specializes in selling Japan surplus trucks across the Philippines. We provide a wide variety of commercial trucks such as wing vans, dump trucks, forward types, and flatbeds.
  </p>
  <p>
    With years of experience and trusted connections, we ensure all units are inspected and in good working condition. We aim to be your long-term truck supplier by prioritizing honesty, transparency, and unbeatable value.
  </p>
</section>

<section id="faqs">
  <h2>Frequently Asked Questions</h2>
  <div class="faq-item">
    <button class="faq-question">What types of trucks do you sell?</button>
    <div class="faq-answer">
      <p>We specialize in Japan surplus trucks including wing vans, dump trucks, forward types, flatbeds, and more.</p>
    </div>
  </div>
  <div class="faq-item">
    <button class="faq-question">Do you provide inspection and warranty?</button>
    <div class="faq-answer">
      <p>Yes, all trucks are inspected to ensure good working condition. We also offer limited warranty options depending on the truck.</p>
    </div>
  </div>
  <div class="faq-item">
    <button class="faq-question">How can I purchase a truck?</button>
    <div class="faq-answer">
      <p>You can select your truck, then message us via Facebook or email to proceed.</p>
    </div>
  </div>
  <div class="faq-item">
    <button class="faq-question">Do you deliver trucks nationwide?</button>
    <div class="faq-answer">
      <p>Yes, we offer delivery services across the Philippines. Delivery fees may vary depending on the location.</p>
    </div>
  </div>
</section>

<section id="services">
  <h2>Available Trucks</h2>
  <div class="truck-gallery" id="truckGallery">
    <!-- Truck cards will be loaded dynamically -->
  </div>
</section>

<section id="contact">
  <h2>Contact Us</h2>
  <ul>
    <li><strong>Globe/TM:</strong> 0915‑759‑9700</li>
    <li><strong>Smart:</strong> 0923‑858‑9691</li>
  </ul>
  <h3>Our Location</h3>
  <iframe src="https://www.google.com/maps/embed?..." width="100%" height="300" style="border:0;" allowfullscreen="" loading="lazy"></iframe>
</section>

<footer>
  <p>© 2025 LDCA Trucks Trading. All rights reserved.</p>
</footer>

<script>
  function toggleMenu() {
    document.getElementById('navLinks').classList.toggle('show');
  }

  document.querySelectorAll('.faq-question').forEach(button => {
    button.addEventListener('click', () => {
      const answer = button.nextElementSibling;
      const isOpen = answer.style.maxHeight;
      document.querySelectorAll('.faq-answer').forEach(ans => ans.style.maxHeight = null);
      if (!isOpen) answer.style.maxHeight = answer.scrollHeight + "px";
    });
  });

  async function loadTruckData() {
    try {
      const response = await fetch('https://docs.google.com/spreadsheets/d/1pU3KdAG09jccIFvo1anZHg3JGz85NLkpkVrRE87IEQs/export?format=csv');
      const text = await response.text();
      const rows = text.trim().split('\n').slice(1).map(r => r.split(','));
      const gallery = document.getElementById('truckGallery');
      rows.forEach(([model, year, imageUrl]) => {
        const card = document.createElement('div');
        card.className = 'truck-card';
        card.innerHTML = `<img src="${imageUrl}" alt="${model} (${year})" loading="lazy" /><h3>${model} (${year})</h3>`;
        gallery.appendChild(card);
      });
    } catch (err) {
      console.error('Failed to load truck data:', err);
    }
  }
  loadTruckData();
</script>
</body>
</html>
