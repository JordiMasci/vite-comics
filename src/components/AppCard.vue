<script>
export default {
  props: {
    card: {
      type: Object,
    },
  },
};
</script>

<template>
  <div class="card">
    <img :src="card.thumb" alt="" />
    <h3 class="title">{{ card.series }}</h3>
  </div>
</template>

<style lang="scss" scoped>
.card {
  width: calc(100% / 6);

  color: white;

  img {
    max-width: 100%;
    height: 281px;
  }
}
</style>
