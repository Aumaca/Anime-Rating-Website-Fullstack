<script setup lang="ts">
const darkMode: string | null = localStorage.getItem('darkMode');
const emit = defineEmits<{
  (event: 'setDarkMode'): void,
}>()
const setDarkMode = (): void => emit('setDarkMode');
</script>

<template>
  <nav class="navbar navbar-expand-lg bg-body-tertiary p-3">
    <div class="container-fluid">

      <!-- Logo -->
      <a class="navbar-brand" href="/">
        <div>
          Anime Rating
          <i class="ri-star-half-line ms-2"></i>
        </div>
      </a>

      <!-- Toggle -->
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent">
        <span class="navbar-toggler-icon"></span>
      </button>

      <!-- Links -->
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav me-auto mb-2 mb-lg-0">

          <li class="nav-item">
            <RouterLink to="/" class="nav-link active">Home</RouterLink>
          </li>

          <li class="nav-item">
            <RouterLink to="/reviews" class="nav-link active">Reviews</RouterLink>
          </li>

          <li class="nav-item">
            <RouterLink to="/about" class="nav-link active">About</RouterLink>
          </li>

          <!-- Dark Mode -->
          <li class="nav-link active d-flex gap-2">
            Dark Mode
            <div class="form-check form-switch">
              <input :checked="darkMode === 'true'" class="form-check-input" type="checkbox" role="switch"
                id="flexSwitchCheckDefault" @click="setDarkMode" />
            </div>
          </li>
        </ul>

        <!-- Search Input -->
        <form class="d-flex" role="search">
          <input class="form-control me-2" type="search" placeholder="Search Anime">
          <button class="btn btn-outline-success" type="submit">Search</button>
        </form>
      </div>

    </div>
  </nav>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Unbounded&display=swap');

nav {
  width: 100%;
  position: sticky;
  top: 0;
  border-bottom: 3px solid #198754;
  padding: 20px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  z-index: 999;
}

.navbar-brand div {
  font-family: 'Unbounded', cursive;
  display: flex;
  font-size: 23px;
}

.navbar-toggler-icon {
  font-size: 14px;
}
</style>
