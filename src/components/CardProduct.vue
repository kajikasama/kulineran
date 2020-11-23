<template>
  <div class="card shadow card-product" style="">
    <img :src="'assets/img/' + product.gambar" class="card-img-top" />
    <div class="card-body">
      <h5 class="card-title">{{ product.nama }}</h5>
      <p class="card-text">Harga : Rp. {{ product.harga }}</p>
      <a href="#" class="btn btn-primary"><b-icon-cart /> Pesan</a>
    </div>
  </div>
</template>

<script>
export default {
  name: "CardProduct",
  props: ["product"],
};
</script>

<style></style>
