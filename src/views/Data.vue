<template>
  <div class="home">
    <Heropage page="Data Hari Ini" />
    <Datas />
    <Abouts />
    <Footer />
  </div>
</template>

<script>
// @ is an alias to /src
import Heropage from "@/components/Heropage.vue";
import Datas from "@/components/Data.vue";
import Abouts from "@/components/About.vue";
import Footer from "@/components/Footer.vue";

export default {
  name: "Home",
  components: {
    Heropage,
    Datas,
    Abouts,
    Footer,
  },
};
</script>
