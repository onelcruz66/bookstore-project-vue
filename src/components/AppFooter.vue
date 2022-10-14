<script setup lang="ts"></script>
<style>
footer {
  background: var(--secondary-background-color);
  display: flex;
  gap: 1em;
}
.about {
  position: relative;
  left: 1200px;
  top: 20px;
  font-family: "Proza Libre", serif;
  font-size: 30px;
}
.contact {
  position: relative;
  left: 800px;
  bottom: 20px;
  font-family: "Proza Libre", serif;
  font-size: 30px;
}
.directions {
  position: relative;
  left: 400px;
  bottom: 60px;
  font-family: "Proza Libre", serif;
  font-size: 30px;
}
.copyright {
  position: relative;
  left: 50px;
  bottom: 110px;
  font-family: "Proza Libre", serif;
}

.links,
.social-media-icons {
  display: flex;
  flex-direction: column;
}

.social-media-icons {
  text-align: center;
  gap: 0.25em;
}
.fb-button {
  position: relative;
  left: 1500px;
  top: 35px;
  height: 40px;
  width: 80px;
}
.tw-button {
  position: relative;
  left: 1550px;
  bottom: 9px;
  height: 40px;
  width: 80px;
}
</style>
<!--<style scoped>-->
<!--footer {-->
<!--  background: var(&#45;&#45;secondary-background-color);-->
<!--  display: flex;-->
<!--  gap: 1em;-->
<!--}-->

<!--.links,-->
<!--.social-media-icons {-->
<!--  display: flex;-->
<!--  flex-direction: column;-->
<!--}-->

<!--.social-media-icons {-->
<!--  text-align: center;-->
<!--  gap: 0.25em;-->
<!--}-->
<!--</style>-->

<template>
  <footer class="container">
    <section class="links">
      <router-link to="/"><a class="about">about</a></router-link>
      <router-link to="/"><a class="contact">contact</a></router-link>
      <router-link to="/"><a class="directions">directions</a></router-link>

      <a class="copyright"
        ><img
          src="@/assets/images/site/copyright.png"
          alt="copyright-icon"
          height="20px"
          width="20px"
        />
        Ye Old Bochord 2022</a
      >
      >
    </section>
    <section class="social-media-icons">
      <router-link to="/"
        ><img
          src="@/assets/images/site/facebook-icon.png"
          alt="fb-icon"
          class="fb-button"
      /></router-link>
      <router-link to="/"
        ><img
          src="@/assets/images/site/twitter-icon.png"
          alt="tw-icon"
          class="tw-button"
      /></router-link>
    </section>
  </footer>
</template>
