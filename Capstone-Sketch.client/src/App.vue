<template>
  <header>
    <Navbar />
  </header>
  <main class="bg-img">
    <router-view />
  </main>
   <footer class="bg-dark text-light">
    Made with 💖 by CodeWorks
  </footer>
</template>

<script>
import { computed } from 'vue'
import { AppState } from './AppState'
import Navbar from './components/Navbar.vue'

export default {
  setup() {
    return {
      appState: computed(() => AppState)
    }
  },
  components: { Navbar }
}
</script>
<style lang="scss">
@import "./assets/scss/main.scss";

:root{
  --main-height: calc(100vh - 32px - 64px);
}

.bg-img {
  // Uncomment after change text color
  // background-image: url(https://images.unsplash.com/photo-1554755229-ca4470e07232?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1887&q=80);
  background-image: url(https://images.unsplash.com/photo-1520299607509-dcd935f9a839?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1931&q=80);
  object-position: right;
  object-fit: cover;
  background-attachment: fixed;
  min-height: 100vh;
}
footer {
  display: grid;
  place-content: center;
  height: 32px;
}
</style>
