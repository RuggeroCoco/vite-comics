<script>
import img1 from "../assets/buy-comics-digital-comics.png";
import img2 from "../assets/buy-comics-merchandise.png";
import img3 from "../assets/buy-comics-subscriptions.png";
import img4 from "../assets/buy-comics-shop-locator.png";
import img5 from "../assets/buy-dc-power-visa.svg";

export default {
  data() {
    return {
      links: [
        {
          title: "Digital Comics",
          icon: img1,
          url: "/",
        },
        {
          title: "Digital Comics",
          icon: img2,
          url: "/",
        },
        {
          title: "Digital Comics",
          icon: img3,
          url: "/",
        },
        {
          title: "Digital Comics",
          icon: img4,
          url: "/",
        },
        {
          title: "Digital Comics",
          icon: img5,
          url: "/",
        },
      ],
    };
  },
};
</script>

<template>
  <div class="buy-comics">
    <div v-for="(link, index) in links" :key="index.toString()">
      <a class="buy-comics_link" :href="link.url">
        <img :src="link.icon" alt="" />
        <p>{{ link.title }}</p>
      </a>
    </div>
  </div>
  <div></div>
  <div></div>
</template>

<style scoped lang="scss">
.buy-comics {
  background-color: blue;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 40px 10vw;

  &_link {
    display: flex;
    align-items: center;
    color: white;
    img {
      max-height: 80px;
      max-width: 60px;
      margin-right: 20px;
      object-fit: contain;
    }
  }
}
</style>
