<script>
export default {
  data() {
    return {
      loghi: [
        {
          image: "/img/footer-facebook.png",
          url: "#",
        },
        {
          image: "/img/footer-twitter.png",
          url: "#",
        },
        {
          image: "/img/footer-youtube.png",
          url: "#",
        },
        {
          image: "/img/footer-pinterest.png",
          url: "#",
        },
        {
          image: "/img/footer-periscope.png",
          url: "#",
        },
      ],
    };
  },
};
</script>

<template>
  <footer>
    <div class="container div-container">
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
        <div v-for="logo in loghi" :key="logo.url">
          <img :src="logo.image" alt="" />
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
// PRIMA PARTE FOOTER
footer {
  position: relative;
  height: 400px;
  background-image: url("./img/footer-bg.jpg");

  .div-container {
    position: absolute;
    background-image: url("./img/dc-logo-bg.png");
    background-repeat: no-repeat;
    background-position: 750px -50px;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    z-index: 2;
  }
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
      align-items: center;

      p {
        margin: 0 15px;
        color: blue;
        font-size: 20px;
      }

      img {
        width: 30px;
        height: 30px;
        margin: 0 10px;
      }
    }
  }
}
</style>
