<script lang="ts">
import { RouterLink, RouterView } from "vue-router";
import Navbar from "./components/Navbar.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",

  components: {
    Navbar,
    Footer,
  },

  data() {
    return {
      darkMode: false as boolean,
    }
  },

  computed: {
    /* Check if the value of theme will be dark or light based in boolean value of darkMode */
    theme(): string {
      return this.darkMode ? "dark" : "light";
    }
  },

  created(): void {
    this.setInitialDarkMode();
  },

  methods: {
    scrollToTop(): void {
      window.scrollTo({
        top: 0,
        behavior: "smooth",
      });
    },

    /* Set the initial darkMode value */
    setInitialDarkMode(): void {
      localStorage.getItem('darkMode') === 'true' ? this.darkMode = true : false;
    },

    /* Change the boolean value of darkMode and then set to client's localStorage */
    setDarkMode(): void {
      if (localStorage.getItem('darkMode') === 'true') {
        localStorage.setItem('darkMode', 'false');
        this.darkMode = false;
      } else {
        localStorage.setItem('darkMode', 'true');
        this.darkMode = true;
      }
    }
  },

}
</script>

<template>
  <body :data-bs-theme="theme">
    <!-- Navbar -->
    <Navbar @setDarkMode="setDarkMode" />

    <!-- Dot that go back to top on click -->
    <div class="dot" @click="scrollToTop">
      <i class="ri-arrow-up-line"></i>
    </div>

    <RouterView />
    <Footer></Footer>
  </body>
</template>

<!-- style without 'scoped' to apply to all HTML -->
<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,300;0,400;0,500;1,200;1,300;1,400;1,500&display=swap');

* {
  margin: 0;
  padding: 0;
  border: 0;
  box-sizing: border-box;
  font-family: 'Poppins', sans-serif;
}

.dot {
  color: black;
  height: 50px;
  width: 50px;
  position: fixed;
  bottom: 0;
  right: 0;
  margin: 20px;
  background-color: #f7f7f7b0;
  border-radius: 50%;
  z-index: 1;
  display: flex;
  justify-content: center;
  align-items: center;
}

.dot:hover {
  background-color: #f7f7f7;
  cursor: pointer;
}
</style>
