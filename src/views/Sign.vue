<script>
import Navbar from "../components/nav_bar.vue";
import SignUp from "../components/SignUp.vue";

export default {
  name: "Home",
  components: {
    Navbar,
    SignUp,
  },
};
</script>

<template>
  <header>
    <Navbar />
 
  </header>
  <SignUp />
 
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
