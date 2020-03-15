<template>
  <header class="header">
    <div class="header__wrapper">
      <KuflinkSvg class="header__logo" />

      <nav class="nav">
        <ul class="nav__list">
          <li class="nav__item">
            <a href="/" class="nav__link">Peer to Peer Lending</a>
          </li>
          <li class="nav__item">
            <a href="/" class="nav__link">IF-ISA</a>
          </li>
          <li class="nav__item">
            <a href="/" class="nav__link">SIPP</a>
          </li>
          <li class="nav__item">
            <a href="/" class="nav__link">Borrow</a>
          </li>
          <li class="nav__item">
            <a href="/" class="nav__link nav__link--last">Contact</a>
          </li>
        </ul>
        <div class="nav__actions"></div>
      </nav>
      <div class="nav-btn">
        <svg
          id="menu-btn"
          width="91"
          height="54"
          viewBox="0 0 91 54"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            class="top"
            d="M67.2519 1.23366L2 1.52438L53.9866 40.9616C62.9045 47.7268 75.4715 46.7605 83.2504 38.7115C96.847 24.6426 86.817 1.14649 67.2519 1.23366Z"
            stroke="white"
          />
          <path class="middle" d="M10.5 25H66.5" stroke="white" />
          <path
            class="bottom"
            d="M63.3934 53.5H2L57.0783 9.97662C66.1052 2.84344 79.2252 4.48675 86.214 13.6259C90.4468 19.1612 91.5944 26.4611 89.2642 33.0282L88.2222 35.9647C84.4923 46.4763 74.5472 53.5 63.3934 53.5Z"
            stroke="white"
          />
        </svg>
      </div>
    </div>
  </header>
</template>

<script>
import KuflinkSvg from "../assets/kuflink.svg";
export default {
  name: "Header",
  components: {
    KuflinkSvg
  },
  mounted() {
    const menuBtn = document.querySelector("#menu-btn");
    // const html = document.querySelector("html");
    // const nav = document.querySelector(".nav");

    menuBtn.addEventListener("click", () => {
      let svgIcon = document.querySelectorAll("#menu-btn path");

      svgIcon.forEach(path => {
        path.classList.toggle("cross");
      });

      document.querySelector(".nav").classList.toggle("reveal");
      // if (nav.classList.contains("reveal")) {
      //   html.style.overflowY = "hidden";
      // } else {
      //   html.style.overflowY = "visible";
      // }
    });

    console.log("Header mounted");
    console.log(new Date().getDate());
  }
};
</script>


<style lang="scss">
@import "../styles/components/_nav.scss";
</style>