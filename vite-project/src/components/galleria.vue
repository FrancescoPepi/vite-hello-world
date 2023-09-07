<script>
export default {
  data() {
    return {
      img: "../../img/mobile-logo.png",
    };
  },

  methods: {
    printImg(img) {
      const imgUrl = new URL(img, import.meta.url);
      console.log(imgUrl);
      return imgUrl.href;
    },
  },
};
</script>
<template>
  <div>
    <img :src="printImg(img)" alt="asdas" />
  </div>
</template>
<style lang="scss" scoped>
img {
  width: 50%;
}
</style>
