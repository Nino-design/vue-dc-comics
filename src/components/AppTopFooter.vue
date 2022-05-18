<template>
  <div class="footer">
    <div class="footer-wrapper container">
      <div class="col">
        <div>
          <h3>DC COMICS</h3>
          <ul>
            <li v-for="(element, index) in icons" :key="index">
              {{ element.text }}
            </li>
          </ul>
          <h3>SHOP</h3>
          <ul>
            <li v-for="(element, index) in icons2" :key="index">
              {{ element.text }}
            </li>
          </ul>
        </div>

        <div class="col">
          <h3>DC</h3>
          <ul>
            <li v-for="(element, index) in icons3" :key="index">
              {{ element.text }}
            </li>
          </ul>
        </div>

        <div class="col">
          <h3>SITES</h3>
          <ul>
            <li v-for="(element, index) in icons4" :key="index">
              {{ element.text }}
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "AppTopFooter",
  data: function () {
    return {
      icons: [
        {
          url: "#",
          text: "Characters",
        },
        {
          url: "#",
          text: "Comics",
        },
        {
          url: "#",
          text: "Movies",
        },
        {
          url: "#",
          text: "Tv",
        },
        {
          url: "#",
          text: "Games",
        },
        {
          url: "#",
          text: "Videos",
        },
        {
          url: "#",
          text: "News",
        },
      ],
      icons2: [
        {
          url: "#",
          text: "Shop DC",
        },
        {
          url: "#",
          text: "Shop DC Collectibles",
        },
      ],
      icons3: [
        {
          url: "#",
          text: "Terms Of Use",
        },
        {
          url: "#",
          text: "Privacy policy (New)",
        },
        {
          url: "#",
          text: "Ad Choices",
        },
        {
          url: "#",
          text: "Advertising",
        },
        {
          url: "#",
          text: "Jobs",
        },
        {
          url: "#",
          text: "Subscription",
        },
        {
          url: "#",
          text: "Talent Workshops",
        },
        {
          url: "#",
          text: "CPSC Certificates",
        },
        {
          url: "#",
          text: "Ratings",
        },
        {
          url: "#",
          text: "Shop Help",
        },
        {
          url: "#",
          text: "Contact Us",
        },
      ],
      icons4: [
        {
          url: "#",
          text: "DC",
        },
        {
          url: "#",
          text: "Mad Magazines",
        },
        {
          url: "#",
          text: "DC Kids",
        },
        {
          url: "#",
          text: "DC Universe",
        },
        {
          url: "#",
          text: "DC Power Visa",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../style/common.scss";
.footer {
  height: 250px;
  background: url(../assets/img/dc-logo-bg.png) right bottom no-repeat,
    url(../assets/img/footer-bg.jpg);
  background-size: 100% contain;
}

.footer-wrapper {
  display: flex;
  justify-content: flex-start;
}

.col {
  display: flex;
  margin-top: 1em;
}

h3 {
  font-size: 0.8rem;
  color: white;
  margin-bottom: 0.8rem;
}

ul li {
  color: lightgray;
  line-height: 1rem;
  font-size: 0.6rem;
}
</style>
