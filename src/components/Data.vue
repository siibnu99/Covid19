<template>
  <div class="said bg-overlay1" data-aos="zoom-in-up" data-aos-duration="1000">
    <div
      class="flex container mx-auto p-4 px-4 md:px-28 h-auto md:h-screen items-center"
    >
      <div class="w-full text-center dark:text-white">
        <h1
          class="text-2xl font-bold text-blue-600 dark:text-yellow-400"
          data-aos="fade-up"
          data-aos-duration="2000"
        >
          Data COVID 19 Hari ini!
        </h1>
        <h2
          class="text-lg font-medium"
          data-aos="fade-up"
          data-aos-duration="2000"
        >
          Data covid ini diperoleh dari API Kawalcorona.com
        </h2>
        <div
          class="flex justify-between flex-col md:flex-row text-gray-700 space-y-10 md:space-y-0 md:space-x-10 mt-20 text-left"
        >
          <div
            class="w-full md:w-1/2 text-center"
            data-aos="fade-right"
            data-aos-duration="2000"
          >
            <h1 class="text-2xl dark:text-white font-bold">Data Global</h1>
            <div
              class="text-left flex mt-10 justify-between flex-col space-y-2"
            >
              <div
                class="bg-white flex items-center space-x-5 p-5 shadow-lg rounded-md"
              >
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  width="48"
                  height="48"
                  fill="currentColor"
                  class="bi bi-emoji-frown text-blue-700 shadow-2xl"
                  viewBox="0 0 16 16"
                >
                  <path
                    d="M8 15A7 7 0 1 1 8 1a7 7 0 0 1 0 14zm0 1A8 8 0 1 0 8 0a8 8 0 0 0 0 16z"
                  />
                  <path
                    d="M4.285 12.433a.5.5 0 0 0 .683-.183A3.498 3.498 0 0 1 8 10.5c1.295 0 2.426.703 3.032 1.75a.5.5 0 0 0 .866-.5A4.498 4.498 0 0 0 8 9.5a4.5 4.5 0 0 0-3.898 2.25.5.5 0 0 0 .183.683zM7 6.5C7 7.328 6.552 8 6 8s-1-.672-1-1.5S5.448 5 6 5s1 .672 1 1.5zm4 0c0 .828-.448 1.5-1 1.5s-1-.672-1-1.5S9.448 5 10 5s1 .672 1 1.5z"
                  />
                </svg>
                <div>
                  <h1 class="text-sm font-semibold">Total Kasus</h1>
                  <h1 class="text-2xl font-bold">
                    {{ state.dataGlobal.kasus }}
                  </h1>
                </div>
              </div>
              <div
                class="bg-white flex items-center space-x-5 p-5 shadow-lg rounded-md"
              >
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  width="48"
                  height="48"
                  fill="currentColor"
                  class="bi bi-emoji-dizzy text-red-700"
                  viewBox="0 0 16 16"
                >
                  <path
                    d="M8 15A7 7 0 1 1 8 1a7 7 0 0 1 0 14zm0 1A8 8 0 1 0 8 0a8 8 0 0 0 0 16z"
                  />
                  <path
                    d="M9.146 5.146a.5.5 0 0 1 .708 0l.646.647.646-.647a.5.5 0 0 1 .708.708l-.647.646.647.646a.5.5 0 0 1-.708.708l-.646-.647-.646.647a.5.5 0 1 1-.708-.708l.647-.646-.647-.646a.5.5 0 0 1 0-.708zm-5 0a.5.5 0 0 1 .708 0l.646.647.646-.647a.5.5 0 1 1 .708.708l-.647.646.647.646a.5.5 0 1 1-.708.708L5.5 7.207l-.646.647a.5.5 0 1 1-.708-.708l.647-.646-.647-.646a.5.5 0 0 1 0-.708zM10 11a2 2 0 1 1-4 0 2 2 0 0 1 4 0z"
                  />
                </svg>
                <div>
                  <h1 class="text-sm font-semibold">Total Kematian</h1>
                  <h1 class="text-2xl font-bold">
                    {{ state.dataGlobal.mati }}
                  </h1>
                </div>
              </div>
              <div
                class="bg-white flex items-center space-x-5 p-5 shadow-lg rounded-md"
              >
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  width="48"
                  height="48"
                  fill="currentColor"
                  class="bi bi-emoji-heart-eyes text-green-700"
                  viewBox="0 0 16 16"
                >
                  <path
                    d="M8 15A7 7 0 1 1 8 1a7 7 0 0 1 0 14zm0 1A8 8 0 1 0 8 0a8 8 0 0 0 0 16z"
                  />
                  <path
                    d="M11.315 10.014a.5.5 0 0 1 .548.736A4.498 4.498 0 0 1 7.965 13a4.498 4.498 0 0 1-3.898-2.25.5.5 0 0 1 .548-.736h.005l.017.005.067.015.252.055c.215.046.515.108.857.169.693.124 1.522.242 2.152.242.63 0 1.46-.118 2.152-.242a26.58 26.58 0 0 0 1.109-.224l.067-.015.017-.004.005-.002zM4.756 4.566c.763-1.424 4.02-.12.952 3.434-4.496-1.596-2.35-4.298-.952-3.434zm6.488 0c1.398-.864 3.544 1.838-.952 3.434-3.067-3.554.19-4.858.952-3.434z"
                  />
                </svg>
                <div>
                  <h1 class="text-sm font-semibold">Total Sembuh</h1>
                  <h1 class="text-2xl font-bold">
                    {{ state.dataGlobal.sembuh }}
                  </h1>
                </div>
              </div>
            </div>
          </div>
          <div
            class="w-full md:w-1/2 text-center"
            data-aos="fade-left"
            data-aos-duration="2000"
          >
            <h1 class="text-2xl dark:text-white font-bold">Data Indonesia</h1>
            <div
              class="text-left flex mt-10 justify-between flex-col space-y-2"
            >
              <div
                class="bg-white flex items-center space-x-5 p-5 shadow-lg rounded-md"
              >
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  width="48"
                  height="48"
                  fill="currentColor"
                  class="bi bi-emoji-frown text-blue-700 shadow-2xl"
                  viewBox="0 0 16 16"
                >
                  <path
                    d="M8 15A7 7 0 1 1 8 1a7 7 0 0 1 0 14zm0 1A8 8 0 1 0 8 0a8 8 0 0 0 0 16z"
                  />
                  <path
                    d="M4.285 12.433a.5.5 0 0 0 .683-.183A3.498 3.498 0 0 1 8 10.5c1.295 0 2.426.703 3.032 1.75a.5.5 0 0 0 .866-.5A4.498 4.498 0 0 0 8 9.5a4.5 4.5 0 0 0-3.898 2.25.5.5 0 0 0 .183.683zM7 6.5C7 7.328 6.552 8 6 8s-1-.672-1-1.5S5.448 5 6 5s1 .672 1 1.5zm4 0c0 .828-.448 1.5-1 1.5s-1-.672-1-1.5S9.448 5 10 5s1 .672 1 1.5z"
                  />
                </svg>
                <div>
                  <h1 class="text-sm font-semibold">Total Kasus</h1>
                  <h1 class="text-2xl font-bold">
                    {{ state.dataIndonesia.positif }}
                  </h1>
                </div>
              </div>
              <div
                class="bg-white flex items-center space-x-5 p-5 shadow-lg rounded-md"
              >
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  width="48"
                  height="48"
                  fill="currentColor"
                  class="bi bi-emoji-dizzy text-red-700"
                  viewBox="0 0 16 16"
                >
                  <path
                    d="M8 15A7 7 0 1 1 8 1a7 7 0 0 1 0 14zm0 1A8 8 0 1 0 8 0a8 8 0 0 0 0 16z"
                  />
                  <path
                    d="M9.146 5.146a.5.5 0 0 1 .708 0l.646.647.646-.647a.5.5 0 0 1 .708.708l-.647.646.647.646a.5.5 0 0 1-.708.708l-.646-.647-.646.647a.5.5 0 1 1-.708-.708l.647-.646-.647-.646a.5.5 0 0 1 0-.708zm-5 0a.5.5 0 0 1 .708 0l.646.647.646-.647a.5.5 0 1 1 .708.708l-.647.646.647.646a.5.5 0 1 1-.708.708L5.5 7.207l-.646.647a.5.5 0 1 1-.708-.708l.647-.646-.647-.646a.5.5 0 0 1 0-.708zM10 11a2 2 0 1 1-4 0 2 2 0 0 1 4 0z"
                  />
                </svg>
                <div>
                  <h1 class="text-sm font-semibold">Total Kematian</h1>
                  <h1 class="text-2xl font-bold">
                    {{ state.dataIndonesia.meninggal }}
                  </h1>
                </div>
              </div>
              <div
                class="bg-white flex items-center space-x-5 p-5 shadow-lg rounded-md"
              >
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  width="48"
                  height="48"
                  fill="currentColor"
                  class="bi bi-emoji-heart-eyes text-green-700"
                  viewBox="0 0 16 16"
                >
                  <path
                    d="M8 15A7 7 0 1 1 8 1a7 7 0 0 1 0 14zm0 1A8 8 0 1 0 8 0a8 8 0 0 0 0 16z"
                  />
                  <path
                    d="M11.315 10.014a.5.5 0 0 1 .548.736A4.498 4.498 0 0 1 7.965 13a4.498 4.498 0 0 1-3.898-2.25.5.5 0 0 1 .548-.736h.005l.017.005.067.015.252.055c.215.046.515.108.857.169.693.124 1.522.242 2.152.242.63 0 1.46-.118 2.152-.242a26.58 26.58 0 0 0 1.109-.224l.067-.015.017-.004.005-.002zM4.756 4.566c.763-1.424 4.02-.12.952 3.434-4.496-1.596-2.35-4.298-.952-3.434zm6.488 0c1.398-.864 3.544 1.838-.952 3.434-3.067-3.554.19-4.858.952-3.434z"
                  />
                </svg>
                <div>
                  <h1 class="text-sm font-semibold">Total Sembuh</h1>
                  <h1 class="text-2xl font-bold">
                    {{ state.dataIndonesia.sembuh }}
                  </h1>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import axios from "axios";
import { reactive } from "vue";
export default {
  name: "Said",
  setup() {
    const state = reactive({
      dataGlobal: {
        sembuh: {},
        mati: {},
        kasus: {},
      },
      dataIndonesia: {},
    });
    axios
      .get("https://api.kawalcorona.com/sembuh/")
      .then(function (response) {
        state.dataGlobal.sembuh = response.data.value;
      })
      .catch(function (error) {
        console.log("Error");
      });
    axios
      .get("https://api.kawalcorona.com/positif/")
      .then(function (response) {
        state.dataGlobal.kasus = response.data.value;
      })
      .catch(function (error) {
        console.log("Error");
      });
    axios
      .get("https://api.kawalcorona.com/meninggal/")
      .then(function (response) {
        state.dataGlobal.mati = response.data.value;
      })
      .catch(function (error) {
        console.log("Error");
      });
    axios
      .get("https://api.kawalcorona.com/indonesia")
      .then(function (response) {
        state.dataIndonesia = response.data[0];
      })
      .catch(function (error) {
        console.log("Error");
      });
    return {
      state,
    };
  },
};
</script>

<style>
</style>