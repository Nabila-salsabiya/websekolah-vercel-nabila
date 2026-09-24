<template>
  <div class="about-page">
    <!-- Banner -->
    <section class="banner">
      <h1>Tentang Kami</h1>
    </section>

    <!-- Bagian 1: Cerita Kami (layout 2 kolom) -->
    <section class="cerita-kami">
      <div class="cerita-content">
        <div class="cerita-teks">
          <h2>Cerita Kami</h2>
          <p>
          
            Toko kami berdiri dari kecintaan kami terhadap [produk dior] 
            set make up yang sangat bagus flowless, memakai make up dior dijamin muka mu menyala
            make up kami make up yang bagus jujur dbahan" nya  ...
          </p>
        </div>
        <div class="cerita-gambar">
          <!-- Placeholder gambar atau <img> -->
          <img src="https://i.pinimg.com/736x/30/06/d9/3006d9e3e80756becfb8bc410210fbb0.jpg" alt="cerita-gambar"/>

        
        </div>
    </div>
    </section>

    <!-- Bagian 2: Tim Kami -->
    <section class="tim-kami">
      <h2>Tim Kami</h2>
      <div class="tim-grid">
        <!--
          v-for untuk loop array daftarTim
          :key harus unik (bisa pakai index atau nama)
        -->
        <TeamCard
          v-for="anggota in daftarTim"
          :key="anggota.nama"
          :nama="anggota.nama"
          :jabatan="anggota.jabatan"
        />
      </div>
    </section>
    </div>
</template>

<script setup>
import { ref } from 'vue'
import TeamCard from '../components/TeamCard.vue'

// Data anggota tim — ganti dengan nama kelompok kalian!
const daftarTim = ref([
  { nama: 'Nabila', jabatan: 'Project Manager' },
  { nama: 'cinta', jabatan: 'Frontend Developer' },
  { nama: 'kayla', jabatan: 'UI/UX Designer' },
  { nama: 'alya', jabatan: 'Manager2' },
  // Tambahkan anggota lain jika perlu
])
</script>

<style scoped>
.banner {
  background-color: beige;   /* Sesuaikan dengan warna Landing Page */
  color: white;
  text-align: center;
  padding: 3rem 1rem;
}

/* Layout 2 kolom untuk Cerita Kami */
.cerita-content {
  display: flex;               /* <-- flexbox 2 kolom */
  align-items: center;         /* <-- rata tengah vertikal */
  gap: 2rem;                   /* <-- jarak antar kolom */
  padding: 3rem 2rem;
  max-width: 1000px;
  margin: 0 auto;
}

.cerita-teks {
  flex: 1;
  min-width: 200px;                     /* <-- berbagi lebar merata */
}

.cerita-gambar {
  display: flex;
gap: 2rem;
padding: 2rem;
flex-wrap: wrap;       
justify-content: center;              
}

.cerita-gambar img {
  width: 100%;
  max-width: 400px;
  height: 350px;
  object-fit: cover;
  border-radius: 20px;
}

.img-placeholder {
  background-color: #e0e0e0;
  height: 250px;
  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: 12px;
  font-size: 1.2rem;
  color: lightpink;
}

/* Grid untuk kartu tim */
.tim-kami {
  padding: 3rem 2rem;
  text-align: center;
}

.tim-grid {
  display: flex;
  justify-content: center;
  gap: 2rem;
  flex-wrap: wrap;
  margin-top: 2rem;
}
</style>