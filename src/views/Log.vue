<script>
import Navbar from "../components/nav_bar.vue";
import login from "../components/login.vue";

export default {
  name: "Home",
  components: {
    Navbar,
    login
  },
};
</script>

<template>
  <header>
    <Navbar />
  </header>
  <login />
 
  <RouterLink />
</template>
<style scoped>
@media screen and (max-width: 414px) {
  .title_button h2 {
    width: 30vw;
  }
}
@media screen and (max-width: 541px) {
  nav {
    justify-content: space-between;
  }
}
</style>
