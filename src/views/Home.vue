<template>
  <div class="home">
    <Hero />
    <Said />
    <About />
    <Data />
    <Penularan />
  </div>
</template>

<script>
// @ is an alias to /src
import Hero from "@/components/Hero.vue";
import Said from "@/components/Said.vue";
import About from "@/components/About.vue";
import Penularan from "@/components/Penularan.vue";
import Data from "@/components/Data.vue";

export default {
  name: "Home",
  components: {
    Hero,
    Said,
    About,
    Data,
    Penularan,
  },
};
</script>
