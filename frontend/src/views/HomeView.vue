<script setup lang="ts">
import Carousel from '../components/Carousel.vue';
import kaguya3 from '../assets/imgs/kaguya3.png';
import codegeassposter from '../assets/imgs/codegeassposter.jpg';
import attackontitan from '../assets/imgs/attackontitan.jpg';
import kimetsuposter from '../assets/imgs/kimetsuposter.jpg';
</script>

<template>
  <main>
    <!-- Carousel -->
    <Carousel />

    <div class="container">
      <div class="d-flex flex-column flex-md-row justify-content-center">
        <!-- Recents Ratings -->
        <article class="m-3 mt-3 d-flex justify-content-center">
          <div class="list rounded bg-success p-1">

            <!-- List Header -->
            <div class="list-header">
              <h4 class="py-2 px-2 m-0 text-white">Recent reviews</h4>
            </div>

            <!-- List Body -->
            <div class="list-body px-2 py-1">

              <!-- Card -->
              <div class="card mb-3 border-0 shadow-lg">
                <div class="row g-0">
                  <div class="card-image-container col-md-4 col-4">
                    <img :src="kaguya3" class="img-fluid object-fit-cover h-100 rounded-start shadow">
                  </div>
                  <div class="col-md-8 col-8">
                    <div class="card-body">
                      <h5 class="card-title">Kaguya Sama: Love Is War - Season 3</h5>
                      <p class="card-text">The third season of Kaguya-sama: Love Is War, titled Kaguya-sama: Love Is War –
                        Ultra Romantic, is a 2022 Japanese anime series, based on the manga series of the The third season
                        of Kaguya-sama: Love Is War, titled Kaguya-sama: Love Is War –
                        Ultra Romantic, is a 2022 Japanese anime series, based on the manga series of the</p>
                      <p class="card-text"><small class="text-muted">Last updated 3 mins ago</small></p>
                    </div>
                  </div>
                </div>
              </div>

              <!-- Card -->
              <div class="card border-0 shadow-lg">
                <div class="row g-0">
                  <div class="card-image-container col-md-4 col-4">
                    <img :src="codegeassposter" class="img-fluid object-fit-cover h-100 rounded-start shadow">
                  </div>
                  <div class="col-md-8 col-8">
                    <div class="card-body">
                      <h5 class="card-title">Code Geass: Lelouch of the Rebellion</h5>
                      <p class="card-text">Code Geass: Lelouch of the Rebellion (コードギアス 反逆のルルーシュ Kōdo Giasu: Hangyaku no
                        Rurūshu?) é um anime da franquia Code Geass, de 2006, com 25 episódios, criado pela Sunrise.
                        Dirigida por Gorō Taniguchi e escrita por Ichirō Ōkouchi, ambos tendo anteriormente trabalhado em
                        outra série da Sunrise, chamado Planetes. Code Geass - Lelouch of the Rebellion apresenta character
                        design original da CLAMP.

                        A primeira temporada da série foi apresentada no Japão pela MBS em 6 de outubro de 2006 e foi
                        concluída em 28 de Julho de 2007, após 25 episódios. A segunda temporada e sequência da série, Code
                        Geass: Lelouch of the Rebellion R2 começou a ser apresentada nas redes MBS e TBS em 6 de abril de
                        2008.</p>
                      <p class="card-text"><small class="text-muted">Last updated 3 mins ago</small></p>
                    </div>
                  </div>
                </div>
              </div>

            </div>
          </div>
        </article>

        <!-- Popular Ratings -->
        <article class="m-3 mt-3 d-flex justify-content-center">
          <div class="list rounded bg-success p-1">

            <!-- List Header -->
            <div class="list-header">
              <h4 class="py-2 px-2 m-0 text-white">Popular reviews</h4>
            </div>

            <!-- List Body -->
            <div class="list-body px-2 py-1">

              <!-- Card -->
              <div class="card mb-3 border-0">
                <div class="row g-0">
                  <div class="card-image-container col-md-4 col-4">
                    <img :src="attackontitan" class="img-fluid object-fit-cover h-100 rounded-start">
                  </div>
                  <div class="col-md-8 col-8">
                    <div class="card-body">
                      <h5 class="card-title">Attack on Titan - Season 4</h5>
                      <p class="card-text">TShingeki no Kyojin (進撃の巨人 lit. Titã de Ataque?) também conhecido pelo título em
                        inglês Attack on Titan, é uma série de mangá escrita e ilustrada por Hajime Isayama. É ambientado em
                        um mundo onde a humanidade vive dentro de cidades cercadas por três enormes muralhas que os protegem
                        dos gigantescos humanóides devoradores de humanos chamados de Titãs; a história segue Eren Yeager,
                        que jura exterminar os Titãs após um Titã causar a destruição de sua cidade natal e a morte de sua
                        mãe. Shingeki no Kyojin teve seus capítulos publicados na revista mensal de mangás shōnen Bessatsu
                        Shōnen Magazine da editora Kodansha entre setembro de 2009 a abril de 2021, com os seus capítulos
                        compilados em 34 volumes tankōbon.</p>
                      <p class="card-text"><small class="text-muted">Last updated 3 mins ago</small></p>
                    </div>
                  </div>
                </div>
              </div>

              <!-- Card -->
              <div class="card border-0">
                <div class="row g-0">
                  <div class="card-image-container col-md-4 col-4">
                    <img :src="kimetsuposter" class="img-fluid object-fit-cover h-100 rounded-start">
                  </div>
                  <div class="col-md-8 col-8">
                    <div class="card-body">
                      <h5 class="card-title">Demon Slayer - Season 2</h5>
                      <p class="card-text">Kimetsu no Yaiba (鬼滅きめつの刃やいば , Ki metsuKimetsu no YaibaYaiba?, lit. Lâmina
                        (刃)Lâmina de Destruição (滅)Destruição de Onis (鬼)Onis), também conhecido pelo título em língua
                        inglesa Demon Slayer (Matador de Demônios, em português) é uma série japonesa de mangá shōnen
                        escrita e ilustrada por Koyoharu Gotōge. O mangá é serializado desde 15 de fevereiro de 2016 e foi
                        encerrado em 18 de maio de 2020 na revista semanal Weekly Shōnen Jump, com seus capítulos sendo
                        reunidos em 23 volumes tankōbon pela editora Shueisha. Uma adaptação de um mangá para um anime de 26
                        episódios, produzida pelo estúdio ufotable, teve sua 1ª temporada exibida entre 6 de abril e 28 de
                        setembro de 2019,[1] e 2ª temporada, entre 10 de outubro de 2021 e 13 de fevereiro de 2022.
                        Em setembro de 2019, foi divulgado que todos os volumes juntos da série já tinham excedido mais de
                        10 milhões de cópias vendidas.[3] Em dezembro de 2019, o mangá já contava com mais de 25 milhões de
                        cópias em circulação.[4][5]</p>
                      <p class="card-text"><small class="text-muted">Last updated 3 mins ago</small></p>
                    </div>
                  </div>
                </div>
              </div>

            </div>
          </div>
        </article>
      </div>
    </div>

  </main>
</template>

<style scoped>
.card {
  max-width: 540px;
  max-height: 250px;
  overflow: hidden;
}

.card .card-title {
  display: -webkit-box;
  -webkit-line-clamp: 1;
  -webkit-box-orient: vertical;
  overflow: hidden;
  text-overflow: ellipsis;
}

.card p {
  display: -webkit-box;
  -webkit-line-clamp: 6;
  -webkit-box-orient: vertical;
  overflow: hidden;
  text-overflow: ellipsis;
}
</style>
