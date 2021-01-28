<template>
  <div class="home">
    <Heropage page="Aspek Corona" />
    <Penularan />
    <Pencegahan />
    <Footer />
  </div>
</template>

<script>
// @ is an alias to /src
import Heropage from "@/components/Heropage.vue";
import Penularan from "@/components/Penularan.vue";
import Pencegahan from "@/components/Pencegahan.vue";
import Footer from "@/components/Footer.vue";

export default {
  name: "Home",
  components: {
    Heropage,
    Penularan,
    Pencegahan,
    Footer,
  },
};
</script>
