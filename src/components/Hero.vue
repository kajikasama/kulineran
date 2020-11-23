<template>
  <div class="hero">
    <!-- Desktop -->
    <div class="d-none d-md-block">
      <div class="row mt-4">
        <div class="col-md-6">
          <div class="d-flex h-100">
            <div class="justify-content-center align-self-center">
              <h2>
                <strong>Delicious, Food Menu, </strong> <br />
                in Your Gadget
              </h2>
              <p>Ayo segera pesan dan pilih <strong>makanan</strong> favorit anda</p>
              <button class="btn btn-lg btn-primary">
                <b-icon-arrow-right />
                Pesan
              </button>
            </div>
          </div>
        </div>
        <div class="col-md-6 mt-4">
          <img src="../assets/img/hero.png" width="100%" alt="" />
        </div>
      </div>
    </div>

    <!-- Mobile -->
    <div class="row mt-4 d-sm-block d-md-none">
      <div class="col-md-6 mt-4">
        <img src="../assets/img/hero.png" width="100%" alt="" />
      </div>
      <div class="col-md-6 mt-4">
        <div class="d-flex h-100">
          <div class="justify-content-center align-self-center">
            <h2>
              <strong>Delicious, Food Menu, </strong> <br />
              in Your Gadget
            </h2>
            <p>Ayo segera pesan dan pilih makanan favorit anda</p>
            <button class="btn btn-lg btn-primary mt-3">
              <b-icon-arrow-right />
              Pesan
            </button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Hero",
};
</script>

<style></style>
