<template>
  <div>
    <Navbar />
    <div class="container">
      <div class="row">
        <div class="col mt-4">
          <h2>Buku Cuy <strong>Banyak</strong> ni</h2>
        </div>
      </div>
      <div class="row">
        <div class="col-md-4" v-for="buku in bukus" :key="buku.id">
          <CardBuku :buku="buku" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Navbar from "@/components/Navbar.vue";
import CardBuku from "@/components/CardBuku.vue";
import axios from "axios";

export default {
  name: "Buku",
  components: {
    Navbar,
    CardBuku,
  },
  data() {
    return {
      bukus: [],
    };
  },
  methods: {
    setBuku(data) {
      this.bukus = data;
    },
  },
  mounted() {
    axios
      .get("http://localhost:3030/buku")
      .then((response) => this.setBuku(response.data))
      .catch((error) => console.log(error));
  },
};
</script>

<style></style>
