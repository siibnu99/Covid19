<template>
  <div class="home">
    <Heropage page="About" />
    <Said />
    <Abouts />
    <Footer />
  </div>
</template>

<script>
// @ is an alias to /src
import Heropage from "@/components/Heropage.vue";
import Said from "@/components/Said.vue";
import Abouts from "@/components/About.vue";
import Footer from "@/components/Footer.vue";

export default {
  name: "Home",
  components: {
    Heropage,
    Said,
    Abouts,
    Footer,
  },
};
</script>
