# Malaysian-burger-1
Burger malaysia
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Malaysian Burger - Burger Kings</title>
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@600;700&display=swap" rel="stylesheet" />
  <style>
    /* Reset dan base styles */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Montserrat', sans-serif;
      scroll-behavior: smooth;
    }

    body {
      background: radial-gradient(circle at center, #850909, #4d0000);
      color: #f6c85f;
      min-height: 100vh;
      overflow-x: hidden;
    }

    a {
      text-decoration: none;
      color: #f6c85f;
    }

    /* Container utama */
    .container {
      max-width: 1100px;
      margin: 2rem auto;
      padding: 0 1.5rem;
    }

    /* Header Logo */
    .header-logo {
      display: flex;
      justify-content: center;
      align-items: center;
      margin-bottom: 1.5rem;
      filter: drop-shadow(0 0 6px #f6c85f);
    }

    .header-logo img {
      max-width: 180px;
      cursor: pointer;
      transition: transform 0.3s ease;
    }

    .header-logo img:hover {
      transform: scale(1.1);
    }

    /* Judul Utama */
    .main-title {
      text-align: center;
      font-weight: 700;
      font-size: 3rem;
      letter-spacing: 5px;
      color: #f6c85f;
      text-shadow: 0 0 12px #fff1a8;
      margin-bottom: 0.3rem;
      user-select: none;
    }

    /* Tagline */
    .tagline {
      text-align: center;
      font-style: italic;
      font-weight: 600;
      font-size: 1.2rem;
      color: #ffec99;
      margin-bottom: 3rem;
      user-select: none;
    }

    /* Menu Cards */
    .menu-section {
      background: rgba(40, 13, 0, 0.85);
      border-radius: 16px;
      padding: 2rem;
      margin-bottom: 3rem;
      box-shadow: 0 0 20px #f6c85f80;
      transition: box-shadow 0.4s ease;
    }

    .menu-section:hover {
      box-shadow: 0 0 30px #f6c85fff;
    }

    .menu-section h2 {
      font-weight: 700;
      font-size: 2.4rem;
      margin-bottom: 1.5rem;
      border-bottom: 3px solid #f6c85f;
      display: inline-block;
      padding-bottom: 4px;
      user-select: none;
    }

    .menu-list {
      list-style: none;
      font-weight: 600;
      font-size: 1.15rem;
      line-height: 2;
      color: #ffd85f;
    }

    .menu-list li {
      display: flex;
      justify-content: space-between;
      align-items: center;
      border-bottom: 1px solid #f6c85f30;
      padding: 6px 0;
      cursor: default;
      transition: color 0.3s ease;
    }

    .menu-list li:hover {
      color: #ffffff;
    }

    .menu-item-name {
      display: flex;
      align-items: center;
      gap: 10px;
    }

    .menu-price {
      font-weight: 700;
      font-size: 1.1rem;
      color: #fff;
      min-width: 55px;
      text-align: right;
    }

    /* Ikon Burger dan Ayam (simbol emoji sederhana) */
    .icon-chicken {
      font-size: 1.3rem;
    }

    .icon-burger {
      font-size: 1.3rem;
    }

    /* Banner Gambar Burger */
    .burger-banner {
      text-align: center;
      margin-bottom: 3rem;
      user-select: none;
    }

    .burger-banner img {
      max-width: 320px;
      border-radius: 20px;
      box-shadow: 0 0 25px #ffcf5f66;
      transition: transform 0.5s ease;
      cursor: pointer;
    }

    .burger-banner img:hover {
      transform: scale(1.05) rotate(-2deg);
      box-shadow: 0 0 40px #fff59dcc;
    }

    /* Call to Action */
    .cta {
      text-align: center;
      margin-bottom: 3rem;
    }

    .cta-phone {
      font-size: 1.5rem;
      font-weight: 700;
      background: #f6c85f;
      color: #500900;
      padding: 1rem 2rem;
      border-radius: 50px;
      cursor: pointer;
      user-select: none;
      box-shadow: 0 0 10px #f6c85fcc;
      display: inline-flex;
      align-items: center;
      gap: 0.5rem;
      transition: background-color 0.3s ease;
    }

    .cta-phone:hover {
      background: #fff8b0;
    }

    /* Animations */
    @keyframes float {
      0%, 100% {
        transform: translateY(0px);
      }

      50% {
        transform: translateY(-12px);
      }
    }

    .animated-burger {
      animation: float 4s ease-in-out infinite;
      filter: drop-shadow(0 0 6px #f6c85f);
    }

    /* Footer - Platform Delivery */
    .delivery-platforms {
      display: flex;
      justify-content: center;
      align-items: center;
      gap: 2.5rem;
      margin-top: 2rem;
      user-select: none;
    }

    .delivery-platforms img {
      width: 80px;
      filter: drop-shadow(0 0 4px #f6c85f);
      transition: transform 0.3s ease;
      cursor: pointer;
    }

    .delivery-platforms img:hover {
      transform: scale(1.2);
    }

    /* Responsive */
    @media (max-width: 720px) {
      .menu-section {
        padding: 1rem 1.5rem;
      }

      .burger-banner img {
        max-width: 240px;
      }

      .main-title {
        font-size: 2.3rem;
      }

      .menu-section h2 {
        font-size: 1.9rem;
      }

      .menu-list li {
        font-size: 1rem;
      }

      .cta-phone {
        font-size: 1.3rem;
        padding: 0.75rem 1.5rem;
      }

      .delivery-platforms img {
        width: 60px;
      }
    }
  </style>
</head>
<body>
  <div class="container">
    <!-- Header with logo -->
    <header class="header-logo">
      <img src="https://i.ibb.co/4pYyHxi/burger-kings-logo.png" alt="Burger Kings Logo" />
    </header>

    <!-- Main title -->
    <h1 class="main-title">MALAYSIAN BURGER</h1>
    <p class="tagline">Rasanya Juara, Harganya Rakyat!</p>

    <!-- Banner burger image with animation -->
    <section class="burger-banner">
      <img class="animated-burger" src="https://i.ibb.co/7X7nJHk/burger-double.jpg" alt="Double Burger Special" />
    </section>

    <!-- Menu ayam section -->
    <section class="menu-section" aria-label="Menu Burger Ayam">
      <h2>BURGER AYAM</h2>
      <ul class="menu-list">
        <li><span class="menu-item-name"><span class="icon-chicken">🍗</span> Ayam Biasa</span><span class="menu-price">18K</span></li>
        <li><span class="menu-item-name"><span class="icon-chicken">🍗</span> Ayam Special</span><span class="menu-price">20K</span></li>
        <li><span class="menu-item-name"><span class="icon-burger">🍔</span> Ayam Special Cheese</span><span class="menu-price">25K</span></li>
        <li><span class="menu-item-name"><span class="icon-burger">🍔</span> Double Ayam</span><span class="menu-price">21K</span></li>
        <li><span class="menu-item-name"><span class="icon-burger">🍔</span> Double Ayam Cheese</span><span class="menu-price">26K</span></li>
        <li><span class="menu-item-name"><span class="icon-burger">🍔</span> Double Ayam Special Cheese</span><span class="menu-price">28K</span></li>
      </ul>
    </section>

    <!-- Menu daging section -->
    <section class="menu-section" aria-label="Menu Burger Daging">
      <h2>BURGER DAGING</h2>
      <ul class="menu-list">
        <li><span class="menu-item-name"><span class="icon-burger">🍔</span> Daging Biasa</span><span class="menu-price">19K</span></li>
        <li><span class="menu-item-name"><span class="icon-burger">🍔</span> Daging Special</span><span class="menu-price">21K</span></li>
        <li><span class="menu-item-name"><span class="icon-burger">🍔</span> Daging Special Cheese</span><span class="menu-price">26K</span></li>
        <li><span class="menu-item-name"><span class="icon-burger">🍔</span> Double Daging</span><span class="menu-price">22K</span></li>
        <li><span class="menu-item-name"><span class="icon-burger">🍔</span> Double Daging Cheese</span><span class="menu-price">27K</span></li>
        <li><span class="menu-item-name"><span class="icon-burger">🍔</span> Double Daging Special</span><span class="menu-price">29K</span></li>
      </ul>
    </section>

    <!-- Call to action -->
    <section class="cta">
      <a href="https://wa.me/6281371477768" target="_blank" class="cta-phone" aria-label="Hubungi kami via WhatsApp">
        <svg style="width:22px;height:22px;" fill="#500900" viewBox="0 0 24 24">
          <path d="M12.041 2.003C6.482 2.008 2 6.496 2 12.052c0 2.06.654 4.042 1.886 5.67L2 22l4.406-1.844c1.593 1.017 3.41 1.621 5.66 1.623 5.56 0 10.043-4.492 10.047-10.067.004-5.555-4.476-10.007-10.072-10.006zm0 18.49c-1.787 0-3.465-.545-4.848-1.52l-.35-.237-2.635 1.104 1.112-2.56-.228-.354c-1.08-1.681-1.385-3.778-.792-5.72 1.26-4.364 7.01-5.532 10.063-2.48 3.052 3.028 2.008 8.571-2.442 10.428a7.196 7.196 0 0 1-2.028.94v-.001zm2.445-4.718c-.135-.067-.798-.39-.922-.434-.124-.045-.214-.068-.305.067-.09.134-.351.435-.43.524-.08.09-.16.101-.296.034-.134-.067-.565-.209-1.077-.664-.398-.355-.67-.793-.75-.927-.08-.134-.008-.206.059-.27.061-.06.134-.158.202-.236.068-.08.09-.135.135-.224.045-.089.022-.168-.012-.235-.034-.067-.305-.735-.417-1.008-.11-.268-.223-.232-.305-.237-.08-.006-.168-.007-.257-.007-.089 0-.234.034-.358.168-.123.134-.469.457-.469 1.114 0 .658.48 1.292.547 1.382.068.09.945 1.443 2.29 2.022.32.138.57.22.765.282.321.096.613.082.843.05.257-.036.798-.326.91-.641.113-.314.113-.583.08-.641-.033-.059-.122-.095-.257-.161z"></path>
        </svg>
        0813-7147-7768
      </a>
    </section>

    <!-- Delivery Platforms -->
    <section class="delivery-platforms" aria-label="Platform Pemesanan">
      <a href="https://gofood.link" target="_blank" aria-label="GoFood">
        <img src="https://seeklogo.com/images/G/go-food-logo-4248F4104A-seeklogo.com.png" alt="Logo GoFood" />
      </a>
      <a href="https://grab.com/food" target="_blank" aria-label="GrabFood">
        <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/d0/Grab_logo.svg/2560px-Grab_logo.svg.png" alt="Logo GrabFood" />
      </a>
    </section>
  </div>

  <!-- GSAP Animation CDN -->
  <script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.11.4/gsap.min.js"></script>
  <script>
    // Animasi floating burger
    gsap.to(".animated-burger", {
      y: -20,
      duration: 3,
      ease: "power1.inOut",
      yoyo: true,
      repeat: -1,
    });

    // Animasi judul utama flicker effect
    gsap.to(".main-title", {
      textShadow: "0 0 20px #fff, 0 0 30px #fff, 0 0 40px #f6c85f, 0 0 70px #f6c85f, 0 0 80px #f6c85f",
      duration: 2,
      repeat: -1,
      yoyo: true,
      ease: "power2.inOut",
    });
  </script>
</body>
</html>
