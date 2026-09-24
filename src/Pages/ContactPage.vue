
<template>
  <div class="contact-page">
    <!-- Banner senada dengan AboutPage -->
    <section class="banner">
      <h1>Hubungi Kami</h1>
    </section>

    <!-- Konten utama: 2 kolom sejajar -->
    <section class="contact-content">
      <!-- Kolom 1: Info Kontak -->
      <div class="info-kontak">
        <h2>Info Kontak</h2>
        <ul>
          <li>📍 Jl. Bandung kota No 62</li>
          <li>📞 (813) 892184428 </li>
          <li>✉️ info@SalsabiyaDIOR.com</li>
        </ul>
        <p class="jam-operasional">
          🕐 Senin – Jumat: 08.00 – 17.00
        </p>
      </div>

      <!-- Kolom 2: Formulir Kontak (tampilan saja) -->
      <div class="form-card">
        <h2>Kirim Pesan</h2>
        <form @submit.prevent>
          <div class="form-group">
            <label for="nama">Nama</label>
            <input
              id="nama"
              type="text"
              placeholder="Masukkan nama kamu"
            />
          </div>

          <div class="form-group">
            <label for="email">email</label>
            <input
              id="email"
              type="email"
              placeholder="salsabiya@email.com"
            />
          </div>

          <div class="form-group">
            <label for="pesan">Pesan</label>
            <textarea
              id="pesan"
              rows="5"
              placeholder="Tulis pesan kamu di sini..."
            ></textarea>
          </div>

          <!-- Tombol bergaya pil, belum perlu berfungsi -->
          <button type="submit" class="btn-kirim">
            Kirim 🚀
          </button>
        </form>
      </div>
    </section>
  </div>
</template>

<script setup>
// Belum perlu logic apapun — form ini CUKUP TAMPILAN saja
</script>

<style scoped>
/* Banner — samakan warna dengan Landing Page & About Page */
.banner {
  background-color: bisque;   /* Ganti sesuai tema warna kalian */
  color: rgb(237, 12, 12);
  text-align: center;
  padding: 3rem 1rem;
}

/* Layout 2 kolom sejajar */
.contact-content {
  display: flex;               /* <-- 2 kolom sejajar */
  gap: 2rem;                   /* <-- jarak antar kolom */
  padding: 3rem 2rem;
  max-width: 1000px;
  margin: 0 auto;
  align-items: flex-start;
}

/* Kolom Info Kontak */
.info-kontak {
  flex: 1;
}

.info-kontak ul {
  list-style: none;
  padding: 0;
}

.info-kontak li {
  margin-bottom: 1rem;
  font-size: 1.1rem;
}

.jam-operasional {
  margin-top: 1.5rem;
  color: whitesmoke;
}

/* Kolom Formulir — tampil seperti kartu */
.form-card {
  flex: 1;
  padding: 2rem;              /* <-- padding supaya terlihat kartu */
  border-radius: 12px;        /* <-- sudut membulat */
  box-shadow: 0 2px 12px rgba(0, 0, 0, 0.1);
  background-color: #fff;
}

/* Styling field formulir */
.form-group {
  margin-bottom: 1.2rem;
}

.form-group label {
  display: block;
  margin-bottom: 0.4rem;
  font-weight: 600;
  color: #333;
}

input,
textarea {
  width: 100%;
  padding: 0.75rem 1rem;      /* <-- padding dalam field */
  border-radius: 8px;         /* <-- sudut membulat */
  border: 1px solid #ccc;     /* <-- border tipis */
  font-size: 1rem;
  transition: border-color 0.3s;
  box-sizing: border-box;
}

input:focus,
textarea:focus {
  outline: none;
  border-color: #4a90d9;      /* Warna fokus senada tema */
}

/* Tombol Kirim bergaya pil */
.btn-kirim {
  background: #4a90d9;        /* <-- warna senada Landing Page */
  color: white;               /* <-- teks putih */
  border: none;
  border-radius: 999px;       /* <-- bentuk pil */
  padding: 0.75rem 2rem;
  font-size: 1rem;
  cursor: pointer;
  width: 100%;
  margin-top: 0.5rem;
  transition: background 0.3s;
}

.btn-kirim:hover {
  background: #357abd;        /* Warna lebih gelap saat hover */
}
</style>

