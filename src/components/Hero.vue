<template>
  <div class="hero" data-aos="fade-down" data-aos-duration="1000">
    <div class="overlay bg-overlay"></div>
    <div
      class="flex flex-col md:flex-row container mx-auto p-4 px-4 md:px-28 h-screen items-center z-20 justify-center"
      data-aos="fade-right"
      data-aos-duration="2000"
    >
      <div class="w-full md:w-1/2">
        <img src="@/assets/img/hero.png" class="w-full" alt="" />
      </div>
      <div
        class="w-full md:w-1/2 text-center md:text-left"
        data-aos="fade-left"
        data-aos-duration="2000"
      >
        <h1 class="md:text-4xl text-2xl font-extrabold text-white z-20">
          Informasi Tentang <span class="text-yellow-400">Covid19</span> Dengan
          API
          <a
            href="https://kawalcorona.com/api/"
            class="hborder-b-2 border-blue-500"
            target="_blank"
            >Kawalcorona.com</a
          >
        </h1>
        <h2 class="pl-2 pt-2 text-white text-extrabold my-5 dark:text-white">
          Semoga korona lekas hilang dan bisa menjalankan aktifitas sebagaiamana
          mestinya. Lihat data terbaru tentang Covid 19
        </h2>
        <button
          class="bg-blue-600 text-white font-semibold p-3 rounded-lg shadow-2xl transform hover:scale-105 transition duration-500 hover:bg-blue-700 flex items-center focus:outline-none mx-auto md:mx-0"
        >
          Pantau Corona
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
    </div>
  </div>
</template>

<script>
export default {
  name: "Hero",
};
</script>

<style lang="scss">
.overlay {
  position: absolute;
  width: 100%;
  height: 100%;
  top: 0px;
  left: 0px;
  -webkit-transform: skewY(-8deg);
  transform: skewY(-8deg);
  -webkit-transform-origin: 0;
  transform-origin: 0;
  z-index: -1;
}
.bg-overlay1 {
  background-image: url(../assets/svg/bg.svg);
  background-size: cover;
}
.bg-overlay {
  background-image: url(../assets/svg/bg.svg),
    linear-gradient(95deg, rgb(29, 25, 235), rgb(39, 207, 236));
  background-size: cover;
}
.dark .dark-bg-overlay {
  background-image: url(../assets/svg/bg.svg),
    linear-gradient(95deg, rgb(39, 39, 92), rgb(16, 78, 88));
  background-size: cover;
}
.dark .bg-overlay {
  background-image: url(../assets/svg/bg.svg),
    linear-gradient(95deg, rgb(39, 39, 92), rgb(16, 78, 88));
  background-size: cover;
}
</style>