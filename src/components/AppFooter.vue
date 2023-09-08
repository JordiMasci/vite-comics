<script>
export default {};
</script>

<template>
  <footer>
    <div class="container">
      <div></div>
      <div></div>
      <div></div>
    </div>
  </footer>

  <div class="foot">
    <div class="container">
      <button>SIGN-UP NOW!</button>
      <div class="loghi">
        <p>FOLLOW US</p>
        <img src="/img/footer-facebook.png" alt="" />
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
// PRIMA PARTE FOOTER
footer {
  height: 500px;
  background-image: url("./img/footer-bg.jpg");
}

// SECONDA PARTE FOOTER
.foot {
  height: 130px;
  background-color: #303030;
  .container {
    max-width: 1200px;
    height: 100%;
    margin: 0 auto;

    display: flex;
    justify-content: space-between;

    button {
      background-color: #303030;
      color: white;
      border: 1px solid #0d6dc6;
      height: 50px;
      align-self: center;
    }

    .loghi {
        display: flex;
    }
  }
}
</style>
