<template>
  <div class="contact-page">
    <!-- Banner -->
    <section class="banner">
      <h1>Hubungi Kami</h1>
    </section>

    <!-- Konten utama: 2 kolom -->
    <section class="contact-content">
      <!-- Kolom Info Kontak -->
      <div class="info-kontak">
        <h2>Info Kontak</h2>

        <ul>
          <li>📍 Jl. Bandung Kota No. 62</li>
          <li>📞 (813) 892184428</li>
          <li>✉️ info@SalsabiyaDIOR.com</li>
        </ul>

        <p class="jam-operasional">
          🕐 Senin – Jumat: 08.00 – 17.00
        </p>
      </div>

      <!-- Kolom Formulir Kontak -->
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
            <label for="email">Email</label>
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

          <button type="submit" class="btn-kirim">
            Kirim 🚀
          </button>
        </form>
      </div>
    </section>
  </div>
</template>

<script setup>
// Belum membutuhkan logic.
// Form hanya digunakan sebagai tampilan.
</script>

<style scoped>
/* Banner */
.banner {
  background-color: bisque;
  color: white;
  text-align: center;
  padding: 3rem 1rem;
}

.banner h1 {
  margin: 0;
}

/* Layout 2 kolom */
.contact-content {
  display: flex;
  gap: 2rem;
  padding: 3rem 2rem;
  max-width: 1000px;
  margin: 0 auto;
  align-items: flex-start;
}

/* Kolom Info Kontak */
.info-kontak {
  flex: 1;
}

.info-kontak h2,
.form-card h2 {
  margin-top: 0;
  margin-bottom: 1.5rem;
}

.info-kontak ul {
  list-style: none;
  padding: 0;
  margin: 0;
}

.info-kontak li {
  margin-bottom: 1rem;
  font-size: 1.1rem;
}

.jam-operasional {
  margin-top: 1.5rem;
  color: #555;
}

/* Kolom Formulir */
.form-card {
  flex: 1;
  padding: 2rem;
  border-radius: 12px;
  box-shadow: 0 2px 12px rgba(0, 0, 0, 0.1);
  background-color: #fff;
}

/* Styling field */
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
  padding: 0.75rem 1rem;
  border-radius: 8px;
  border: 1px solid #ccc;
  font-size: 1rem;
  font-family: inherit;
  box-sizing: border-box;
  transition: border-color 0.3s;
}

input:focus,
textarea:focus {
  outline: none;
  border-color: #4a90d9;
}

/* Tombol Kirim */
.btn-kirim {
  background: #4a90d9;
  color: white;
  border: none;
  border-radius: 999px;
  padding: 0.75rem 2rem;
  font-size: 1rem;
  cursor: pointer;
  width: 100%;
  margin-top: 0.5rem;
  transition: background 0.3s;
}

.btn-kirim:hover {
  background: #357abd;
}

/* Responsive untuk HP */
@media (max-width: 768px) {
  .contact-content {
    flex-direction: column;
    padding: 2rem 1rem;
  }

  .info-kontak,
  .form-card {
    width: 100%;
    box-sizing: border-box;
  }

  .form-card {
    padding: 1.5rem;
  }
}