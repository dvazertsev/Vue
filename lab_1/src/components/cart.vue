<template>
  <br />
  <div class="container-md p-1 card">
    <div class="row">
      <div class="col col-md-4">
        <router-link to="/" class="btn bg-info"> Повернутись</router-link>
      </div>
      <div class="col-auto">
        <h2>Кошик</h2>
      </div>
    </div>

    <hr />
    <table class="table">
      <tr>
        <th>
          <h5>Речі: <strong>1</strong></h5>
        </th>
        <th>
          <h5>Всього: <strong>1000</strong></h5>
        </th>
        <th>
          <a
            style="float: right; margin: 5px"
            class="btn bg-success"
            href="checkout"
            >Перевірити</a
          >
          <!--                <th><a style="float: right;margin: 5px" class="btn btn-success" href="">Checkout</a>-->
        </th>
      </tr>
    </table>
  </div>
  <br />
  <br />
  <div class="col-auto p-1 card">
    <table class="table">
      <thead>
        <tr>
          <th scope="col">Картинка</th>
          <th scope="col">Кількість</th>
          <th scope="col">Ціна</th>
          <th scope="col">Додати</th>

          <th scope="col">Всього</th>
        </tr>
      </thead>
      <tbody>
        <!--      {% for  elem in items %}-->
        <tr>
          <th scope="row">
            <img
              src="../images/item3.jpeg"
              style="width: 100px; height: 100px"
            />
          </th>
          <td>
            <p class="px-lg-2"></p>
            1
          </td>
          <td>
            <p class="px-lg-2"></p>
            1000
          </td>
          <td>
            <p class="px-sm-2">
              <button class="btn update-cart" data-product="" data-action="add">
                +
              </button>
              <button
                class="btn update-cart"
                data-product=""
                data-action="remove"
              >
                -
              </button>
            </p>
          </td>
          <td>
            <p class="px-lg-2"></p>
            1000
          </td>
        </tr>
        <!--      {% endfor %}-->
      </tbody>
    </table>
  </div>
</template>

<script>
export default {
  name: "cart",
};
</script>

<style scoped></style>
