<template>
  <div class="main-links">
    <div class="container">
      <ul class="links-list">
        <li v-for="(element, index) in icons" :key="index">
          <img :src="require(`../assets/img/${element.img}`)" alt="" />
          <h3>{{ element.text }}</h3>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "AppMainLinks",
  data: function () {
    return {
      icons: [
        {
          img: "buy-comics-digital-comics.png",
          text: "Digital Comics",
        },
        {
          img: "buy-comics-merchandise.png",
          text: "DC merchandise",
        },
        {
          img: "buy-comics-subscriptions.png",
          text: "Subscription",
        },
        {
          img: "buy-comics-shop-locator.png",
          text: "Comic shop locator",
        },
        {
          img: "buy-dc-power-visa.svg",
          text: "DC power visa",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../style/common.scss";

.main-links{
  background-color: rgba(2,130,249,255);
  color: white;
  padding: 2rem 0;
  .links-list {
    display: flex;
    li {
      width: calc(100% / 5);
      display: flex;
      align-items: center;
      padding: .5rem;
      img {
        width: 20%;
        margin-right: 1rem;
      }
    }
  }
}
</style>
