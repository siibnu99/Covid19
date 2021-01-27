<template>
  <div class="home">
    <Hero />
    <Said />
    <About />
    <Data />
  </div>
</template>

<script>
// @ is an alias to /src
import Hero from "@/components/Hero.vue";
import Said from "@/components/Said.vue";
import Data from "@/components/Data.vue";
import About from "@/components/About.vue";

export default {
  name: "Home",
  components: {
    Hero,
    Said,
    About,
    Data,
  },
};
</script>
