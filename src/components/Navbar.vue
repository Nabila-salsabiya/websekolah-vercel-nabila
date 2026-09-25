<template>
  <nav class="w-full shadow-md">
    <!-- <div class=""> -->
      <!-- <div class="jus gap-10 py-4 justify-between">  -->
        <p class="flex justify-start text-3xl">Nabila-olshop</p>
        <div class="flex justify-end items-center gap-10 py-4"> 
          
      <RouterLink
        to="/"
        class="text-gray-700 font-medium hover:text-pink-500"
      >
        Landing
      </RouterLink>

      <RouterLink
        to="/product"
        class="text-gray-700 font-medium hover:text-pink-500"
      >
        Product
      </RouterLink>

      <RouterLink
        to="/about"
        class="text-gray-700 font-medium hover:text-pink-500"
      >
        About
      </RouterLink>

      <RouterLink
        to="/contact"
        class="text-gray-700 font-medium hover:text-pink-500"
      >
        Contact
      </RouterLink>

    </div>
  </nav>
</template>