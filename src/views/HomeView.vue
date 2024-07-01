<template>
  <div class="home">
    <navbar />
    <hero/>
  </div>
</template>

<script>
// @ is an alias to /src
import Navbar from '@/components/Navbar.vue'
import Hero from '@/components/Hero.vue'

export default {
  name: 'HomeView',
  components: {
    Navbar,
    Hero
  }
}
</script>