<template>
  <div>
    <navbar/>
  </div>
  
</template>

<script>
// @ is an alias to /src
import Navbar from '@/components/Navbar.vue'

export default {
  name: "AboutApp",
  components: {
    Navbar,
  }
};
</script>