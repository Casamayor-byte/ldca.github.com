<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>LDCA TRUCKS TRADING</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background-color: #111;
      color: #fff;
    }
    header {
      background-color: #000;
      padding: 1rem;
      text-align: center;
    }
    nav {
      background-color: #222;
      display: flex;
      justify-content: center;
      gap: 1rem;
      padding: 1rem;
    }
    nav a {
      color: white;
      text-decoration: none;
      font-weight: bold;
    }
    .hero {
      background: url('your-truck-background.jpg') center/cover no-repeat;
      height: 400px;
      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
    }
    .hero h1 {
      background: rgba(0, 0, 0, 0.6);
      padding: 1rem;
      border-radius: 10px;
    }
    .section {
      padding: 2rem;
      max-width: 1200px;
      margin: auto;
    }
    .truck-gallery {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
      gap: 1rem;
    }
    .truck-card {
      background: #222;
      padding: 1rem;
      border-radius: 10px;
      text-align: center;
    }
    .truck-card img {
      width: 100%;
      height: 200px;
      object-fit: cover;
      border-radius: 8px;
    }
    footer {
      background: #000;
      text-align: center;
      padding: 1rem;
      margin-top: 2rem;
    }
  </style>
</head>
<body>
  <header>
    <h1>LDCA TRUCKS TRADING</h1>
  </header>

  <nav>
    <a href="#home">Home</a>
    <a href="#about">About</a>
    <a href="#services">Services</a>
    <a href="#contact">Contact</a>
  </nav>

  <div class="hero" id="home">
    <h1>Japan Surplus Commercial Trucks</h1>
  </div>

  <section class="section" id="about">
    <h2>About Us</h2>
    <p>LDCA Trucks Trading specializes in quality Japan surplus commercial trucks. We offer durable, affordable, and reliable units tailored for your business needs.</p>
  </section>

  <section class="section" id="services">
    <h2>Available Truck Units</h2>
    <div class="truck-gallery" id="truckGallery">
      <!-- Truck cards will be loaded here -->
    </div>
  </section>

  <section class="section" id="contact">
    <h2>Contact Us</h2>
    <p>Email: ldcacommercial@gmail.com</p>
    <p>Phone: 0912-345-6789</p>
    <p>Visit us at: Davao City, Philippines</p>
    <div>
      <iframe src="4J9G+4M6, Davao City Diversion Rd, Buhangin, Davao City, Davao del Sur"
              width="100%" height="300" style="border:0;" allowfullscreen="" loading="lazy">
      </iframe>
    </div>
  </section>

  <footer>
    <p>&copy; 2025 LDCA Trucks Trading. All rights reserved.</p>
  </footer>

  <script>
    const truckData = [
      // Replace with actual data from your CSV
      { model: "Isuzu Elf", year: "2015", imageUrl: "images/isuzu_elf.jpg" },
      { model: "Mitsubishi Canter", year: "2016", imageUrl: "images/mitsubishi_canter.jpg" },
      { model: "Hino Dutro", year: "2014", imageUrl: "images/hino_dutro.jpg" },
      { model: "Nissan Atlas", year: "2017", imageUrl: "images/nissan_atlas.jpg" },
      { model: "Toyota Dyna", year: "2013", imageUrl: "images/toyota_dyna.jpg" }
    ];

    const gallery = document.getElementById('truckGallery');

    truckData.forEach(({ model, year, imageUrl }) => {
      const card = document.createElement('div');
      card.className = 'truck-card';
      card.innerHTML = `
        <img src="${imageUrl}" alt="${model} ${year}" loading="lazy" />
        <h3>${model} (${year})</h3>
      `;
      gallery.appendChild(card);
    });
  </script>
</body>
</html>
