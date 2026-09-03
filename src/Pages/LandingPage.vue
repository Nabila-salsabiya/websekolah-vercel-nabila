
<template>
  <div class="landing-page">
    <!-- ========== HERO ========== -->
    <section class="hero bg-indigo-500 p-[100px] flex-col items-center text-center
    text-white gap-[18px]">
      <h1 class="text-[62pt] text-center">Selamat Datang di Toko Kami</h1>
      <p class="hero-subtitle">
        Temukan produk terbaik dengan kualitas premium dan harga bersahabat
      </p>
      <center>
        <video controls width="480" loop>
 <source src="https://www.w3schools.com/html/mov_bbb.mp4" type="video/mp4" />
        </video>
      </center>
      <router-link to="/product" class="btn-hero">    Lihat Produk 🛒
      </router-link>
    </section>

    <!-- ========== FITUR ========== -->
    <section class="fitur">
      <h2>Kenapa Pilih Kami?</h2>

      <div class="fitur-container">
        <!-- Kartu 1: Warna ungu muda -->
        <div class="fitur-card card-1">
          <span class="fitur-icon">🚚</span>
          <h3>Gratis Ongkir</h3>
          <p>Pengiriman gratis ke seluruh Indonesia tanpa minimum belanja</p>
        </div>

        <!-- Kartu 2: Warna pink muda -->
        <div class="fitur-card card-2">
          <span class="fitur-icon">⭐</span>
          <h3>Kualitas Terjamin</h3>
          <p>Semua produk melewati quality control ketat sebelum dikirim</p>
        </div>

        <!-- Kartu 3: Warna biru muda -->
        <div class="fitur-card card-3">
          <span class="fitur-icon">💬</span>
          <h3>Support 24/7</h3>
          <p>Tim kami siap membantu kapan saja melalui chat dan telepon</p>
        </div>
      </div>
    </section>
  </div>
</template>

<script setup>
</script>

<style scoped>
.hero {
  background: linear-gradient(135deg, #db7dbf, #d371a1);
  color: white;
  text-align: center;
  padding: 5rem 2rem;
}

.hero h1 {
  font-size: 2.5rem;
  margin-bottom: 1rem;
}

.hero-subtitle {
  font-size: 1.2rem;
  margin-bottom: 2rem;
  opacity: 0.9;
}

.btn-hero {
  display: inline-block;
  background: white;
  color: #0f9b8e;
  text-decoration: none;
  padding: 0.85rem 2.5rem;
  border-radius: 999px;
  font-weight: bold;
  font-size: 1rem;
  transition: transform 0.3s, box-shadow 0.3s;
}

/* Efek hover: tombol terangkat */
.btn-hero:hover {
  transform: translateY(-3px);
  box-shadow: 0 6px 20px rgba(0, 0, 0, 0.2);
}

/* ===== FITUR SECTION ===== */
.fitur {
  padding: 4rem 2rem;
  text-align: center;
  background-color: #f9fafb;
}

.fitur h2 {
  margin-bottom: 2rem;
  font-size: 1.8rem;
  color: #333;
}

/* Container kartu sejajar */
.fitur-container {
  display: flex;
  gap: 2rem;
  flex-wrap: wrap;
  justify-content: center;
  max-width: 1000px;
  margin: 0 auto;
}

/* Style dasar semua kartu */
.fitur-card {
  flex: 1;
  min-width: 250px;
  padding: 2rem;
  border-radius: 12px;
  box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
  transition: transform 0.3s, box-shadow 0.3s;
}

.fitur-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 8px 25px rgba(0, 0, 0, 0.15);
}

/* ===== WARNA MASING-MASING KARTU ===== */

/* Kartu 1: Ungu muda */
.card-1 {
  background-color: #ede9fe;
  border-left: 4px solid #8b5cf6;
}

/* Kartu 2: Pink muda */
.card-2 {
  background-color: #fce7f3;
  border-left: 4px solid #ec4899;
}

/* Kartu 3: Biru muda */
.card-3 {
  background-color: #e0f2fe;
  border-left: 4px solid #0ea5e9;
}

.fitur-icon {
  font-size: 2.5rem;
  display: block;
  margin-bottom: 1rem;
}

.fitur-card h3 {
  margin-bottom: 0.5rem;
  color: #333;
}

.fitur-card p {
  color: #666;
  font-size: 0.95rem;
}
</style>

