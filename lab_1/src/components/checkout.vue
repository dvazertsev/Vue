<template>
    <br>
    <div class="container-md p-1 card ">

        <div class="row">
            <div class=" col col-md-5">
            </div>
            <div class="col-auto ">
                <h2>Перевірка замовлення </h2>
            </div>
        </div>
    </div>
    <br>
    <div class="col p-1">
        <div class="row">
            <div class="col-auto col-md-6  px-2  card">
                <div id="shipping-info">
                    <div class="text-center"><p><h4>Адреса</h4></p></div>

                    <div class="input-group mb-3">
                        <span class="input-group-text" id="username">Місто</span>
                        <input type="text" class="form-control" placeholder="Місто" aria-label="First Name"
                               aria-describedby="basic-addon1">
                    </div>
                    <div class="input-group mb-3">
                        <span class="input-group-text" id="username">Адреса</span>
                        <input type="text" class="form-control" placeholder="Адреса" aria-label="First Name"
                               aria-describedby="basic-addon1">
                    </div>
                    <div class="input-group mb-3">
                        <span class="input-group-text" id="username">Телефон</span>
                        <input type="text" class="form-control" placeholder="+38(099)-999-99-99" aria-label="First Name"
                               aria-describedby="basic-addon1">
                    </div>


                    <div class="d-grid gap-2 py-2">
                        <button type="submit" class="btn btn-primary  bt btn-block"> Продовжити</button>
                    </div>
                    <!--                    </form>-->
                </div>
            </div>

            <div class="col-auto col-md-6 px-2 card">

                <div class="row  p-2">
                    <div class="col-md-5 p-3">
                        <a class="btn btn-outline-primary" href="/"> Повернутись на головну</a>
                    </div>
                    <div class="col-md-4">
                        <p><h2><strong>Кошик</strong></h2></p>
                    </div>
                </div>
                <table class="table">
                    <thead>
                    <tr>
                        <th scope="col">Картинка</th>
                        <th scope="col">Речі</th>
                        <th scope="col">Ціна</th>
                        <th scope="col">Кількість</th>
                        <th scope="col">Всього</th>
                    </tr>
                    </thead>
                    <tbody>
                    <!--                    {% for elem in items %}-->
                    <tr>
                        <div scope="row"><img src="../images/kid1.jpeg"
                                             style="width: 50px ; height: 50px">
                        </div>
                        <td><p class="px-lg-2"> Кофта для хлопців</p></td>
                        <td><p class="px-lg-2"> 1000</p></td>
                        <td><p class="px-lg-2"> 1</p></td>
                        <td><p class="px-lg-2">1000 </p></td>
                    </tr>
                    <!--                    {% endfor %}-->
                    </tbody>

                </table>
                <div class="row-auto">
                    <table class="table">
                        <div>
                            <th><h5>Речі: <strong>1</strong></h5></th>
                            <th><h5>Всього: <strong>1000</strong></h5></th>
<!--                            {#-->
                            <th><a style="float: right;margin: 5px" class="btn btn-success"
                                    href="">Повернутись  </a></th>
<!--                            #}-->
                        </div>
                    </table>
                </div>
            </div>
        </div>
        </div>
</template>

<script>
export default {
    name: "checkout"
}
</script>

<style scoped>

</style>