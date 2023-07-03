<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
import Header from './components/Header.vue';
</script>
<template>
  <header class="container pt-0">
    <div class="wrapper">
      <h1 class="text-primary"></h1>PERPUSTAKAAN ONLINE
  <nav class="navbar navbar-expand-lg navbar-light bg-light">
  <div class="container d-flex justify-content-center">
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNavAltMarkup" aria-controls="navbarNavAltMarkup" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
      <div class="navbar-nav">
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/buku">Buku</RouterLink>
        <RouterLink to="/kategori">Kategori</RouterLink>
        <RouterLink to="/anggota">Anggota</RouterLink>
        <RouterLink to="/peminjaman">Peminjaman</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </div>
    </div>
  </div>
</nav>
</div>
</header>
   <!-- <header class="container pt-0">
    <div class="wrapper">
      <Header title="PERPUSTAKAAN ONLINE" />
  <nav class="navbar navbar-expand-lg navbar-light bg-light">
    <div class="container">
      <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav"
        aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav">
          <li class="nav-item">
            <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/buku">Buku</RouterLink>
        <RouterLink to="/kategori">Kategori</RouterLink>
        <RouterLink to="/anggota">Anggota</RouterLink>
        <RouterLink to="/peminjaman">Peminjaman</RouterLink>
        <RouterLink to="/about">About</RouterLink>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</div>
</header> -->
<RouterView />
</template>


<!-- <template>
  <header class="container pt-0">
    <div class="wrapper">
      <Header title="PERPUSTAKAAN ONLINE" />
      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/buku">Buku</RouterLink>
        <RouterLink to="/kategori">Kategori</RouterLink>
        <RouterLink to="/anggota">Anggota</RouterLink>
        <RouterLink to="/peminjaman">Peminjaman</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>
    </div>
  </header>

  <RouterView />
</template> -->

<style scoped>
header {
  color: #171714;
  text-align: center;
  line-height: 1.5;
  max-height: 100vh;
  font-size: 48px;
  margin-right: 50px;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: #ffcc00;
}

nav a {
  display: inline-block;
  background-color: #1a1811;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }

  nav {
    text-align: center;
    margin-left: -1rem;
    font-size: 1rem;

    padding: 1rem 0;
    margin-top: 1rem;
  }
  h1 {
    text-align: center;
    font-size: 200px;
  }
  
}
</style>
