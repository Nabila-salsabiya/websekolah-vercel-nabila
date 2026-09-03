
<template>
  <!-- Wrapper card untuk satu anggota tim -->
  <div class="team-card">
    <!-- Avatar lingkaran: bisa pakai gambar atau inisial -->
    <div class="avatar">
      <!-- Tampilkan inisial dari nama, misal "A" dari "Andi" -->
      {{ nama.charAt(0) }}
    </div>
    <h3>{{ nama }}</h3>
    <p>{{ jabatan }}</p>
  </div>
</template>

<script setup>
// defineProps menerima data dari komponen parent
defineProps({
  nama: {
    type: String,
    required: true
  },
  jabatan: {
    type: String,
    required: true
  }
})
</script>

<style scoped>
.team-card {
  text-align: center;
  padding: 1.5rem;
  border-radius: 12px;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
}

.avatar {
  width: 80px;
  height: 80px;
  border-radius: 50%;          /* <-- membuat lingkaran */
  background-color: #4a90d9;   /* sesuaikan warna tema */
  color: white;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 2rem;
  font-weight: bold;
  margin: 0 auto 1rem;
}
</style>

