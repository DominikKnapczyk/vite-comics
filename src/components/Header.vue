<script>
export default {
  data() {
    return {
      logo: "/dc-logo.png",
      navLinks: {
        characters: {
          name: "CHARACTERS",
          link: "#",
          selected: false,
        },
        comics: {
          name: "COMICS",
          link: "#",
          selected: true,
        },
        movies: {
          name: "MOVIES",
          link: "#",
          selected: false,
        },
        tv: {
          name: "TV",
          link: "#",
          selected: false,
        },
        games: {
          name: "GAMES",
          link: "#",
          selected: false,
        },
        collectibles: {
          name: "COLLECTIBLES",
          link: "#",
          selected: false,
        },
        videos: {
          name: "VIDEOS",
          link: "#",
          selected: false,
        },
        fans: {
          name: "FANS",
          link: "#",
          selected: false,
        },
        news: {
          name: "NEWS",
          link: "#",
          selected: false,
        },
        shop: {
          name: "SHOP",
          link: "#",
          selected: false,
        },
      },
    };
  },

  methods: {
    selectNavLink(key) {
      for (let linkKey in this.navLinks) {
        if (linkKey !== key) {
          this.navLinks[linkKey].selected = false;
        } else {
          this.navLinks[linkKey].selected = true;
        }
      }
    }
  },
};
</script>

<template>
  <div class="nav-container">
    <nav>
      <div class="nav-left">
        <img :src="logo" alt="logo">
      </div>
      <div class="nav-right">
        <ul>
          <li v-for="(link, key) in navLinks"
              :key="key"
              :class="{ selected: link.selected }"
              @click="selectNavLink(key)">
            <a :href="link.link">{{ link.name }}</a>
          </li>
        </ul>
      </div>
    </nav>
  </div>
</template>

<style lang="scss" scoped>

.nav-container {
  display: flex;
  justify-content: center;
  align-items: center;

  background-color: white;
}

nav {
  display: flex;
  justify-content: space-between;
  align-items: center;

  min-width: 1100px;
  width: 80vw;
  max-width: 1400px;

  height: 120px;
  background-color: white;
}


ul {
  li {
    display: inline-block;
    margin: 0 20px;
    height: 115px;
    line-height: 115px;

    a {
      text-decoration: none;
      color: black;
      font-family:'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
      font-weight: bold;
    }
  }

}
.selected {
  border-bottom: 5px solid #0282F9;

  a {
    color: #0282F9;
  }
}

</style>