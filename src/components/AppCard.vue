<script>
// import MyComponent from "./components/MyComponent. vue!";

export default {
  data() {
    return {
      title: "Hello world",
    };
  },

  // components: {
  //   MyComponent,
  // },
};
</script>

<template>
  <div class="container">
    <div class="card-container">
      <div class="card"></div>
      <div class="card"></div>
      <div class="card"></div>
      <div class="card"></div>
      <div class="card"></div>
      <div class="card"></div>
      <div class="card"></div>
      <div class="card"></div>
      <div class="card"></div>
      <div class="card"></div>
      <div class="card"></div>
      <div class="card"></div>
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
        width: calc(100% / 7);
        min-height: 200px;
        border: 2px solid red;
      }
  }
}
</style>
