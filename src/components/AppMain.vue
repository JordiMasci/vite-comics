<script>
import AppCard from "./AppCard.vue";
export default {
  components: { AppCard },

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
      cards: [
        {
          thumb: "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
          price: "$19.99",
          series: "Action Comics",
          type: "comic book",
        },
        {
          thumb:
            "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
          price: "$3.99",
          series: "American Vampire 1976",
          type: "comic book",
        },
        {
          thumb:
            "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
          price: "$16.99",
          series: "Aquaman",
          type: "graphic novel",
        },
        {
          thumb: "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
          price: "$2.99",
          series: "Batgirl",
          type: "comic book",
        },
        {
          thumb:
            "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
          price: "$3.99",
          series: "Batman",
          type: "comic book",
        },
        {
          thumb:
            "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
          price: "$2.99",
          series: "Batman Beyond",
          type: "comic book",
        },
        {
          thumb:
            "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
          price: "$3.99",
          series: "Batman/Superman",
          type: "comic book",
        },
        {
          thumb:
            "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
          price: "$4.99",
          series: "Batman/Superman Annual",
          type: "comic book",
        },
        {
          thumb:
            "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
          price: "$5.99",
          series: "Batman: The Joker War Zone",
          type: "comic book",
        },
        {
          thumb:
            "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
          price: "$6.99",
          series: "Batman: Three Jokers",
          type: "comic book",
        },
        {
          thumb:
            "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
          price: "$4.99",
          series: "Batman: White Knight Presents: Harley Quinn",
          type: "comic book",
        },
        {
          thumb:
            "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
          price: "$16.99",
          series: "Catwoman",
          type: "graphic novel",
        },
      ],
    };
  },
};
</script>

<template>
  <main>
    <div class="contents">
      <AppCard v-for="(card, index) in cards" :card="card" :key="index"></AppCard>
    </div>
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
  min-height: 150px;
  background-color: black;
  

  div {
    max-width: 1200px;
    margin: 0 auto;
  }
  .contents {
    background-color: #1c1c1c;
    color: white;

    display: flex;
    flex-wrap: wrap;
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
