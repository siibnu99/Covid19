<template>
  <div
    class="said bg-blue-50 dark:bg-gray-600 bg-overlay1"
    data-aos="fade-up"
    data-aos-duration="1000"
  >
    <div
      class="flex flex-col md-:flex-row container mx-auto p-4 px-4 md:px-28 h-auto md:h-screen items-center justify-center"
    >
      <div class="w-full text-center dark:text-white space-y-4">
        <h1
          class="text-lg md:text-2xl font-bold text-blue-600 dark:text-yellow-400"
          data-aos="fade-up"
          data-aos-duration="1000"
        >
          Mau menghubungi saya?
        </h1>
        <h2
          class="text-sm md:text-lg font-medium"
          data-aos="fade-up"
          data-aos-duration="1000"
        >
          Hubungi saya dengan media yang tertera dibawah.
        </h2>
        <textarea
          class="w-full p-2 shadow border-none focus:outline-none focus:ring-blue-500 dark:bg-gray-600 font-medium"
          rows="10"
          v-model="state.chat"
          placeholder="Silahkan Masukan Pesan di form ini!"
        ></textarea>
      </div>
      <a
        :href="'https://wa.me/6281939495630?text=' + state.chat"
        target="_blank"
        class="bg-white dark:bg-gray-400 dark:text-white dark:hover:bg-yellow-500 px-5 py-2 rounded-lg mt-10 font-bold text-blue-700 hover:bg-blue-700 hover:text-white hover:scale-110 transform transition duration-700"
        v-if="state.chat"
      >
        Kirim</a
      >
    </div>
  </div>
</template>

<script>
import { reactive } from "vue";
export default {
  name: "Said",
  setup() {
    const state = reactive({
      chat: "",
    });
    return {
      state,
    };
  },
};
</script>

<style>
</style>