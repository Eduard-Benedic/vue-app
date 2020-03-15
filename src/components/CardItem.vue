<template>
  <div class="card">
    <div class="card__header">
      <img class="card__logo" src="../assets/card-logo-round.jpg" alt="Kuflnik logo white" />
      <div class="card__info">
        <h2 class="card__title">{{cardData.title}}</h2>
        <h3 v-if="cardData.subtitle" class="card__subtitle">{{cardData.subtitle}}</h3>
      </div>
    </div>
    <img src="../assets/card-icon.png" class="card__img" />
    <p class="card__p">{{cardData.description}}</p>
    <div class="card__footer">
      <div class="card__actions">
        <a class="button button--main" href="/">Login</a>
        <a class="button button--secondary" href="/">Register</a>
      </div>
      <ul class="share">
        <li class="share__item">
          <a href="/" class="share__link share__link--green">
            <font-awesome-icon icon="heart" />
          </a>
        </li>
        <li class="share__item">
          <a href="/" class="share__link share__link--green">
            <font-awesome-icon icon="share-alt" />
          </a>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "CardItem",
  props: {
    cardData: Object
  }
};
</script>

<style lang="scss">
@import "../styles/components/card.scss";
@import "../styles/setup/grids";
@import "../styles/components/share";
@import "../styles/components/button";
</style>
