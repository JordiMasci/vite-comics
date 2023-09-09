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
    <div class="div-container">
      <div class="container">
        <div>
          <h3>DC COMICS</h3>
          <ul>
            <li>Characters</li>
            <li>Comics</li>
            <li>Movies</li>
            <li>Tv</li>
            <li>Games</li>
            <li>Videos</li>
            <li>News</li>
          </ul>
          <h3>SHOP</h3>
          <ul>
            <li>Shop DC</li>
            <li>Shop DC Collectibles</li>
          </ul>
        </div>
        <div>
          <h3>DC</h3>
          <ul>
            <li>Term Of Use</li>
            <li>Privacy Policy (News)</li>
            <li>Ad Choises</li>
            <li>Advertising</li>
            <li>Jobs</li>
            <li>Subscriptions</li>
            <li>Talent Whork Shop</li>
            <li>CPSC Certificates</li>
            <li>Ratings</li>
            <li>Shop Help</li>
            <li>Contact Us</li>
          </ul>
        </div>
        <div>
          <h3>SITES</h3>
          <ul>
            <li>DC</li>
            <li>Mad Magazine</li>
            <li>DC Kids</li>
            <li>DC Universe</li>
            <li>DC Power Visa</li>
          </ul>
        </div>
      </div>
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

  .container {
    display: flex;
    max-width: 1200px;
    height: 100%;
    margin: 0 auto;

    div {
      margin-right: 50px;
    }

    h3 {
      color: white;
      font-size: 25px;
    }

    ul {
      padding-inline-start: 0;

      li {
        color: #817a7a;
        list-style: none;
        font-size: 15px;
        line-height: 1.5;
      }
    }
  }

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
