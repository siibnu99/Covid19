<template>
  <div class="footer bg-gray-600 bg-overlay1 mb-10 md:mb-0">
    <div
      class="flex flex-col container mx-auto p-4 px-0 md:px-28 h-52 text-center content-center space-y-5"
    >
      <div class="mx-auto">
        <router-link to="/"
          ><img src="@/assets/svg/logo.svg" alt="Logo" class="w-52 text-white"
        /></router-link>
      </div>
      <h2 class="text-gray-50 text-sm">Copryright &copy 2020 Siibnu</h2>
      <div class="space-x-5 text-white font-semibold">
        <router-link to="/">Home</router-link>
        <router-link to="/about">About</router-link>
        <router-link to="/data">Data Hari Ini</router-link>
        <router-link to="/aspek">Aspek</router-link>
        <router-link to="/contact">Contact</router-link>
      </div>
      <h1></h1>
    </div>
  </div>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style>
</style>