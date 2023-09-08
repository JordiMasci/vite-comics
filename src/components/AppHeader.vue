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
    <ul>
      <li v-for="link in links">
        <a :href="link.url" :class="link.current ? 'active' : ''">
          {{ link.text }}
        </a>
      </li>
    </ul>
  </header>
</template>

<style lang="scss" scoped>
    
    li {
        list-style: none;

        a {
            color: black;
            text-decoration: none;

        }
        .active {
            color: blue;
            border-bottom: 2px solid blue;
        }
    }
</style>
