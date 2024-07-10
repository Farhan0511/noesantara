<template>
  <div class="container card shadow card-costum" style="width: 18rem">
    <img
      :src="'/assets/images/' + product.gambar"
      class="card-img-top"
      alt="..."
    />
    <div class="card-body">
      <h5 class="card-title">{{ product.nama }}</h5>
      <p class="card-text">harga : Rp. {{ product.harga }}</p>
      <a href="#" class="btn btn-success text-white btn-centered">
        <b-icon-cart></b-icon-cart>
        Pesan sekarang
      </a>
    </div>
  </div>
</template> 

<script>
export default {
  name: "CardProduct",
  props: ["product"],
};
</script>

<style>
</style>