<template>
  <div class="dark:bg-gray-700">
    <Navbar />
    <router-view />
    <div class="toogle-mode fixed z-30 bottom-20 right-10">
      <div
        class="border-2 w-12 h-12 rounded-full bg-gray-600 dark:bg-white dark:text-gray-400 text-white flex justify-center items-center focus:outline-none c-mode cursor-pointer"
        @click="cMode()"
      >
        <svg
          xmlns="http://www.w3.org/2000/svg"
          width="20"
          height="20"
          fill="currentColor"
          class="bi bi-brightness-high-fill"
          viewBox="0 0 16 16"
        >
          <path
            d="M12 8a4 4 0 1 1-8 0 4 4 0 0 1 8 0zM8 0a.5.5 0 0 1 .5.5v2a.5.5 0 0 1-1 0v-2A.5.5 0 0 1 8 0zm0 13a.5.5 0 0 1 .5.5v2a.5.5 0 0 1-1 0v-2A.5.5 0 0 1 8 13zm8-5a.5.5 0 0 1-.5.5h-2a.5.5 0 0 1 0-1h2a.5.5 0 0 1 .5.5zM3 8a.5.5 0 0 1-.5.5h-2a.5.5 0 0 1 0-1h2A.5.5 0 0 1 3 8zm10.657-5.657a.5.5 0 0 1 0 .707l-1.414 1.415a.5.5 0 1 1-.707-.708l1.414-1.414a.5.5 0 0 1 .707 0zm-9.193 9.193a.5.5 0 0 1 0 .707L3.05 13.657a.5.5 0 0 1-.707-.707l1.414-1.414a.5.5 0 0 1 .707 0zm9.193 2.121a.5.5 0 0 1-.707 0l-1.414-1.414a.5.5 0 0 1 .707-.707l1.414 1.414a.5.5 0 0 1 0 .707zM4.464 4.465a.5.5 0 0 1-.707 0L2.343 3.05a.5.5 0 1 1 .707-.707l1.414 1.414a.5.5 0 0 1 0 .708z"
          />
        </svg>
      </div>
    </div>
  </div>
</template>
<script>
import Navbar from "@/components/Navbar.vue";
import { onMounted, watch } from "vue";
export default {
  name: "App",
  components: { Navbar },
  setup() {
    function applyMode() {
      localStorage.theme === "light" || !localStorage.theme
        ? document.querySelector("html").classList.remove("dark")
        : document.querySelector("html").classList.add("dark");
    }
    function cMode() {
      if (localStorage.theme === "dark") {
        localStorage.theme = "light";
      } else {
        localStorage.theme = "dark";
      }
      applyMode();
    }
    onMounted(applyMode);

    return {
      cMode,
    };
  },
};
</script>
<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Montserrat:wght@100;200;300;400;500;600;700;800;900&display=swap");
#app {
  font-family: Montserrat, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
nav.xl .router-link-active {
  border-bottom: 2px solid white;
}
</style>
