<!doctype html>
<html lang="id">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Layout Responsif - Febriano Aldo</title>

  <!-- Bootstrap 5 CSS CDN -->
  <link
    href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css"
    rel="stylesheet"
    integrity="sha384-QWTKZyjpPEjISv5WaRU9OFeRpok6YctnYmDr5pNlyT2bRjXh0JMhjY6hW+ALEwIH"
    crossorigin="anonymous"
  />

  <style>
    /* Bikin footer “lengket” di bawah saat konten sedikit */
    html, body { height: 100%; }
    body { display: flex; flex-direction: column; }
    main { flex: 1 0 auto; }
    footer { flex-shrink: 0; }
    /* Contoh kecil biar kartu terlihat rapi */
    .content-card { min-height: 220px; }
  </style>
</head>
<body>

  <!-- Header / Navbar -->
  <nav class="navbar navbar-expand-lg bg-body-tertiary border-bottom">
    <div class="container">
      <a class="navbar-brand fw-semibold" href="#">Febriano Aldo</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navMain" aria-controls="navMain" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navMain">
        <ul class="navbar-nav ms-auto">
          <li class="nav-item"><a class="nav-link active" aria-current="page" href="#">Beranda</a></li>
          <li class="nav-item"><a class="nav-link" href="#kolom-1">Tentang</a></li>
          <li class="nav-item"><a class="nav-link" href="#kolom-2">Kontak</a></li>
        </ul>
      </div>
    </div>
  </nav>

  <!-- Konten Utama -->
  <main class="py-4">
    <div class="container">
      <div class="row g-4">

        <!-- Kolom 1 -->
        <section id="kolom-1" class="col-12 col-lg-6">
          <div class="card content-card shadow-sm h-100">
            <div class="card-body">
              <h5 class="card-title">Informasi 1 — Tentang Saya</h5>
              <p class="card-text">
                Halo! Saya <strong>Febriano Aldo</strong>. Ini contoh kolom pertama.
                Layout menggunakan <em>grid</em> Bootstrap: pada layar kecil (mobile) kolom menumpuk (12),
                pada layar lebar menjadi 2 kolom (6–6).
              </p>
              <ul class="mb-0">
                <li>Responsif: <code>.col-12</code> di mobile, <code>.col-lg-6</code> di desktop</li>
                <li>Komponen: Navbar, Card, Container, Row, Col</li>
                <li>CDN: Bootstrap 5.3.3</li>
              </ul>
            </div>
          </div>
        </section>

        <!-- Kolom 2 -->
        <section id="kolom-2" class="col-12 col-lg-6">
          <div class="card content-card shadow-sm h-100">
            <div class="card-body">
              <h5 class="card-title">Informasi 2 — Kontak</h5>
              <p class="card-text">
                Kamu bisa mengubah isi kolom ini sesuai kebutuhan tugas. Berikut data tugasmu:
              </p>
              <div class="border rounded p-3">
                <div><strong>Nama:</strong> Febriano Aldo</div>
                <div><strong>Email:</strong> <a href="mailto:febrianoaldo19@gmail.com">febrianoaldo19@gmail.com</a></div>
                <div><strong>GitHub:</strong> <a href="https://github.com/aldoo1nonly" target="_blank" rel="noopener">aldoo1nonly</a></div>
              </div>
              <p class="mt-3 mb-0">
                Silakan tambahkan gambar, daftar proyek, atau tautan portofolio di sini.
              </p>
            </div>
          </div>
        </section>

      </div>
    </div>
  </main>

  <!-- Footer -->
  <footer class="bg-body-tertiary border-top py-3">
    <div class="container text-center small">
      © <span id="year"></span> Febriano Aldo · Dibuat dengan Bootstrap 5
    </div>
  </footer>

  <!-- Bootstrap JS -->
  <script
    src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"
    integrity="sha384-YvpcrYf0tY3lHB60NNkmXc5s9fDVZLESaAA55NDzOxhy9GkcIdslK1eN7N6jIeHz"
    crossorigin="anonymous"
  ></script>
  <script>
    document.getElementById('year').textContent = new Date().getFullYear();
  </script>
</body>
</html>


