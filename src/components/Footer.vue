<template>
  <footer class="footer">
    <div class="container container--padd4">
      <div class="grid-25 gap4">
        <div class="footer__section">
          <h3 class="footer__title">Products & Services</h3>
          <ul class="footer__list">
            <li class="footer__item">
              <a href="/" class="footer__link">Select Invest</a>
            </li>
            <li class="footer__item">
              <a href="/" class="footer__link">Auto Invest</a>
            </li>
            <li class="footer__item">
              <a href="/" class="footer__link">IFISA</a>
            </li>
            <li class="footer__item">
              <a href="/" class="footer__link">Secondary Market</a>
            </li>

            <li class="footer__item">
              <a href="/" class="footer__link">Borrow</a>
            </li>
            <li class="footer__item">
              <a href="/" class="footer__link">Bridgin Loans</a>
            </li>
          </ul>
        </div>
        <div class="footer__section">
          <h3 class="footer__title">About Us</h3>
          <ul class="footer__list">
            <li class="footer__item">
              <a href="/" class="footer__link">Meet Kuflink</a>
            </li>
            <li class="footer__item">
              <a href="/" class="footer__link">Kuflink Foundation</a>
            </li>
            <li class="footer__item">
              <a href="/" class="footer__link">GDPR Statement</a>
            </li>
            <li class="footer__item">
              <a href="/" class="footer__link">Privacy Policy</a>
            </li>
            <li class="footer__item">
              <a href="/" class="footer__link">Governance</a>
            </li>
            <li class="footer__item">
              <a href="/" class="footer__link">Customer Complaints</a>
            </li>
            <li class="footer__item">
              <a href="/" class="footer__link">Investor Terms & Conditions</a>
            </li>
            <li class="footer__item">
              <a href="/" class="footer__link">User Agreement</a>
            </li>
            <li class="footer__item">
              <a href="/" class="footer__link">Statistics</a>
            </li>
            <li class="footer__item">
              <a href="/" class="footer__link">Wind Down Plan</a>
            </li>
          </ul>
        </div>
        <div class="footer__section">
          <h3 class="footer__title">Work With us</h3>
          <ul class="footer__list">
            <li class="footer__item">
              <a href="/" class="footer__link">Careers</a>
            </li>
            <li class="footer__item">
              <a href="/" class="footer__link">Affiliates</a>
            </li>
            <li class="footer__item">
              <a href="/" class="footer__link">Independent Financial</a>
            </li>
            <li class="footer__item">
              <a href="/" class="footer__link">Advisers</a>
            </li>
          </ul>
        </div>
        <div class="footer__section">
          <h3 class="footer__title">Media Hub</h3>
          <ul class="footer__list">
            <li class="footer__item">
              <a href="/" class="footer__link">Newsroom</a>
            </li>
            <li class="footer__item">
              <a href="/" class="footer__link">Investor Blog</a>
            </li>
            <li class="footer__item">
              <a href="/" class="footer__link">Bridging News</a>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </footer>
</template>
<script>
export default {
  name: "Footer",
  mounted() {
    console.log("Footer mounted");
    console.log(new Date().getDate());
  }
};
</script>

<style lang="scss">
@import "../styles/components/footer.scss";
</style>