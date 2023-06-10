<script setup>
import Welcome from '../components/Welcome.vue'
import NavBar from '../components/Navbar.vue'
</script>

<template class="container">
  <main>
    <NavBar />
    <Welcome />
  </main>
</template>

<style lang="scss">
.container {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
}
</style>