# EVNepal
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <title>EVNepal | Electric Vehicle Information Hub</title>

  <meta name="description"
        content="EVNepal - Nepal's electric vehicle information hub for EV cars, scooters, used EVs, prices, specifications, battery, charging, comparisons and news.">

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: Arial, Helvetica, sans-serif;
      background: #f5f7f9;
      color: #1f2937;
    }

    /* HEADER */

    header {
      background: white;
      border-bottom: 1px solid #e5e7eb;
      position: sticky;
      top: 0;
      z-index: 1000;
    }

    .navbar {
      max-width: 1250px;
      margin: auto;
      padding: 15px 20px;
      display: flex;
      align-items: center;
      justify-content: space-between;
    }

    .logo {
      font-size: 28px;
      font-weight: 800;
      color: #16a34a;
    }

    .logo span {
      color: #111827;
    }

    .menu {
      display: flex;
      gap: 22px;
      list-style: none;
    }

    .menu a {
      text-decoration: none;
      color: #374151;
      font-size: 15px;
      font-weight: 500;
    }

    .menu a:hover {
      color: #16a34a;
    }

    /* HERO */

    .hero {
      background: linear-gradient(135deg, #ecfdf5, #ffffff);
      padding: 70px 20px 65px;
      text-align: center;
    }

    .hero h1 {
      font-size: 46px;
      margin-bottom: 12px;
      color: #111827;
    }

    .hero h1 span {
      color: #16a34a;
    }

    .hero p {
      font-size: 18px;
      color: #6b7280;
      margin-bottom: 30px;
    }

    .search-box {
      max-width: 720px;
      margin: auto;
      display: flex;
      background: white;
      border: 1px solid #d1d5db;
      border-radius: 10px;
      overflow: hidden;
      box-shadow: 0 5px 20px rgba(0,0,0,0.06);
    }

    .search-box input {
      flex: 1;
      padding: 17px;
      border: none;
      outline: none;
      font-size: 16px;
    }

    .search-box button {
      border: none;
      padding: 0 28px;
      background: #16a34a;
      color: white;
      font-size: 16px;
      cursor: pointer;
    }

    /* MAIN */

    .container {
      max-width: 1250px;
      margin: auto;
      padding: 55px 20px;
    }

    .section-title {
      text-align: center;
      margin-bottom: 30px;
    }

    .section-title h2 {
      font-size: 30px;
      margin-bottom: 8px;
      color: #111827;
    }

    .section-title p {
      color: #6b7280;
    }

    /* CATEGORY */

    .category-grid {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 20px;
    }

    .category-card {
      background: white;
      padding: 30px 20px;
      text-align: center;
      border-radius: 14px;
      border: 1px solid #e5e7eb;
      transition: 0.2s;
    }

    .category-card:hover {
      transform: translateY(-4px);
      box-shadow: 0 10px 25px rgba(0,0,0,0.08);
    }

    .category-icon {
      font-size: 42px;
      margin-bottom: 15px;
    }

    .category-card h3 {
      margin-bottom: 9px;
    }

    .category-card p {
      font-size: 14px;
      color: #6b7280;
      line-height: 1.5;
    }

    /* FILTERS */

    .filter-section {
      background: white;
      padding: 35px 20px;
      margin-top: 30px;
      border-radius: 14px;
      border: 1px solid #e5e7eb;
    }

    .filter-title {
      font-size: 23px;
      margin-bottom: 20px;
    }

    .filter-grid {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 15px;
    }

    .filter {
      border: 1px solid #d1d5db;
      padding: 14px;
      border-radius: 8px;
      background: #fff;
    }

    /* INFORMATION CARDS */

    .info-grid {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 20px;
    }

    .info-card {
      background: white;
      padding: 25px;
      border-radius: 12px;
      border: 1px solid #e5e7eb;
    }

    .info-card h3 {
      margin-bottom: 10px;
    }

    .info-card p {
      color: #6b7280;
      line-height: 1.6;
    }

    /* USED EV */

    .used-ev {
      background: #ffffff;
      border-radius: 14px;
      padding: 35px 25px;
      border: 1px solid #e5e7eb;
    }

    .used-buttons {
      display: flex;
      flex-wrap: wrap;
      gap: 12px;
      margin-top: 20px;
    }

    .used-buttons button {
      padding: 12px 20px;
      border: 1px solid #d1d5db;
      border-radius: 8px;
      background: white;
      cursor: pointer;
    }

    .used-buttons button:hover {
      border-color: #16a34a;
      color: #16a34a;
    }

    /* CTA */

    .cta {
      background: #111827;
      color: white;
      text-align: center;
      padding: 55px 20px;
      border-radius: 15px;
      margin-top: 20px;
    }

    .cta h2 {
      font-size: 32px;
      margin-bottom: 12px;
    }

    .cta p {
      color: #d1d5db;
      margin-bottom: 22px;
    }

    .cta button {
      background: #16a34a;
      border: none;
      color: white;
      padding: 13px 25px;
      border-radius: 8px;
      font-size: 16px;
      cursor: pointer;
    }

    /* FOOTER */

    footer {
      background: #111827;
      color: #9ca3af;
      margin-top: 50px;
      padding: 35px 20px;
      text-align: center;
    }

    footer h3 {
      color: white;
      margin-bottom: 10px;
    }

    footer p {
      margin: 6px 0;
    }

    /* MOBILE */

    @media (max-width: 900px) {

      .menu {
        display: none;
      }

      .category-grid {
        grid-template-columns: repeat(2, 1fr);
      }

      .info-grid {
        grid-template-columns: repeat(2, 1fr);
      }

      .filter-grid {
        grid-template-columns: 1fr 1fr;
      }

      .hero h1 {
        font-size: 38px;
      }
    }

    @media (max-width: 600px) {

      .hero {
        padding: 50px 15px;
      }

      .hero h1 {
        font-size: 32px;
      }

      .hero p {
        font-size: 16px;
      }

      .search-box {
        flex-direction: column;
      }

      .search-box button {
        padding: 14px;
      }

      .category-grid {
        grid-template-columns: 1fr 1fr;
      }

      .info-grid {
        grid-template-columns: 1fr;
      }

      .filter-grid {
        grid-template-columns: 1fr;
      }
    }

  </style>
</head>

<body>

<!-- HEADER -->

<header>

  <div class="navbar">

    <div class="logo">
      EV<span>Nepal</span>
    </div>

    <ul class="menu">
      <li><a href="#">Home</a></li>
      <li><a href="#cars">Cars</a></li>
      <li><a href="#scooters">Scooters</a></li>
      <li><a href="#used">Used EV</a></li>
      <li><a href="#other">Other EV</a></li>
      <li><a href="#charging">Charging</a></li>
      <li><a href="#brands">Brands</a></li>
    </ul>

  </div>

</header>


<!-- HERO -->

<section class="hero">

  <h1>Welcome to <span>EVNepal</span></h1>

  <p>
    Nepal's Electric Vehicle Information Hub
  </p>

  <div class="search-box">

    <input
      type="text"
      placeholder="Search EV, brand, model, price..."
    >

    <button onclick="searchEV()">
      Search
    </button>

  </div>

</section>


<!-- MAIN CATEGORIES -->

<div class="container">

  <div class="section-title">

    <h2>Explore EVNepal</h2>

    <p>
      Find electric vehicles, prices, specifications and more.
    </p>

  </div>


  <div class="category-grid">


    <div class="category-card" id="cars">

      <div class="category-icon">🚗</div>

      <h3>EV Cars</h3>

      <p>
        Electric cars available and coming to Nepal.
      </p>

    </div>


    <div class="category-card" id="scooters">

      <div class="category-icon">🛵</div>

      <h3>EV Scooters</h3>

      <p>
        Electric scooters, specifications, prices and range.
      </p>

    </div>


    <div class="category-card" id="used">

      <div class="category-icon">♻️</div>

      <h3>Used EV</h3>

      <p>
        Find used electric cars and scooters from different platforms.
      </p>

    </div>


    <div class="category-card" id="other">

      <div class="category-icon">🚜</div>

      <h3>Other EV</h3>

      <p>
        Electric dozers, tippers, trucks, buses, vans and more.
      </p>

    </div>


    <div class="category-card" id="charging">

      <div class="category-icon">🔌</div>

      <h3>Charging Stations</h3>

      <p>
        Find EV charging stations and charging information.
      </p>

    </div>


    <div class="category-card" id="brands">

      <div class="category-icon">🏷️</div>

      <h3>Brands</h3>

      <p>
        Explore EV manufacturers and their models.
      </p>

    </div>


    <div class="category-card">

      <div class="category-icon">⚖️</div>

      <h3>Compare EVs</h3>

      <p>
        Compare price, battery, range, power and features.
      </p>

    </div>


    <div class="category-card">

      <div class="category-icon">📰</div>

      <h3>EV News</h3>

      <p>
        Latest electric vehicle news and updates.
      </p>

    </div>

  </div>


  <!-- PRICE SORTING -->

  <div class="filter-section">

    <h2 class="filter-title">
      🔎 Find EV by Price, Battery & Motor
    </h2>

    <div class="filter-grid">

      <div class="filter">
        💰 Price: Low → High
      </div>

      <div class="filter">
        💰 Price: High → Low
      </div>

      <div class="filter">
        🔋 Battery: Low → High
      </div>

      <div class="filter">
        🔋 Battery: High → Low
      </div>

      <div class="filter">
        ⚡ Motor Power: Low → High
      </div>

      <div class="filter">
        ⚡ Motor Power: High → Low
      </div>

    </div>

  </div>


  <!-- USED EV -->

  <div class="container" id="used">

    <div class="section-title">

      <h2>♻️ Used EV</h2>

      <p>
        Explore used EV listings from different marketplaces.
      </p>

    </div>

    <div class="used-ev">

      <h3>Find Used EV Listings</h3>

      <p>
        EVNepal can provide links to external marketplaces
        where used EV listings are available.
      </p>

      <div class="used-buttons">

        <button>
          HamroBazar
        </button>

        <button>
          Facebook Marketplace
        </button>

        <button>
          Other Websites
        </button>

        <button>
          Submit Your Used EV
        </button>

      </div>

    </div>

  </div>


  <!-- FULL DETAILS -->

  <div class="section-title">

    <h2>📋 Full EV Details</h2>

    <p>
      Detailed specifications for every vehicle.
    </p>

  </div>


  <div class="info-grid">

    <div class="info-card">

      <h3>💰 Price</h3>

      <p>
        Nepal price, international price and price updates.
      </p>

    </div>


    <div class="info-card">

      <h3>🔋 Battery</h3>

      <p>
        Battery capacity, chemistry, warranty and battery information.
      </p>

    </div>


    <div class="info-card">

      <h3>⚡ Motor</h3>

      <p>
        Motor power, torque, performance and top speed.
      </p>

    </div>


    <div class="info-card">

      <h3>🛣️ Range</h3>

      <p>
        Claimed range and real-world range information.
      </p>

    </div>


    <div class="info-card">

      <h3>📏 Dimensions</h3>

      <p>
        Length, width, height, wheelbase and ground clearance.
      </p>

    </div>


    <div class="info-card">

      <h3>🔌 Charging</h3>

      <p>
        AC charging, DC fast charging, charging time and cost.
      </p>

    </div>


    <div class="info-card">

      <h3>🛡️ Safety</h3>

      <p>
        Airbags, ABS, ESC, ADAS, cameras and other safety features.
      </p>

    </div>


    <div class="info-card">

      <h3>🧰 Warranty</h3>

      <p>
        Vehicle warranty and battery warranty information.
      </p>

    </div>


    <div class="info-card">

      <h3>⭐ Reviews</h3>

      <p>
        Practical reviews, ownership experience and EV tests.
      </p>

    </div>

  </div>


  <!-- CTA -->

  <div class="cta">

    <h2>Thinking About Going Electric?</h2>

    <p>
      Find the right EV for Nepal with EVNepal.
    </p>

    <button onclick="alert('EVNepal features are coming soon!')">
      Explore EVs
    </button>

  </div>

</div>


<!-- FOOTER -->

<footer>

  <h3>EVNepal</h3>

  <p>
    Nepal's Electric Vehicle Information Hub
  </p>

  <p>
    © 2026 EVNepal. All rights reserved.
  </p>

</footer>


<script>

function searchEV() {

  const input = document.querySelector(".search-box input");

  const query = input.value.trim();

  if (query === "") {

    alert("Please enter an EV, brand, model or price.");

  } else {

    alert("Search feature will be connected to the EV database soon.");

  }

}

</script>

</body>
</html>
