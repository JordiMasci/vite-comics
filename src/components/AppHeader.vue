<script>


export default {
  

  data() {
    return {
      links: [
        {
          text: "CHARACTERS",
          url: "#",
          current: false,
        },
        {
          text: "COMICS",
          url: "#",
          current: true,
        },
        {
          text: "MOVIES",
          url: "#",
          current: false,
        },
        {
          text: "TV",
          url: "#",
          current: false,
        },
        {
          text: "GAMES",
          url: "#",
          current: false,
        },
        {
          text: "COLLECTIBLES",
          url: "#",
          current: false,
        },
        {
          text: "VIDEO",
          url: "#",
          current: false,
        },
        {
          text: "FANS",
          url: "#",
          current: false,
        },
        {
          text: "NEWS",
          url: "#",
          current: false,
        },
        {
          text: "SHOP",
          url: "#",
          current: false,
        },
      ],
    };
  },
};
</script>

<template>
  <header>
    <div>
      <img src="/img/dc-logo.png" alt="" />
    </div>

    <ul>
      <li v-for="link in links" :key="link.url">
        <a :href="link.url" :class="link.current ? 'active' : ''">
          {{ link.text }}
        </a>
      </li>
    </ul>
  </header>
  
</template>

<style lang="scss" scoped>
header {
  height: 150px;
  max-width: 1200px;
  margin: 1rem auto;

  display: flex;
  justify-content: space-between;

  div {
    display: flex;
  }

  ul {
    display: flex;
    align-items: center;

    li {
      list-style: none;
      padding: 0.5rem;

      a {
        color: black;
        text-decoration: none;
        font-family: fantasy;

        &:hover {
          color: blue;
        }
      }
      .active {
        color: blue;
        border-bottom: 2px solid blue;
      }
    }
  }
}
</style>
