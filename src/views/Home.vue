<template>
  <div class="home">
    <Hero />
    <Said />
    <About />
    <Data />
    <Penularan />
    <Pencegahan />
    <Footer />
  </div>
</template>

<script>
// @ is an alias to /src
import Hero from "@/components/Hero.vue";
import Said from "@/components/Said.vue";
import About from "@/components/About.vue";
import Penularan from "@/components/Penularan.vue";
import Data from "@/components/Data.vue";
import Pencegahan from "@/components/Pencegahan.vue";
import Footer from "@/components/Footer.vue";

export default {
  name: "Home",
  components: {
    Hero,
    Said,
    About,
    Data,
    Penularan,
    Pencegahan,
    Footer,
  },
};
</script>
