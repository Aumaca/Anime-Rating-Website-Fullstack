<script setup lang="ts">
import kaguya from '../assets/imgs/kaguya.png';
import attackontitan from '../assets/imgs/attackontitan.jpg';
import codegeassposter from '../assets/imgs/codegeassposter.jpg';

function activeTag(evt: MouseEvent): void {
    const element = evt.target as HTMLElement;
    if (element.classList.contains("active")) {
        element.classList.remove("active");
        return
    }
    element.classList.add("active");
}
</script>

<template>
    <div class="container-md p-3">
        <!-- Title -->
        <h1 class="display-3 mb-3">Reviews</h1>

        <!-- Tags -->
        <div class="tags d-flex gap-3 overflow-x-scroll pb-2">
            <h6><span class="badge border rounded-pill bg-primary p-2" @click="activeTag">Adventure</span></h6>
            <h6><span class="badge border rounded-pill bg-success p-2" @click="activeTag">Action</span></h6>
            <h6><span class="badge border rounded-pill bg-pink p-2" @click="activeTag">Drama</span></h6>
            <h6><span class="badge border rounded-pill bg-warning p-2" @click="activeTag">Magic</span></h6>
            <h6><span class="badge border rounded-pill bg-dark p-2" @click="activeTag">Horror</span></h6>
            <h6><span class="badge border rounded-pill bg-someblue p-2" @click="activeTag">Psychological</span></h6>
            <h6><span class="badge border rounded-pill bg-info p-2" @click="activeTag">Sci-Fi</span></h6>
            <h6><span class="badge border rounded-pill bg-danger p-2" @click="activeTag">Romance</span></h6>
        </div>

        <!-- Reviews Grid -->
        <div class="reviews-container row justify-content-center justify-content-md-start gap-3 mt-4">

            <!-- Review -->
            <div class="card col-10 col-sm-5 col-lg-3 col-xl-2 p-0">
                <img :src="kaguya" class="card-img-top">
                <div class="card-body">
                    <h5 class="card-title">Kaguya-Sama: Love is War - Season 3</h5>
                    <p class="card-text">Some quick example text to build on the card title and make up the bulk of
                        the card's content.</p>
                    <div class="d-flex gap-2 overflow-x-scroll">
                        <span class="badge active border rounded-pill bg-danger p-2">Romance</span>
                    </div>
                </div>
            </div>

            <!-- Review -->
            <div class="card col-10 col-sm-5 col-lg-3 col-xl-2 p-0">
                <img :src="codegeassposter" class="card-img-top">
                <div class="card-body">
                    <h5 class="card-title">Code Geass: Lelouch of the Rebellion</h5>
                    <p class="card-text">
                        Code Geass: Lelouch of the Rebellion (コードギアス 反逆のルルーシュ Kōdo Giasu: Hangyaku no
                        Rurūshu?) é um anime da franquia Code Geass, de 2006, com 25 episódios, criado pela Sunrise.
                        Dirigida por Gorō Taniguchi e escrita por Ichirō Ōkouchi, ambos tendo anteriormente trabalhado em
                        outra série da Sunrise, chamado Planetes. Code Geass - Lelouch of the Rebellion apresenta character
                        design original da CLAMP.

                        A primeira temporada da série foi apresentada no Japão pela MBS em 6 de outubro de 2006 e foi
                        concluída em 28 de Julho de 2007, após 25 episódios. A segunda temporada e sequência da série, Code
                        Geass: Lelouch of the Rebellion R2 começou a ser apresentada nas redes MBS e TBS em 6 de abril de
                        2008.
                    </p>
                    <div class="d-flex gap-2 overflow-x-scroll">
                        <span class="badge active border rounded-pill bg-primary p-2">Adventure</span>
                        <span class="badge active border rounded-pill bg-success p-2">Action</span>
                        <span class="badge active border rounded-pill bg-success p-2">Action</span>
                    </div>
                </div>
            </div>

            <!-- Review -->
            <div class="card col-10 col-sm-5 col-lg-3 col-xl-2 p-0">
                <img :src="kaguya" class="card-img-top">
                <div class="card-body">
                    <h5 class="card-title">Kaguya-Sama: Love is War - Season 3</h5>
                    <p class="card-text">Some quick example text to build on the card title and make up the bulk of
                        the card's content.</p>
                    <div class="d-flex gap-2">
                        <span class="badge active border rounded-pill bg-danger p-2">Romance</span>
                    </div>
                </div>
            </div>

            <!-- Review -->
            <div class="card col-10 col-sm-5 col-lg-3 col-xl-2 p-0">
                <img :src="codegeassposter" class="card-img-top">
                <div class="card-body">
                    <h5 class="card-title">Code Geass: Lelouch of the Rebellion</h5>
                    <p class="card-text">
                        Code Geass: Lelouch of the Rebellion (コードギアス 反逆のルルーシュ Kōdo Giasu: Hangyaku no
                        Rurūshu?) é um anime da franquia Code Geass, de 2006, com 25 episódios, criado pela Sunrise.
                        Dirigida por Gorō Taniguchi e escrita por Ichirō Ōkouchi, ambos tendo anteriormente trabalhado em
                        outra série da Sunrise, chamado Planetes. Code Geass - Lelouch of the Rebellion apresenta character
                        design original da CLAMP.

                        A primeira temporada da série foi apresentada no Japão pela MBS em 6 de outubro de 2006 e foi
                        concluída em 28 de Julho de 2007, após 25 episódios. A segunda temporada e sequência da série, Code
                        Geass: Lelouch of the Rebellion R2 começou a ser apresentada nas redes MBS e TBS em 6 de abril de
                        2008.
                    </p>
                    <div class="d-flex gap-2">
                        <span class="badge active border rounded-pill bg-danger p-2">Romance</span>
                    </div>
                </div>
            </div>

            <!-- Review -->
            <div class="card col-10 col-sm-5 col-lg-3 col-xl-2 p-0">
                <img :src="kaguya" class="card-img-top">
                <div class="card-body">
                    <h5 class="card-title">Kaguya-Sama: Love is War - Season 3</h5>
                    <p class="card-text">Some quick example text to build on the card title and make up the bulk of
                        the card's content.</p>
                    <div class="d-flex gap-2">
                        <span class="badge active border rounded-pill bg-danger p-2">Romance</span>
                    </div>
                </div>
            </div>

            <!-- Review -->
            <div class="card col-10 col-sm-5 col-lg-3 col-xl-2 p-0">
                <img :src="codegeassposter" class="card-img-top">
                <div class="card-body">
                    <h5 class="card-title">Code Geass: Lelouch of the Rebellion</h5>
                    <p class="card-text">
                        Code Geass: Lelouch of the Rebellion (コードギアス 反逆のルルーシュ Kōdo Giasu: Hangyaku no
                        Rurūshu?) é um anime da franquia Code Geass, de 2006, com 25 episódios, criado pela Sunrise.
                        Dirigida por Gorō Taniguchi e escrita por Ichirō Ōkouchi, ambos tendo anteriormente trabalhado em
                        outra série da Sunrise, chamado Planetes. Code Geass - Lelouch of the Rebellion apresenta character
                        design original da CLAMP.

                        A primeira temporada da série foi apresentada no Japão pela MBS em 6 de outubro de 2006 e foi
                        concluída em 28 de Julho de 2007, após 25 episódios. A segunda temporada e sequência da série, Code
                        Geass: Lelouch of the Rebellion R2 começou a ser apresentada nas redes MBS e TBS em 6 de abril de
                        2008.
                    </p>
                    <div class="d-flex gap-2">
                        <span class="badge active border rounded-pill bg-danger p-2">Romance</span>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
::-webkit-scrollbar {
    height: 4px;
}

::-webkit-scrollbar-thumb {
    background-color: #bbb;
    border-radius: 2px;
}

.badge {
    cursor: pointer;
    filter: saturate(0);
    transition: 0.1s ease-in-out filter;
    user-select: none;
}

.badge.active {
    filter: saturate(1);
}

.bg-pink {
    background-color: #de5c9d;
}

.bg-someblue {
    background-color: #6e99b4;
}


.card img {
    max-height: 100px;
    object-fit: cover;
    object-position: top;
}

.card .card-title {
    display: -webkit-box;
    -webkit-line-clamp: 3;
    -webkit-box-orient: vertical;
    overflow: hidden;
    text-overflow: ellipsis;
}

.card p {
    display: -webkit-box;
    -webkit-line-clamp: 3;
    -webkit-box-orient: vertical;
    overflow: hidden;
    text-overflow: ellipsis;
}
</style>