<template>
  <!--  <navbar/>-->
  <div class="col-auto px-2 px-lg-2 m-2">
    <h3 class="text-center"></h3>
    <div class="card">
      <div class="card-body">
        <div class="row">
          <div class="col col-md-3 px-1">
            <img class="img-thumbnail" src="../images/kid1.jpeg" />
          </div>
          <div class="col-auto col-md-6 px-2">
            <p class="text">Кофта для хлопців</p>
            <p class="text">Ціна: 1000грн</p>
          </div>
          <div class="col col-md-3 px-1">
            <button
              @click="increase"
              class="btn-outline-success btn update-cart"
              data-product=""
              data-action="add"
              href=""
              style="margin-top: 80px"
            >
              Додати до кошика
            </button>
          </div>
        </div>
      </div>
      <hr />
      <div class="card-body">
        <div class="row">
          <div class="col col-md-3 px-1">
            <img class="img-thumbnail" src="../images/girl.jpeg" />
          </div>
          <div class="col-auto col-md-6 px-2">
            <p class="text">Кофта для дівчат</p>
            <p class="text">Ціна 1000грн</p>
          </div>
          <div class="col col-md-3 px-1">
            <button
              @click="increase"
              class="btn-outline-success btn update-cart"
              data-product=""
              data-action="add"
              href=""
              style="margin-top: 80px"
            >
              Додати до кошика
            </button>
          </div>
        </div>
      </div>
      <hr />
      <div class="card-body">
        <div class="row">
          <div class="col col-md-3 px-1">
            <img class="img-thumbnail" src="../images/item3.jpeg" />
          </div>
          <div class="col-auto col-md-6 px-2">
            <p class="text">Дитячі кросівки</p>
            <p class="text">Ціна: 1000грн</p>
          </div>
          <div class="col col-md-3 px-1">
            <button
              @click="increase"
              class="btn-outline-success btn update-cart"
              data-product=""
              data-action="add"
              href=""
              style="margin-top: 80px"
            >
              Додати до кошика
            </button>
          </div>
        </div>
      </div>
      <hr />
    </div>
  </div>
  <router-view></router-view>
</template>

<script>
import navbar from "./navbar.vue";
import store from "@/store/store";
export default {
  name: "TheStore",
  methods: {
    increase() {
      store.state.count++;
      console.log(store.state.count);
    },
  },
};
</script>

<style scoped></style>
