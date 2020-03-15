<template>
  <transition name="fade">
    <div v-if="show" class="preloader">
      <KuflinkSvg class="preloader__logo" />
    </div>
  </transition>
</template>

<script>
import KuflinkSvg from "../assets/kuflink.svg";
export default {
  name: "Preloader",
  data() {
    return {
      show: true
    };
  },
  components: {
    KuflinkSvg
  },
  mounted() {
    this.showToggle();
    console.log("Preloader mounted");
    console.log(new Date().getDate());
  },
  methods: {
    showToggle() {
      setTimeout(() => {
        this.show = false;
      }, 1000);
    }
  }
};
</script>

<style lang="scss" scoped>
.preloader {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  position: absolute;
  width: 100%;
  height: 100vh;
  background-image: linear-gradient(to bottom, $blue, $green);
  z-index: 9999;

  &__logo {
    color: $white;
    animation-name: scaleOut;
    animation-duration: 1.2s;
    animation-fill-mode: forwards;
    fill: $white;
  }
}

.fade-enter-active,
.fade-leave-active {
  transition: opacity 1s;
}

.fade-enter,
.fade-leave-to {
  opacity: 0;
}

@keyframes scaleOut {
  0% {
    transform: scale(1);
  }
  100% {
    transform: scale(0);
  }
}
</style>