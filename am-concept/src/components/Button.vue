<template>
  <button class="button" :class="className">
    {{ title }}
  </button>
</template>

<script>
export default {
  name: "button",
  data() {
    return {};
  },
  props: {
    title: {
      type: String,
      default: "Buy a set",
    },
    title2: {
      type: String,
      default: "Buy",
    },
    color: {
      tyle: String,
      default: "Black",
    },
    color2: {
      type: String,
      default: "white",
    },
    background: {
      type: Boolean,
      default: false,
    },
    product:{
      type: Boolean,
      default: false,
    }
  },
  computed: {
    className() {
      return {
        button__background: this.background,
        button__product: this.product,

      };
    },
  },
};
</script>

<style scoped lang="scss">
$base-color: #fdc400;
.button {
  transition: 0.5s;
  cursor: pointer;
  max-width: 160px;
  width: 100%;
  height: 54px;
  border: 1px solid #fdc400;
  box-sizing: border-box;
  border-radius: 5px;
  background: #0101;
  color: #fff;
  font-size: 16px;
  z-index: 1;
  &__background {
    background-color: $base-color;
  }
  &__product {
    max-width: 272px;
    width: 100%;
    height: 54px;
    background: #0101;
  }
  &:hover {
    background: #fdc200a1;
  }
}
</style>