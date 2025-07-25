<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>LDCA Truckc:\Users\Benjo\LDCATRUCKS.htmls Trading</title>
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
    /* How to buy slider */
    .how-to-buy {
      position: relative;
      max-width: 700px;
      margin: 50px auto 0;
      overflow: hidden;
      border: 1px solid #0f5132;
      border-radius: 10px;
      background: #111;
      color: #ddd;
    }
    .steps {
      display: flex;
      width: 300%;
      transition: transform 0.5s ease-in-out;
    }
    .step {
      flex: 1 0 100%;
      padding: 30px;
      text-align: center;
    }
    .step h3 {
      color: #0f5132;
      margin-bottom: 10px;
    }
    .step button {
      margin-top: 20px;
      padding: 10px 20px;
      border: none;
      background: #0f5132;
      color: white;
      cursor: pointer;
      border-radius: 5px;
      font-weight: bold;
      transition: background-color 0.3s ease;
    }
    .step button:hover {
      background-color: #095021;
    }
    .slider-controls {
      text-align: center;
      margin: 15px 0 20px;
    }
    .slider-controls button {
      background: none;
      border: none;
      color: white;
      font-size: 28px;
      cursor: pointer;
      margin: 0 20px;
      transition: color 0.3s ease;
    }
    .slider-controls button:hover {
      color: #0f5132;
    }
    /* FAQ Section */
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
    /* Contact section */
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
    /* Footer */
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
      <p>You can select your truck, then follow the steps in the “How to Buy” section to contact us through Facebook or email.</p>
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
  <div class="truck-gallery">
    <div class="truck-card">
      <img src="https://i.imgur.com/9FXSm9U.jpeg" alt="Isuzu Forward" />
      <h3>Isuzu Forward</h3>
    </div>
    <div class="truck-card">
      <img src="https://i.imgur.com/7Vcl2Ow.jpeg" alt="Mitsubishi Fuso Fighter" />
      <h3>Mitsubishi Fuso Fighter</h3>
    </div>
    <div class="truck-card">
      <img src="https://i.imgur.com/9eiuTex.jpg" alt="Isuzu Forward (Newer Model)" />
      <h3>Isuzu Forward (Newer Model)</h3>
    </div>
    <div class="truck-card">
      <img src="https://i.imgur.com/z6lL8a3.jpg" alt="Mitsubishi Fuso Fighter Dump" />
      <h3>Fuso Fighter Dump Truck</h3>
    </div>
    <div class="truck-card">
      <img src="https://i.imgur.com/QEL3vJm.jpg" alt="Isuzu Elf Flatbed" />
      <h3>Isuzu Elf Flatbed</h3>
    </div>
    <div class="truck-card">
      <img src="https://i.imgur.com/97CrJiV.jpg" alt="Isuzu Forward Dump" />
      <h3>Isuzu Forward Dump Truck</h3>
    </div>
    <div class="truck-card">
      <img src="https://i.imgur.com/xyBdreB.jpg" alt="Isuzu Forward Wing Van" />
      <h3>Isuzu Forward Wing Van</h3>
    </div>
  </div>

  
<section id="contact">
  <h2>Contact Us</h2>
  <ul>
    <li><strong>Globe/TM:</strong> 0915‑759‑9700</li>
    <li><strong>Smart:</strong> 0923‑858‑9691</li>
  </ul>

  <h3>Our Location</h3>
  <iframe
    src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3988.236640576567!2d125.61081521475302!3d7.086115394759466!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x32fca8a2d344a8db%3A0x92b1586e42baf21c!2s4J9G%2B4M6%20Davao%20City%20Diversion%20Rd%2C%20Buhangin%2C%20Davao%20City!5e0!3m2!1sen!2sph!4v1690031303380!5m2!1sen!2sph"
    width="100%"
    height="300"
    style="border:0;"
    allowfullscreen=""
    loading="lazy"
    referrerpolicy="no-referrer-when-downgrade"
  ></iframe>
</section>

<footer>
  <p>© 2025 LDCA Trucks Trading. All rights reserved.</p>
</footer>

<script>
  // Slider logic
  let current = 0;
  const steps = document.getElementById('steps');

  function updateSlider() {
    steps.style.transform = `translateX(-${current * 100}%)`;
  }

  function nextStep() {
    if (current < 2) {
      current++;
      updateSlider();
    }
  }

  function prevStep() {
    if (current > 0) {
      current--;
      updateSlider();
    }
  }

  // Responsive menu toggle
  function toggleMenu() {
    document.getElementById('navLinks').classList.toggle('show');
  }

  // Open Facebook page
  function goFB() {
    window.open('https://www.facebook.com/profile.php?id=61578237163428', '_blank');
  }

  // FAQ accordion
  const faqButtons = document.querySelectorAll('.faq-question');
  faqButtons.forEach(button => {
    button.addEventListener('click', () => {
      const answer = button.nextElementSibling;
      const maxHeight = answer.style.maxHeight;
      // Close all answers
      document.querySelectorAll('.faq-answer').forEach(ans => {
        ans.style.maxHeight = null;
      });
      if (!maxHeight) {
        answer.style.maxHeight = answer.scrollHeight + "px";
      } else {
        answer.style.maxHeight = null;
      }
    });
  });
</script>

</body>
</html>
