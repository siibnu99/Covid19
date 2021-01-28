<template>
  <div class="home">
    <Heropage page="Kontak" />
    <Contacts />
    <Footer />
  </div>
</template>

<script>
// @ is an alias to /src
import Heropage from "@/components/Heropage.vue";
import Contacts from "@/components/Contact.vue";
import Footer from "@/components/Footer.vue";

export default {
  name: "Home",
  components: {
    Heropage,
    Contacts,
    Footer,
  },
};
</script>
