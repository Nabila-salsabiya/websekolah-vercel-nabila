<template>
  <nav class="w-full shadow-md flex items-center justify-between px-4">
    <!-- <div class=""> -->
    <!-- <div class="jus gap-10 py-4 justify-between">  -->
    <p class="flex justify-start text-3xl">Nabila-olshop</p>
    <div class="flex justify-end items-center gap-10 py-4">
      <RouterLink to="/" class="text-neutral-200 font-semibold hover:text-pink-500">
        Landing
      </RouterLink>

      <RouterLink to="/product" class="text-neutral-200 font-semibold hover:text-pink-500">
        Product
      </RouterLink>

      <RouterLink to="/about" class="text-neutral-200 font-semibold hover:text-pink-500">
        About
      </RouterLink>

      <RouterLink to="/contact" class="text-neutral-200 font-semibold hover:text-pink-500">
        Contact
      </RouterLink>
    </div>
  </nav>
</template>
