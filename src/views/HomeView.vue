<template>
  <div class="home">
    <navbar />
    <div class="mt-5 container">
      <hero/>

      <div class="best row">
        <div class="col">
          <h3>Best Food</h3>
        </div>
        <div class="col">
          <router-link to="/foods" class="btn btn-success float-right">Lihat semua</router-link>
        </div>
      </div>
    </div>
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