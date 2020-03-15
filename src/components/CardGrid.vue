<template>
  <div class="container grid-33 gap4">
    <card-item v-for="(card, index) in cardArr" :key="index" v-bind:cardData="card" />
  </div>
</template>

<script>
import CardItem from "./CardItem";
import { gsap } from "gsap";
export default {
  name: "CardGrid",
  components: {
    CardItem
  },
  data() {
    return {
      cardArr: [
        {
          title: "Trusted investments for you",
          subtitle: "Join us today",
          description:
            "Fund exciting projects secured against UK property* and earn up to 7.2% interest per annum*, plus up to 4% cashback** on your first investment."
        },
        {
          title: "Lorem ipsum dolor sit",
          subtitle: "Lorem ipsum",
          description:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloribus laudantium placeat accusamus voluptate doloremque consequuntur, dolores beatae impedit debitis nam."
        },
        {
          title: "Lorem ipsum",
          subtitle: false,
          description:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloribus laudantium placeat accusamus voluptate doloremque consequuntur, dolores beatae impedit debitis nam."
        }
      ]
    };
  },
  mounted() {
    gsap
      .timeline()
      .from(".card", { x: 900, duration: 0.6, opacity: 0, stagger: 0.2 }, 1);
  }
};
</script>

<style lang="scss">
</style>