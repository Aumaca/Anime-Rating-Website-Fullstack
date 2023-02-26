<script setup lang="ts">
import Crunchyroll_logo from "../assets/imgs/logos/Crunchyroll_logo.png"
import funimation_logo from "../assets/imgs/logos/funimation_logo.png"
import Hulu_Logo from "../assets/imgs/logos/Hulu_Logo.png"
import netflix_logo from "../assets/imgs/logos/netflix_logo.png"
</script>

<template>
  <div class="container-md p-3">
    <!-- Title -->
    <h1 class="display-3 mb-3">About</h1>

    <!-- Main -->
    <div class="px-4 py-3 text-center">
      <h1 class="d-block mx-auto mb-4"><i class="ri-star-half-line ms-2"></i></h1>
      <h1 class="display-5 fw-bold">Discover new good anime</h1>
      <div class="col-lg-6 mx-auto">
        <p class="lead mb-4">
          Are you in struggle to find a decent anime nowadays?<br>
          Here in AnimeRating, you are able to
          find the animes reviews and check for good animes that will not waste your time!
        </p>
        <div class="d-flex justify-content-center">
          <a href="/reviews" class="btn btn-outline-success btn-lg px-4 d-flex align-items-center gap-2">See reviews <i
              class="ri-arrow-right-line"></i></a>
        </div>
      </div>
    </div>

    <!-- Partners -->
    <div class="partners mt-5 d-flex flex-column justify-content-center">
      <h4 class="text-center mb-4">Our partners</h4>
      <div class="d-flex flex-column flex-sm-row justify-content-center align-items-center gap-5">
        <a href="https://www.crunchyroll.com/" target="_blank"><img :src="Crunchyroll_logo"></a>
        <a href="https://www.funimation.com/" target="_blank"><img :src="funimation_logo"></a>
        <a href="https://www.hulu.com/hub/tv" target="_blank"><img :src="Hulu_Logo"></a>
        <a href="https://www.netflix.com/br/browse/genre/7424" target="_blank"><img :src="netflix_logo"></a> 
      </div>
    </div>
  </div>
</template>


<style scoped>
.partners img {
  filter: grayscale(1);
  transition: 0.3s ease-in-out;
  height: 100%;
  width: 80px;
  cursor: pointer;
}

.partners img:hover {
  filter: grayscale(0);
  height: 100%;
  width: 80px;
}
</style>