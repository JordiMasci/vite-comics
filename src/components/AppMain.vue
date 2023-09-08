<script>
export default {
  data() {
    return {
      marchi: [
        {
          text: "CHARACTERS",
          image: "/img/buy-comics-digital-comics.png",
          url: "#",
        },
        {
          text: "DC MERCHANDISE",
          image: "/img/buy-comics-merchandise.png",
          url: "#",
        },
        {
          text: "SUBSCRIPTION",
          image: "/img/buy-comics-subscriptions.png",
          url: "#",
        },
        {
          text: "COMIC SHOP LOCATOR",
          image: "/img/buy-comics-shop-locator.png",
          url: "#",
        },
        {
          text: "DC POWER VISA",
          image: "/img/buy-dc-power-visa.svg",
          url: "#",
        },
      ],
    };
  },
};
</script>

<template>
  <main>
    <div class="contents">- -> Contents goes here - -</div>
  </main>
  <div class="container">
    <div class="marchi">
      <div class="flex" v-for="marchio in marchi" :key="marchio.url">
        <img :src="marchio.image" alt="" />
        <p>
          {{ marchio.text }}
        </p>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
main {
  height: 150px;
  line-height: 150px;
  background-color: black;

  div {
    max-width: 1200px;
    margin: 0 auto;
  }
  .contents {
    color: white;
    font-size: 30px;
  }
}

.container {
  height: 170px;
  background-color: #0282f9;

  .marchi {
    max-width: 1200px;
    margin: 0 auto;
    height: 100%;
    justify-content: space-around;

    display: flex;

    .flex {
      display: flex;
      align-items: center;

      img {
        width: 50px;
      }

      p {
        margin: 0.5rem;
        color: white;
      }
    }
  }
}
</style>
