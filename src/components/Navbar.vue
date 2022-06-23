<template>
  <header>
    <div class="container">
      <nav class="row justify-content-between py-4">
        <div class="col d-flex justify-content-start">
          <img src="/img/dc-logo.png" alt="Logo DC" />
        </div>

        <div class="col-8 d-flex justify-content-end align-items-center">
          <ul class="nav list-unstyled my-nav">
            <li v-for="(link, i) in navLinks" :key="i">
              <a class="p-3 text-uppercase" :href="link.href">{{
                link.name
              }}</a>
            </li>
          </ul>
        </div>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: "TheHeader",
  data() {
    return {
      navLinks: [
        {
          name: "Characters",
          href: "#",
        },
        {
          name: "Comics",
          href: "#",
        },
        {
          name: "Movies",
          href: "#",
        },
        {
          name: "TV",
          href: "#",
        },
        {
          name: "Games",
          href: "#",
        },
        {
          name: "Collectibles",
          href: "#",
        },
        {
          name: "Videos",
          href: "#",
        },
        {
          name: "Fans",
          href: "#",
        },
        {
          name: "News",
          href: "#",
        },
        {
          name: "Shop",
          href: "#",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
.my-nav {
  font-size: 12px;
  font-weight: bold;
  margin: 0;
  & a {
    color: black;
    text-decoration: none;
  }
}
</style>
