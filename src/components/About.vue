<template>
  <div class="hero">
    <div class="flex container mx-auto p-4 h-screen items-center">
      <div class="w-1/2">
        <h1
          class="text-4xl font-extrabold text-blue-600 dark:text-white capitalize"
        >
          COVID 19 merupakan virus yang berbeda dari
          <span class="text-yellow-400">virus biasanya</span>
        </h1>
        <h2 class="pl-2 pt-2 text-gray-600 text-extrabold my-5 dark:text-white">
          Virus Corona atau severe acute respiratory syndrome coronavirus 2
          (SARS-CoV-2) adalah virus yang menyerang sistem pernapasan. Penyakit
          karena infeksi virus ini disebut COVID-19. Virus Corona bisa
          menyebabkan gangguan ringan pada sistem pernapasan, infeksi paru-paru
          yang berat, hingga kematian.
        </h2>
        <button
          class="bg-blue-600 text-white font-semibold p-3 rounded-lg shadow-2xl transform hover:scale-105 transition duration-500 hover:bg-blue-700 flex items-center focus:outline-none"
        >
          Pelajari Lebih Lanjut
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="18"
            height="18"
            fill="currentColor"
            class="bi bi-arrow-down-right-circle ml-2 font-extrabold"
            viewBox="0 0 16 16"
          >
            <path
              fill-rule="evenodd"
              d="M1 8a7 7 0 1 0 14 0A7 7 0 0 0 1 8zm15 0A8 8 0 1 1 0 8a8 8 0 0 1 16 0zM5.854 5.146a.5.5 0 1 0-.708.708L9.243 9.95H6.475a.5.5 0 1 0 0 1h3.975a.5.5 0 0 0 .5-.5V6.475a.5.5 0 1 0-1 0v2.768L5.854 5.146z"
            />
          </svg>
        </button>
      </div>
      <div class="w-1/2">
        <img src="@/assets/svg/corona.svg" class="w-full" alt="" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Hero",
};
</script>

<style>
</style>