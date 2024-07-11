<template>
  <div class="container">
    <navbar />
    
    <div class="container mt-4 ">
      <div class="row">
        <div class="col mb-4">
          <h2>Daftar <strong>Makanan</strong></h2>
        </div>
      </div>
    </div>

     <div class="row mb-4">
        <div class="col md-4 mt-4" v-for="product in products" :key="product.id">
          <card-product :product="product"/>
        </div>
      </div>

    <div>
      <Footer></Footer>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import Navbar from "@/components/Navbar.vue";
import Footer from "@/components/Footer.vue";
import CardProduct from "@/components/CardProduct.vue";
import axios from "axios";

export default {
  name: "FoodsApp",
  components: {
    Navbar,
    Footer,
    CardProduct
  },
  data() {
    return {
      products: [],
    };
  },
  methods: {
    setProducts(data) {
      this.products = data;
    },
  },
  mounted() {
    axios
      .get("http://localhost:3000/products")
      .then((response) => this.setProducts(response.data))
      .catch((error) => console.log(error))
  },
};
</script>
