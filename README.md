<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Kantin Laris</title>

  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      font-family: Arial, sans-serif;
      background: #f8f5ef;
      color: #222;
    }

    header {
      background: linear-gradient(135deg, #2f1b12, #8b3f14);
      color: white;
      padding: 50px 20px;
      text-align: center;
    }

    header h1 {
      font-size: 42px;
      margin-bottom: 10px;
    }

    header p {
      font-size: 18px;
      opacity: 0.9;
    }

    .hero-button {
      display: inline-block;
      margin-top: 25px;
      background: #ffb703;
      color: #2f1b12;
      padding: 14px 24px;
      border-radius: 30px;
      text-decoration: none;
      font-weight: bold;
    }

    .section {
      max-width: 1100px;
      margin: auto;
      padding: 40px 20px;
    }

    .section-title {
      text-align: center;
      margin-bottom: 25px;
    }

    .section-title h2 {
      font-size: 32px;
      color: #2f1b12;
    }

    .section-title p {
      color: #666;
      margin-top: 8px;
    }

    .category {
      display: flex;
      justify-content: center;
      gap: 10px;
      flex-wrap: wrap;
      margin-bottom: 30px;
    }

    .category span {
      background: white;
      padding: 10px 18px;
      border-radius: 25px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.08);
      font-weight: bold;
    }

    .menu-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
      gap: 22px;
    }

    .card {
      background: white;
      border-radius: 20px;
      overflow: hidden;
      box-shadow: 0 8px 20px rgba(0,0,0,0.10);
      transition: 0.3s;
      position: relative;
    }

    .card:hover {
      transform: translateY(-5px);
    }

    .badge {
      position: absolute;
      top: 14px;
      left: 14px;
      background: #e63946;
      color: white;
      padding: 6px 12px;
      border-radius: 20px;
      font-size: 12px;
      font-weight: bold;
    }

    .food-img {
      height: 150px;
      background: linear-gradient(135deg, #ffb703, #fb8500);
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 64px;
    }

    .card-content {
      padding: 20px;
    }

    .card-content h3 {
      font-size: 22px;
      margin-bottom: 8px;
      color: #2f1b12;
    }

    .desc {
      color: #666;
      font-size: 14px;
      min-height: 42px;
      margin-bottom: 12px;
    }

    .rating {
      font-size: 14px;
      color: #f59e0b;
      margin-bottom: 10px;
    }

    .bottom {
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 12px;
    }

    .price {
      font-size: 20px;
      font-weight: bold;
      color: #d35400;
    }

    .order-btn {
      background: #25d366;
      color: white;
      text-decoration: none;
      padding: 10px 14px;
      border-radius: 20px;
      font-size: 14px;
      font-weight: bold;
    }

    .info-box {
      margin-top: 40px;
      background: #2f1b12;
      color: white;
      border-radius: 22px;
      padding: 28px;
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
      gap: 20px;
      text-align: center;
    }

    .info-box h3 {
      color: #ffb703;
      margin-bottom: 8px;
    }

    footer {
      text-align: center;
      padding: 25px;
      background: #1f120c;
      color: white;
      margin-top: 30px;
    }
  </style>
</head>

<body>

  <header>
    <h1>Kantin Laris</h1>
    <p>Menu makanan dan minuman favorit, praktis dipesan, siap antar di area kantin.</p>
    <a class="hero-button" href="#menu">Lihat Menu</a>
  </header>

  <section class="section" id="menu">
    <div class="section-title">
      <h2>Daftar Menu</h2>
      <p>Pilih menu favoritmu dan pesan langsung melalui WhatsApp.</p>
    </div>

    <div class="category">
      <span>Makanan Berat</span>
      <span>Mie & Bakso</span>
      <span>Minuman</span>
      <span>Cemilan</span>
    </div>

    <div class="menu-grid">

      <div class="card">
        <div class="badge">Best Seller</div>
        <div class="food-img">🍛</div>
        <div class="card-content">
          <h3>Nasi Goreng Spesial</h3>
          <p class="desc">Nasi goreng gurih dengan telur, ayam, kerupuk, dan acar.</p>
          <p class="rating">★★★★★ 4.9</p>
          <div class="bottom">
            <span class="price">Rp15.000</span>
            <a class="order-btn" href="https://wa.me/6281234567890?text=Halo%20saya%20mau%20pesan%20Nasi%20Goreng%20Spesial">Pesan</a>
          </div>
        </div>
      </div>

      <div class="card">
        <div class="food-img">🍜</div>
        <div class="card-content">
          <h3>Mie Ayam Komplit</h3>
          <p class="desc">Mie ayam dengan topping ayam gurih, pangsit, dan sayuran.</p>
          <p class="rating">★★★★★ 4.8</p>
          <div class="bottom">
            <span class="price">Rp12.000</span>
            <a class="order-btn" href="https://wa.me/6281234567890?text=Halo%20saya%20mau%20pesan%20Mie%20Ayam%20Komplit">Pesan</a>
          </div>
        </div>
      </div>

      <div class="card">
        <div class="badge">Favorit</div>
        <div class="food-img">🍗</div>
        <div class="card-content">
          <h3>Ayam Geprek</h3>
          <p class="desc">Ayam crispy dengan sambal pedas, nasi hangat, dan lalapan.</p>
          <p class="rating">★★★★★ 4.9</p>
          <div class="bottom">
            <span class="price">Rp17.000</span>
            <a class="order-btn" href="https://wa.me/6281234567890?text=Halo%20saya%20mau%20pesan%20Ayam%20Geprek">Pesan</a>
          </div>
        </div>
      </div>

      <div class="card">
        <div class="food-img">🥤</div>
        <div class="card-content">
          <h3>Es Teh Manis</h3>
          <p class="desc">Es teh segar dengan rasa manis yang pas.</p>
          <p class="rating">★★★★☆ 4.7</p>
          <div class="bottom">
            <span class="price">Rp5.000</span>
            <a class="order-btn" href="https://wa.me/6281234567890?text=Halo%20saya%20mau%20pesan%20Es%20Teh%20Manis">Pesan</a>
          </div>
        </div>
      </div>

      <div class="card">
        <div class="food-img">🍌</div>
        <div class="card-content">
          <h3>Pisang Goreng</h3>
          <p class="desc">Pisang goreng hangat, renyah di luar dan lembut di dalam.</p>
          <p class="rating">★★★★☆ 4.6</p>
          <div class="bottom">
            <span class="price">Rp8.000</span>
            <a class="order-btn" href="https://wa.me/6281234567890?text=Halo%20saya%20mau%20pesan%20Pisang%20Goreng">Pesan</a>
          </div>
        </div>
      </div>

      <div class="card">
        <div class="food-img">☕</div>
        <div class="card-content">
          <h3>Kopi Susu</h3>
          <p class="desc">Kopi susu creamy cocok untuk teman belajar dan istirahat.</p>
          <p class="rating">★★★★★ 4.8</p>
          <div class="bottom">
            <span class="price">Rp10.000</span>
            <a class="order-btn" href="https://wa.me/6281234567890?text=Halo%20saya%20mau%20pesan%20Kopi%20Susu">Pesan</a>
          </div>
        </div>
      </div>

    </div>

    <div class="info-box">
      <div>
        <h3>Jam Buka</h3>
        <p>Senin - Jumat<br>08.00 - 16.00</p>
      </div>
      <div>
        <h3>Pemesanan</h3>
        <p>Pesan lewat WhatsApp<br>langsung diproses</p>
      </div>
      <div>
        <h3>Lokasi</h3>
        <p>Area Kantin Sekolah/Kampus<br>Meja depan kasir</p>
      </div>
    </div>
  </section>

  <footer>
    <p>© 2026 Kantin Laris. Makan enak, harga hemat.</p>
  </footer>

</body>
</html>
