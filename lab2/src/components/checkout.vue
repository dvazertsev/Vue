<template>
  <br>
  <div class="container-md p-1 card ">

    <div class="row">
      <div class=" col col-md-5">
      </div>
      <div class="col-auto ">
        <h2>Замовлення</h2>
      </div>
    </div>
  </div>
  <br>
  <div class="col p-1">
    <div class="row">
      <div class="col-auto col-md-6  px-2  card">
        <div id="shipping-info">
          <form>
            <div class="text-center">
              <p><h4>Адреса доставки</h4></p>
            </div>

            <div class="input-group mb-3">
              <span class="input-group-text" id="username">Місто</span>
              <input v-model="city"   type="text" id="Місто" class="form-control" placeholder="City"
                     aria-label="First Name"
                     aria-describedby="basic-addon1"
                     City-data>
            </div>
            <div class="input-group mb-3">
              <span class="input-group-text">Адреса</span>
              <input v-model="addres" type="text" id="address" class="form-control" placeholder="Адреса"
                     aria-label="First Name"
                     aria-describedby="basic-addon1"
                     address-data
              >
            </div>
            <div class="input-group mb-3">
              <span class="input-group-text">Телефон</span>
              <input v-model="phone" id="Phone" type="text" maxlength=12 class="form-control" placeholder="38(099)-999-99-99"
                     aria-label="First Name"
                     aria-describedby="basic-addon1"
              phone-data >
            </div>


            <div class="d-grid gap-2 py-2">
              <button @click="validForm" type="submit" class="btn btn-primary  bt btn-block"> Продовжити</button>
            </div>
          </form>
        </div>
      </div>

      <div class="col-auto col-md-6 px-2 card">

        <div class="row  p-2">
          <div class="col-md-5 p-3">
            <a class="btn btn-outline-primary" @click="backToCart"> Повернутись до кошику</a>
          </div>
          <div class="col-md-4">
            <p><h2><strong>Cart</strong></h2></p>
          </div>
        </div>
        <table class="table">
          <thead>
          <tr>
            <th scope="col">Картинка</th>
            <th scope="col">Речі</th>
            <th scope="col">Ціна</th>
            <th scope="col">Збільшити</th>
            <th scope="col">Всього</th>
          </tr>
          </thead>
          <tbody>
          <!--        ../images/Xiaomi-Mi-Notebook-Pro-15-2020-Intel-0_large.jpg    When I use picture I received error in test   -->
          <tr>
            <th scope="row"><img src=""
                                 style="width: 50px ; height: 50px">
            </th>
            <td><p class="px-lg-2"> кофта для дівчат</p></td>
            <td><p class="px-lg-2"> 1000</p></td>
            <td><p class="px-lg-2"> {{ cart.quantity }}</p></td>
            <td><p class="px-lg-2">{{ cart.total }} </p></td>
          </tr>
          <!--                    {% endfor %}-->
          </tbody>

        </table>
        <div class="row-auto">
          <table class="table">
            <tr>
              <th><h5>Items: <strong>{{ cart.items }}</strong></h5></th>
              <th><h5>Total: <strong>{{ cart.total }}</strong></h5></th>
              <!--                            {#-->

            </tr>
          </table>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import store from "./../store/store.js";

export default {
  name: "checkout",
  data() {
    return {
      cart: {
        items: store.state.orderlist.items,
        total: store.state.orderlist.total,
        count: store.state.orderlist.count,
        quantity: store.state.orderlist.quantity,
      },
      city: '',
      addres: '',
      phone: ''
    }


  },
  methods: {
    backToCart() {
      this.$router.push('/cart')
    },
    validForm() {
      if (this.city.length > 0 && this.addres.length > 0 && this.phone.length > 0 && this.phone.length >= 12) {
        if (this.phone.match(/^[0-9]+$/) != null) {
          window.alert("Saved successfully")
          this.$router.push('/')
          return true
        } else {
          window.alert("Phone number must contain only numbers")

        }
      }
      window.alert("Please fill all fields")
    }
  },
}
</script>

<style scoped>

</style>