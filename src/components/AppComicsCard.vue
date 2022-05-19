<template>
  <div class="card">
    <img
      :src="comicsObject.thumb"
      alt=""
    />
    <h3>{{ comicsObject.series }}</h3>
  </div>
</template>

<script>
export default {
  name: "AppComicsCard",
  props: {
    comicsObject: Object,
  },
};
</script>

<style lang="scss" scoped>
.card {
  width: calc(100% / 6);
}
</style>