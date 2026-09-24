<script setup>
import ProductCard from '../components/ProductCard.vue'
const daftarProduk = [
 { id: 1, nama: 'lipstik Diorr', harga: 750000, gambar:
'https://i.pinimg.com/1200x/9f/a6/65/9fa6656e53402d7af42a96bd43bff541.jpg' },
 { id: 2, nama: 'Blush Diorrr', harga: 350000, gambar:
 'https://i.pinimg.com/736x/c1/48/39/c148393080af81ca87a83d14fc387666.jpg' },
{ id:3, nama: 'Farfum Diorr', harga: 8500000, gambar:
'https://i.pinimg.com/736x/07/71/ed/0771edee4246abc5f034c3be2e739e74.jpg' },
{ id:4, nama: 'Set make up Diorr', harga: 10000000, gambar:
'https://i.pinimg.com/736x/51/9e/7d/519e7df49d1200d19f0e45e175afda4c.jpg' },
]
</script>
<template>
 <main>
 <h1>Produk Kami</h1>
 <div class="grid">
 <ProductCard
 v-for="produk in daftarProduk"
 :key="produk.id"
 :nama="produk.nama"
 :harga="produk.harga"
 :gambar="produk.gambar"
 />
 </div>
 </main>
</template>
<style scoped>
.grid {
 display: flex;
 gap: 16px;
 flex-wrap: wrap;
}
</style>