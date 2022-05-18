<template>
  <header class="header">
    <div class="header-wrapper container">
      <div class="header-img">
        <img src="../assets/img/dc-logo.png" alt="dc-logo." />
      </div>
      <div>
        <ul class="header-list">
          <li
            v-for="(element, index) in headerList"
            :key="index"
            :class="{ active: element.active }"
          >
            <a href="">{{ element.text }}</a>
          </li>
        </ul>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: "AppHeader",
  data: function () {
    return {
      headerList: [
        {
          url: "#",
          text: "Characters",
          active: false,
        },
        {
          url: "#",
          text: "Comics",
          active: true,
        },
        {
          url: "#",
          text: "Movies",
          active: false,
        },
        {
          url: "#",
          text: "Tv",
          active: false,
        },
        {
          url: "#",
          text: "Games",
          active: false,
        },
        {
          url: "#",
          text: "Collectibles",
          active: false,
        },
        {
          url: "#",
          text: "Videos",
          active: false,
        },
        {
          url: "#",
          text: "Fans",
          active: false,
        },
        {
          url: "#",
          text: "News",
          active: false,
        },
        {
          url: "#",
          text: "Shop",
          active: false,
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../style/common.scss";

.header-wrapper {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-top: 2rem;
}

.header-img img {
  width: 60%;
}

.header-list {
  display: flex;
}

.header-list li {
  margin: 1rem;
  font-weight: 500;
  text-transform: uppercase;
  line-height: 50px;
}
</style>
