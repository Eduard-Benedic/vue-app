<template>
  <div id="site-container">
    <Preloader />
    <Header />
    <section class="section">
      <card-grid />
    </section>
    <Footer />
  </div>
</template>

<script>
import CardGrid from "./components/CardGrid.vue";
import Preloader from "./components/Preloader.vue";
import Header from "./components/Header";
import Footer from "./components/Footer";

export default {
  name: "App",
  components: {
    CardGrid,
    Header,
    Footer,
    Preloader
  },
  data() {
    return {
      loading: false
    };
  },
  created() {
    console.log(223);
  },
  mounted() {
    this.loading = true;
  }
};
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css?family=Nunito+Sans:300,700&display=swap");
@import "./styles/basics/normalize.css";
@import "./styles/basics/_base.scss";
</style>



