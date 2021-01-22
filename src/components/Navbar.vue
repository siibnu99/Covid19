<template>
  <nav class="navbar">
    <div class="container mx-auto p-4 flex justify-between text-gray-700">
      <div class="logo">
        <router-link to="/"
          ><img src="@/assets/svg/logo.svg" alt="Logo" class="w-24"
        /></router-link>
      </div>
      <div class="menu font-semibold text-sm space-x-5">
        <router-link to="/">Home</router-link>
        <router-link to="/about">About</router-link>
        <router-link to="/contact">Contact</router-link>
        <a href="" target="_blank">View Git</a>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: "navbar",
};
</script>

<style>
</style>