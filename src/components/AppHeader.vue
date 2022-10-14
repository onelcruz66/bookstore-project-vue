<script setup lang="ts">
import HeaderDropdown from "@/components/HeaderDropdown.vue";
</script>

<style scoped>
header {
  background: #997150;
  display: flex;
  padding: 1em;
  gap: 1em;
}

.text-logo {
  font-family: var(--title-font-family);
  position: relative;
  right: 10px;
}
.bookstore-logo img {
  position: relative;
  center: 100%;
  left: 50px;
  bottom: 45px;
  margin-top: 50px;
  width: 150px;
  height: auto;
}
@media (max-width: 600px) {
  header {
    flex-direction: column;
  }
}
.cart-button {
  position: relative;
  left: 15px;
}
.login-button {
  position: relative;
  left: 20px;
  text-align: center;
  font-size: 10px;
  height: 25px;
  width: 25px;
}
.button-background {
  position: relative;
  height: 40px;
  width: 85px;
  left: 1100px;
  background: #282d30;
  border-radius: 8px;
  top: 20px;
}
.button-background2 {
  position: relative;
  bottom: 6px;
  height: 40px;
  width: 85px;
  left: 1110px;
  background: #282d30;
  border-radius: 8px;
  top: 15px;
}
.search-bar {
  border-radius: 8px;
  position: relative;
  top: 20px;
  left: 350px;
  width: 250%;
  text-align: center;
  padding: 0.5em;
}
.search-button {
  position: relative;
  height: 41px;
  bottom: 20px;
  left: 820px;
  background: #282d30;
  border-radius: 8px;
}
</style>

<template>
  <header class="container">
    <section class="bookstore-logo">
      <router-link to="/">
        <img src="/src/assets/images/site/wizard_logo.png" alt="Wizard Logo" />
      </router-link>
    </section>
    <section class="title-and-search-bar">
      <h1>
        <router-link to="/" class="text-logo">Ye Old Bochard</router-link>
      </h1>
    </section>
    <form>
      <input type="text" class="search-bar" /><br />
      <input
        type="image"
        src="/src/assets/images/site/icons8-search-50%20(1).png"
        class="button search-button"
        alt="search-icon"
      />
    </form>
    <section class="header-dropdown-and-cart">
      <button type="button" class="button-background">
        <img
          src="@/assets/images/site/icons8-shopping-cart-30.png"
          alt="Cart"
          height="80"
          width="60"
          class="cart-button"
        />
      </button>
      <button type="button" class="button-background2">
        <img
          src="@/assets/images/site/icons8-login-64.png"
          alt="Log In"
          height="40"
          width="50"
          class="login-button"
        />
      </button>
      <header-dropdown></header-dropdown>
    </section>
  </header>
</template>
