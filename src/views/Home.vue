<script>
import Navbar from "../components/nav_bar.vue";
import Footer from "../components/footer.vue";
import Service from "../components/service.vue";
import Ville from "../components/ville.vue";
import Headeimg from "../components/header_img.vue";

export default {
  name: "Home",
  components: {
    Navbar,
    Footer,
    Service,
    Ville,
    Headeimg,
  },
};
</script>

<template>
  <header>
    <Navbar />
    <Headeimg />
  </header>
  <div class="home">
    <div class="title_button">
      <h2>Explorer d'autre maison</h2>
      <button>Voir plus <i class="bi bi-arrow-right"></i></button>
    </div>

    <div class="home_bx">
      <Ville name="Yaounde" />
      <Ville name="Douala" />
      <Ville name="Kribi" />
      <Ville name="Garoua" />
      <Ville name="Dschang" />
    </div>
  </div>
  <section>
    <h2>Nos services</h2>
    <Service image="src/assets/images/kitchen-1687121_1920.jpg" />
    <Service image="src/assets/images/317e7c5f5d69514a14d0168bdf266a7f.jpg" />
  </section>
  <Footer />
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
