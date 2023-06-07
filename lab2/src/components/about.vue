<template>
  <div class="container-fluid">
    <div class="row"></div>
    <div class="row">
      <div class="col"></div>
      <div class="col-md-8 rounded justify-content-center parent">
        <div class="card card-body">
          <h1 style="text-align: center">Про нас</h1>
          <div class="mb-md-2 d-grid gap-3">
            <div class="mb-md-2 d-grid gap-3 text-center">
              <p>Це сайт магазину для продажу дитячих речей</p>
              <div>
                <a
                  href="https://www.instagram.com/"
                  target="blank"
                  class="inst"
                >
                  <img src="../images/inst.svg"
                /></a>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="col"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: "about",
};
</script>

<style scoped>
.card-body {
  background-color: #9fe88b;
  border: 1px solid #9fe88c;
  border-radius: 10px;
}
.parent {
  height: 50vh;
  display: flex;
  align-items: center;
}
</style>
