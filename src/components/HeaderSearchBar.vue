<script setup lang="ts"></script>

<style scoped>
input[type="text"] {
  margin: 0.5em 0;
  width: 12em;
}
.search-bar {
  border-radius: 8px;
  position: relative;
  top: 20px;
  left: 470px;
  width: 250%;
  text-align: center;
  padding: 0.5em;
}
.search-button {
  position: relative;
  height: 38px;
  bottom: 20px;
  left: 940px;
  background: #282d30;
  border-radius: 8px;
}
</style>

<template>
  <form>
    <input type="text" class="search-bar" /><br />
    <input
      type="image"
      src="/src/assets/images/site/icons8-search-50%20(1).png"
      class="button search-button"
      alt="search-icon"
    />
  </form>
</template>
