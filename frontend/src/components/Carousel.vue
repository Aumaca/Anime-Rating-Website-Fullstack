<script setup lang="ts">
import img1 from '../assets/imgs/kaguya.jpg';
import img2 from '../assets/imgs/kimetsu.jpg';
import img3 from '../assets/imgs/jujutsu.jpg';

const carouselInterval:number = 5000;
</script>

<template>
    <div class="carousel-container col-12 overflow-hidden">
        <div id="carouselExampleAutoplaying" class="carousel slide" data-bs-ride="carousel" :data-bs-interval="carouselInterval">
            <div class="carousel-inner" style="height: 500px;">
                <div class="carousel-item active">
                    <div class="d-flex justify-content-center text-center slide">
                        <img :src="img1" class="d-block img-fluid" alt="...">
                        <div class="position-absolute bottom-0 px-5 text-start text-light fs-5">
                            <h5><span class="caption">Kaguya-sama</span></h5>
                            <p><span class="caption">Love Is War -The First Kiss that Never Ends will be in theatres from
                                    February 14 in the US</span></p>
                        </div>
                    </div>
                </div>
                <div class="carousel-item">
                    <div class="d-flex justify-content-center text-center slide">
                        <img :src="img2" class="d-block img-fluid" alt="...">
                        <div class="position-absolute bottom-0 px-5 text-start text-light fs-5">
                            <h5><span class="caption">Third slide label</span></h5>
                            <p><span class="caption">Some representative placeholder content for the third slide.</span></p>
                        </div>
                    </div>
                </div>
                <div class="carousel-item">
                    <div class="d-flex justify-content-center text-center slide">
                        <img :src="img3" class="d-block img-fluid" alt="...">
                        <div class="position-absolute bottom-0 px-5 text-start text-light fs-5">
                            <h5><span class="caption">Third slide label</span></h5>
                            <p><span class="caption">Some representative placeholder content for the third slide.</span></p>
                        </div>
                    </div>
                </div>
            </div>
            <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleAutoplaying"
                data-bs-slide="prev">
                <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                <span class="visually-hidden">Previous</span>
            </button>
            <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleAutoplaying"
                data-bs-slide="next">
                <span class="carousel-control-next-icon" aria-hidden="true"></span>
                <span class="visually-hidden">Next</span>
            </button>
        </div>
    </div>
</template>

<style scoped>
.carousel-container {
    border-bottom: 3px solid #198754;
}

.caption {
    background-color: rgba(0, 0, 0, 0.534);
}

img {
    object-fit: cover;
    width: 100vw;
}

.slide {
    height: 500px;
    width: 100vw;
}
</style>