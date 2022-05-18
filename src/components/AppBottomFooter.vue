<template>
  <main class="footer-bottom">
    <div class="footer-bottom-wrapper container">
      <button>Sign-up Now</button>

      <div class="icons-container">
        <h3>FOLLOW US</h3>
        <img src="../assets/img/footer-facebook.png" alt="facebook" />
        <img src="../assets/img/footer-youtube.png" alt="youtube" />
        <img src="../assets/img/footer-twitter.png" alt="twitter" />
        <img src="../assets/img/footer-pinterest.png" alt="pinterest" />
        <img src="../assets/img/footer-periscope.png" alt="periscope" />
      </div>
    </div>
  </main>
</template>

<script>
export default {

};
</script>

<style lang="scss" scoped>
@import "../style/common.scss";
.footer-bottom {
  background-color: rgba(48,48,48,255);
  padding: 1.2rem 0;

}
.footer-bottom-wrapper {
  display: flex;
  align-items: center;
  justify-content: space-between;
}
button {
  color: white;
  padding: 1rem;
  font-weight: bold;
  font-size: 1rem;
  border: 2px solid rgba(2,130,249,255);
  background-color: rgba(48,48,48,255);
  text-transform: uppercase;
}
.icons-container {
  display: flex;
  align-items: center;
  h3 {
    color: rgba(2,130,249,255);
    font-size: 1rem;
  }
  img {
    width: 10%;
    margin: 0 0.3em;
  }
}
</style>