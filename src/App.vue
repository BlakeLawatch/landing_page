<template>
  <header>
    <!-- <Navbar /> -->
  </header>
  <main class="main">
    <router-view />
  </main>
  <footer>

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

:root {
  --main-height: calc(100vh - 32px - 64px);
}

.main {
  background-image: url('https://img.freepik.com/premium-photo/grunge-background-with-space-text_196038-5926.jpg?size=626&ext=jpg&ga=GA1.1.66302407.1699569051&semt=ais');
}
</style>
