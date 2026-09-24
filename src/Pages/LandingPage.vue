<template>
  <div class="contact-page">

    <!-- ========== HERO / BANNER ========== -->
    <section
      class="bg-gradient-to-br from-pink-400 to-pink-600
             text-white text-center
             px-6 py-16 md:px-10 lg:py-20"
    >
      <h1
        class="text-4xl md:text-5xl font-bold leading-tight"
      >
        Hubungi Kami
      </h1>

      <p
        class="mt-4 text-lg md:text-xl max-w-2xl
               mx-auto opacity-90 leading-relaxed"
      >
        Kami siap membantu menjawab pertanyaan dan kebutuhan kamu
      </p>
    </section>

    <!-- ========== KONTEN KONTAK ========== -->
    <section class="py-16 px-6 bg-gray-50">

      <div
        class="max-w-6xl mx-auto
               flex flex-col lg:flex-row
               gap-8"
      >

        <!-- ========== INFO KONTAK ========== -->
        <div
          class="flex-1
                 bg-purple-100
                 border-l-4 border-purple-500
                 rounded-xl
                 p-8
                 shadow-md
                 transition duration-300
                 hover:-translate-y-1 hover:shadow-xl"
        >
          <h2
            class="text-2xl md:text-3xl
                   font-bold text-gray-800 mb-6"
          >
            Info Kontak
          </h2>

          <ul class="space-y-5">

            <li class="flex items-start gap-3">
              <span class="text-2xl">📍</span>

              <div>
                <p class="font-semibold text-gray-800">
                  Alamat
                </p>

                <p class="text-gray-600">
                  Jl. Bandung Kota No. 62
                </p>
              </div>
            </li>

            <li class="flex items-start gap-3">
              <span class="text-2xl">📞</span>

              <div>
                <p class="font-semibold text-gray-800">
                  Telepon
                </p>

                <p class="text-gray-600">
                  (813) 892184428
                </p>
              </div>
            </li>

            <li class="flex items-start gap-3">
              <span class="text-2xl">✉️</span>

              <div>
                <p class="font-semibold text-gray-800">
                  Email
                </p>

                <p class="text-gray-600">
                  info@SalsabiyaDIOR.com
                </p>
              </div>
            </li>

          </ul>

          <!-- Jam Operasional -->
          <div
            class="mt-8
                   bg-white/70
                   rounded-lg
                   p-4"
          >
            <p class="font-semibold text-gray-800">
              🕐 Jam Operasional
            </p>

            <p class="text-gray-600 mt-1">
              Senin – Jumat: 08.00 – 17.00
            </p>
          </div>
        </div>


        <!-- ========== FORM KONTAK ========== -->
        <div
          class="flex-1
                 bg-white
                 rounded-xl
                 p-8
                 shadow-md
                 transition duration-300
                 hover:shadow-xl"
        >
          <h2
            class="text-2xl md:text-3xl
                   font-bold text-gray-800 mb-6"
          >
            Kirim Pesan
          </h2>

          <form @submit.prevent>

            <!-- Nama -->
            <div class="mb-5">
              <label
                for="nama"
                class="block mb-2
                       font-semibold text-gray-700"
              >
                Nama
              </label>

              <input
                id="nama"
                type="text"
                placeholder="Masukkan nama kamu"
                class="w-full
                       px-4 py-3
                       rounded-lg
                       border border-gray-300
                       text-gray-800
                       transition duration-300
                       focus:outline-none
                       focus:border-pink-400
                       focus:ring-2
                       focus:ring-pink-200"
              />
            </div>


            <!-- Email -->
            <div class="mb-5">
              <label
                for="email"
                class="block mb-2
                       font-semibold text-gray-700"
              >
                Email
              </label>

              <input
                id="email"
                type="email"
                placeholder="salsabiya@email.com"
                class="w-full
                       px-4 py-3
                       rounded-lg
                       border border-gray-300
                       text-gray-800
                       transition duration-300
                       focus:outline-none
                       focus:border-pink-400
                       focus:ring-2
                       focus:ring-pink-200"
              />
            </div>


            <!-- Pesan -->
            <div class="mb-5">
              <label
                for="pesan"
                class="block mb-2
                       font-semibold text-gray-700"
              >
                Pesan
              </label>

              <textarea
                id="pesan"
                rows="5"
                placeholder="Tulis pesan kamu di sini..."
                class="w-full
                       px-4 py-3
                       rounded-lg
                       border border-gray-300
                       text-gray-800
                       resize-none
                       transition duration-300
                       focus:outline-none
                       focus:border-pink-400
                       focus:ring-2
                       focus:ring-pink-200"
              ></textarea>
            </div>


            <!-- Tombol -->
            <button
              type="submit"
              class="w-full
                     bg-pink-500
                     hover:bg-pink-600
                     text-white
                     px-8 py-3
                     rounded-full
                     font-bold
                     text-base
                     shadow-md
                     transition duration-300
                     hover:-translate-y-1
                     hover:shadow-xl
                     focus:outline-none
                     focus:ring-4
                     focus:ring-pink-200"
            >
              Kirim 🚀
            </button>

          </form>
        </div>

      </div>
    </section>

  </div>
</template>

<script setup>
// Tidak ada logic yang diperlukan.
// Form masih hanya digunakan sebagai tampilan.
</script>