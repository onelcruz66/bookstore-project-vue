<script setup lang="ts">
import HomeCategoryList from "@/components/HomeCategoryList.vue";
</script>

<style scoped>
div {
  position: relative;
  left: 380px;
}
.home-page {
  display: flex;
  position: relative;
  center: 100%;
  left: 800px;
  margin-top: 50px;
}

.welcome-text {
  width: 20em;
}
.welcome-message {
  margin-top: 50px;
  margin-bottom: 50px;
  color: white;
  position: relative;
  left: 600px;
}
.welcome-message h1 {
  font-family: "Proza Libre", serif;
}
.main-page-button {
  position: relative;
  height: 80px;
  width: 250px;
  border-radius: 8px;
  left: 375px;
  background: #282d30;
  color: white;
  font-size: large;
  font-family: "Proza Libre", serif;
}
</style>
<template>
  <div class="home-page">
    <img
      src="@/assets/images/site/wizard_logo.png"
      alt="Wizard Logo"
      class="front-wizard-logo"
    />
  </div>
  <div class="welcome-message">
    <h1>
      Welcome to Ye Old Bochard Bookstore.<br />Your source for medieval stories
      and <br />fantasies...
    </h1>
  </div>
  <div>
    <input
      type="button"
      class="main-page-button"
      value="Categories"
    /><br /><br />
    <input
      type="button"
      class="main-page-button"
      value="Best Sellers"
    /><br /><br /><br />
  </div>
</template>
