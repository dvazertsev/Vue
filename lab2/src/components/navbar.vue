<template>
  <nav class="navbar bg-gradient navbar-dark navbar-expand-lg bg-body-tertiary">
    <div class="container-fluid container px-2 px-lg-4">
      <a class="navbar-brand" style="" href=""
        ><img style="width: 25px; height: 25px" src="../images/home.svg"
      /></a>
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarNavAltMarkup"
        aria-controls="navbarNavAltMarkup"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
        <div class="navbar-nav ms-auto mb-3 mb-lg-1 navigation">
          <router-link
            to="/"
            class="nav-link"
            style="color: #39ad31; margin-left: 10px"
            >Головна</router-link
          >
          <router-link
            to="cart"
            class="nav-link"
            style="color: #39ad31; margin-left: 20px"
            >Кошик</router-link
          >
          <router-link
            to="about"
            class="nav-link"
            style="color: #39ad31; margin-left: 20px"
            >Інформація</router-link
          >
          <li class="nav-item dropdown">
            <a
              class="nav-link dropdown-toggle"
              href="#"
              role="button"
              data-bs-toggle="dropdown"
              aria-expanded="false"
              style="
                color: #39ad31;
                margin-left: 20px;
                border: 1px solid #39ad31;
                border-radius: 10px;
              "
            >
              Профіль
            </a>
            <ul class="dropdown-menu">
              <router-link
                to="profile"
                class="dropdown-item"
                style="color: #39ad31"
                >Профіль</router-link
              >
              <router-link
                to="login"
                class="dropdown-item"
                style="color: #39ad31"
                >logout</router-link
              >
              <router-link
                to="login"
                class="dropdown-item"
                style="color: #39ad31"
                >login</router-link
              >
            </ul>
          </li>
        </div>
      </div>
    </div>
  </nav>
</template>

<script>
import logoSrc from "@/assets/logo.svg";
export default {
  name: "navbar",
};
</script>

<style scoped>
.navigation {
}
</style>
