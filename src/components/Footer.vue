<template>
  <footer>
    <div class="container">
      <div class="row">
        <div class="col d-flex pt-5 text-start">
          <div class="col">
            <h6 class="text-uppercase">DC Comics</h6>
            <ul class="list-unstyled">
              <li :key="i" v-for="(link, i) in comicLinks">
                <a href="#">{{ link }}</a>
              </li>
            </ul>
            <h6 class="text-uppercase">Shop</h6>
            <ul class="list-unstyled">
              <li :key="i" v-for="(link, i) in shopLinks">
                <a href="#">{{ link }}</a>
              </li>
            </ul>
          </div>

          <div class="col">
            <h6>DC</h6>
            <ul class="list-unstyled">
              <li :key="i" v-for="(link, i) in dcLinks">
                <a href="#">{{ link }}</a>
              </li>
            </ul>
          </div>

          <div class="col">
            <h6 class="text-uppercase">Sites</h6>
            <ul class="list-unstyled">
              <li :key="i" v-for="(link, i) in siteLinks">
                <a href="#">{{ link }}</a>
              </li>
            </ul>
          </div>
        </div>

        <div class="col">
          <div class="img-wrapper">
            <img class="maxi-logo" src="/img/dc-logo-bg.png" alt="Logo DC" />
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "TheFooter",
  data() {
    return {
      comicLinks: [
        "Characters",
        "Comics",
        "Movies",
        "TV",
        "Games",
        "Videos",
        "News",
      ],
      shopLinks: ["Shop DC", "Shop DC Collectibles"],
      dcLinks: [
        "Termo of Use",
        "Privacy Policy (New)",
        "Ad Choices",
        "Advertising",
        "Jobs",
        "Subscriptions",
        "Talent Workshop",
        "CPSC Certificates",
        "Ratings",
        "Shop Help",
        "Contact Us",
      ],
      siteLinks: [
        "DC",
        "Mad Magazin",
        "DC Kids",
        "DC Universe",
        "DC Power Visa",
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
footer {
  background-image: url("/public/img/footer-bg.jpg");
}
h6 {
  color: white;
  font-weight: bold;
  margin-bottom: 1rem;
}
li {
  margin-bottom: 0.2rem;
  & a {
    color: gray;
    text-decoration: none;
  }
}
.img-wrapper {
  max-height: 400px;
  overflow: hidden;
  position: relative;
  & img {
    height: 500px;
  }
}
</style>
