<script>
export default {
  data() {
    return {
      buttons: [
        {
          title: "Characters",
          url: "/",
          current: false,
        },
        {
          title: "Characters",
          url: "/",
          current: false,
        },
        {
          title: "Characters",
          url: "/",
          current: false,
        },
        {
          title: "Characters",
          url: "/",
          current: false,
        },
        {
          title: "Characters",
          url: "/",
          current: false,
        },
        {
          title: "Characters",
          url: "/",
          current: false,
        },
        {
          title: "Characters",
          url: "/",
          current: false,
        },
        {
          title: "Characters",
          url: "/",
          current: false,
        },
        {
          title: "Characters",
          url: "/",
          current: false,
        },
      ],
    };
  },
};
</script>

<template>
  <div class="header">
    <img src="../assets/dc-logo.png" alt="Logo" />
    <div v-for="(button, index) in buttons" :key="index.toString()">
      <input type="button" :value="button.title" />
    </div>
  </div>
</template>

<style scoped>
.header {
  width: 100%;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
</style>
