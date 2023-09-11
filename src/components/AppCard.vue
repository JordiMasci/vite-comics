<script>
export default {

  props: {
    files: {
      type: Array,
    },
  },
};
</script>

<template>
  <div class="container">
    <div class="card-container">
      <div class="card" v-for="(file, index) in files" :key="index">
        <img :src="file.thumb" alt="" />
        <h3 class="title">{{ file.series }}</h3>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.container {
  background-color: #1c1c1c;
  .card-container {
    max-width: 1200px;
    margin: 0 auto;
    min-height: 200px;

    display: flex;
    flex-wrap: wrap;

    .card {
      width: 16%;
      min-height: 200px;
      border: 2px solid red;

      gap: 1%;
      color: white;

      img {
        max-width: 100%;
      }
    }
  }
}
</style>
