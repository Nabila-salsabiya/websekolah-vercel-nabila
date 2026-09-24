vue
<template>
  <div class="landing-page">

    <!-- ========== HERO ========== -->
    <section
      class="bg-gradient-to-br from-pink-400 to-pink-600 text-white text-center
             px-6 py-20 md:px-10 lg:py-24 flex flex-col items-center gap-5"
    >
      <h1
        class="text-4xl md:text-5xl lg:text-6xl font-bold leading-tight"
      >
        Selamat Datang di Toko Kami
      </h1>

      <p
        class="text-lg md:text-xl max-w-2xl opacity-90 leading-relaxed"
      >
        Temukan produk terbaik dengan kualitas premium dan harga bersahabat
      </p>

      <!-- Video -->
      <div class="w-full flex justify-center my-4">
        <video
          controls
          loop
          class="w-full max-w-[480px] rounded-xl shadow-lg"
        >
          <source
            src="https://www.w3schools.com/html/mov_bbb.mp4"
            type="video/mp4"
          />
          Browser Anda tidak mendukung video.
        </video>
      </div>

      <!-- Tombol -->
      <router-link
        to="/product"
        class="inline-block bg-white text-pink-600
               px-8 py-3 rounded-full font-bold text-base
               shadow-md transition duration-300
               hover:-translate-y-1 hover:shadow-xl
               focus:outline-none focus:ring-4 focus:ring-white/40"
      >
        Lihat Produk 🛒
      </router-link>
    </section>

    <!-- ========== FITUR ========== -->
    <section class="py-16 px-6 text-center bg-gray-50">

      <h2
        class="mb-10 text-3xl md:text-4xl font-bold text-gray-800"
      >
        Kenapa Pilih Kami?
      </h2>

      <div
        class="flex flex-wrap justify-center gap-8
               max-w-6xl mx-auto"
      >

        <!-- Kartu 1 -->
        <div
          class="flex-1 min-w-[250px] max-w-sm
                 p-8 rounded-xl
                 bg-purple-100 border-l-4 border-purple-500
                 shadow-md
                 transition duration-300
                 hover:-translate-y-2 hover:shadow-xl"
        >
          <span class="block text-5xl mb-4">
            🚚
          </span>

          <h3 class="text-xl font-bold text-gray-800 mb-3">
            Gratis Ongkir
          </h3>

          <p class="text-gray-600 text-base leading-relaxed">
            Pengiriman gratis ke seluruh Indonesia tanpa minimum belanja
          </p>
        </div>

        <!-- Kartu 2 -->
        <div
          class="flex-1 min-w-[250px] max-w-sm
                 p-8 rounded-xl
                 bg-pink-100 border-l-4 border-pink-500
                 shadow-md
                 transition duration-300
                 hover:-translate-y-2 hover:shadow-xl"
        >
          <span class="block text-5xl mb-4">
            ⭐
          </span>

          <h3 class="text-xl font-bold text-gray-800 mb-3">
            Kualitas Terjamin
          </h3>

          <p class="text-gray-600 text-base leading-relaxed">
            Semua produk melewati quality control ketat sebelum dikirim
          </p>
        </div>

        <!-- Kartu 3 -->
        <div
          class="flex-1 min-w-[250px] max-w-sm
                 p-8 rounded-xl
                 bg-sky-100 border-l-4 border-sky-500
                 shadow-md
                 transition duration-300
                 hover:-translate-y-2 hover:shadow-xl"
        >
          <span class="block text-5xl mb-4">
            💬
          </span>

          <h3 class="text-xl font-bold text-gray-800 mb-3">
            Support 24/7
          </h3>

          <p class="text-gray-600 text-base leading-relaxed">
            Tim kami siap membantu kapan saja melalui chat dan telepon
          </p>
        </div>

      </div>
    </section>

  </div>
</template>

<script setup>
// Tidak ada script yang diperlukan
</script>