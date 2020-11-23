<template>
  <div class="card my-3" style="">
    <img :src="'assets/img/' + buku.img " class="card-img-top" alt="..." />
    <div class="card-body">
      <h5 class="card-title">{{ buku.nama }}</h5>
      <p class="card-text">
        {{ buku.harga }}
      </p>
      <p class="card-text">
        {{ buku.stok }}
      </p>
      <a href="#" class="btn btn-primary mr-2">Take It</a>
      <a href="#" class="btn btn-danger">Remove</a>
    </div>
  </div>
</template>

<script>
export default {
  name: "CardBuku",
  props: ["buku"],
};
</script>

<style></style>
