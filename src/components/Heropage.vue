<template>
  <div class="hero" data-aos="fade-down" data-aos-duration="1000">
    <div class="overlay bg-overlay"></div>
    <div
      class="flex flex-col md:flex-row container mx-auto p-4 px-4 md:px-28 h-96 items-center z-20 justify-center"
      data-aos="fade-right"
      data-aos-duration="2000"
    >
      <div
        class="w-full text-center"
        data-aos="fade-left"
        data-aos-duration="2000"
      >
        <h1
          class="md:text-4xl text-2xl font-extrabold text-white z-20 border-b-4 inline-block"
        >
          {{ page }}
        </h1>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Hero",
  props: {
    page: String,
  },
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