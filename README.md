<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Website Saya</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0; padding: 0;
      background-color: #f5f3f0; /* warna latar belakang soft */
    }

    header {
      background-color: #a9745b; /* coklat susu gelap */
      color: white;
      padding: 30px 0;
      text-align: center;
    }

    nav {
      background-color: #c8a98d; /* coklat susu medium */
      display: flex;
      justify-content: center;
    }

    nav a, .dropbtn {
      color: white;
      text-decoration: none;
      padding: 14px 20px;
      font-weight: bold;
      display: inline-block;
    }

    nav a:hover, .dropdown:hover .dropbtn {
      background-color: #a9745b;
      border-radius: 5px;
    }

    /* Dropdown */
    .dropdown {
      position: relative;
      display: inline-block;
    }
    .dropdown-content {
      display: none;
      position: absolute;
      background: #fff;
      min-width: 160px;
      box-shadow: 0px 8px 16px rgba(0,0,0,0.2);
      z-index: 1;
      border-radius: 5px;
    }
    .dropdown-content a {
      color: #333;
      padding: 10px 14px;
      display: block;
      text-decoration: none;
    }
    .dropdown-content a:hover {
      background: #f2e6da;
    }
    .dropdown:hover .dropdown-content {
      display: block;
    }

    section {
      display: none;
      padding: 40px;
      text-align: center;
    }
    section.active {
      display: block;
    }

    .card {
      background: white;
      padding: 20px;
      border-radius: 10px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.1);
      display: inline-block;
    }

    button {
      background: #a9745b;
      color: white;
      padding: 8px 14px;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      margin-top: 10px;
    }
    button:hover {
      background: #8c5e47;
    }

    input {
      padding: 5px;
      margin: 5px;
      border-radius: 4px;
      border: 1px solid #ccc;
    }
  </style>
</head>
<body>

  <header>
    <h1>⋆˚✿˖° Website Anita Putri Lestari 🧸༄.°</h1>
    <p>Blog Website Saya</p>
  </header>

  <nav>
    <a href="#" onclick="showPage('beranda')">Beranda</a>
    <a href="#" onclick="showPage('tentang')">Tentang Saya</a>
    <a href="#" onclick="showPage('jadwal')">Jadwal Pelajaran</a>
    <a href="#" onclick="showPage('syair')">Syair Lagu</a>
    <div class="dropdown">
      <a href="#" class="dropbtn">Menghitung ▼</a>
      <div class="dropdown-content">
        <a href="#" onclick="showPage('luas')">Luas Persegi</a>
        <a href="#" onclick="showPage('volume')">Volume Kotak</a>
      </div>
    </div>
  </nav>

  <!-- Halaman -->
  <section id="beranda" class="active">
    <div class="card">
      <h2>Haiii Selamat Datang!~</h2>
      <p>Blog ini merupakan beranda Anita Putri Lestari siswi SMKN 1 Kota Tangerang.</p>
    </div>
  </section>

  <section id="tentang">
    <div class="card">
      <h2>Tentang Saya</h2>
      <p>Halo, kenalin nama aku Anita dan ini adalah web pribadi tentang diri aku.</p>
    </div>
  </section>

  <section id="jadwal">
    <div class="card">
      <h2>Jadwal Pelajaran</h2>
          <p>Berikut jadwal mingguan aku di kelas XII DKV 2.</p>
 </div>
  </section>

  <section id="syair">
    <div class="card">
      <h2>Syair Lagu</h2>
      <p>Berisikan syair lagu favoriteku!!!</p>
    </div>
  </section>

  <section id="luas">
    <div class="card">
      <h2>Menghitung Luas Persegi</h2>
      <p>Masukkan panjang sisi:</p>
          </div>
  </section>

  <section id="volume">
    <div class="card">
      <h2>Menghitung Volume Kotak</h2>
      <p>Masukkan panjang, lebar, tinggi:</p>

    </div>
  </section>

  <script>
    function showPage(pageId) {
      let pages = document.querySelectorAll("section");
      pages.forEach(p => p.classList.remove("active"));
      document.getElementById(pageId).classList.add("active");
    }

   
      </script>

</body>
</html>
