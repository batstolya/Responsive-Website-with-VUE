<template>
  <div class="product">
    <div class="product__img" :class="className"></div>
    <h6 class="product__title">{{ title }}</h6>
    <p class="product__subtitle" v-if="subtitle">
      {{ subtitle }}
    </p>
    <div class="product__cost">
      <span class="product__prise"  >{{ prise }}</span>
      <span class="product__discount">{{ discount }}</span>
    </div>
    <Button :product="true" title="Buy" />
  </div>
</template>

<script>
import Button from "./Button";
export default {
  name: "product",
  data() {
    return {};
  },
  components: { Button },

  props: {
    title: {
      type: String,
      default: "Fire engine red filters set",
    },
    subtitle: {
      type: String,
      default:
        "These baby filters make your drone look faster. Or at least you won’t lose them like those other black filters",
    },
    prise: {
      type: String,
      default: "200 USD",
    },

    discount: {
      type: String,
      default: "",
    },

    img1: {
      type: Boolean,
      default: false,
    },
    img2: {
      type: Boolean,
      default: false,
    },
    img3: {
      type: Boolean,
      default: false,
    },
    img4: {
      type: Boolean,
      default: false,
    },
  },
  computed: {
    className() {
      return {
        product__img1: this.img1,
        product__img2: this.img2,
        product__img3: this.img3,
        product__img4: this.img4,
      };
    },
  },
};
</script>

<style scoped lang="scss">
.product {
  display: flex;
  flex-direction: column;
  max-width: 272px;
  width: 100%;
  color: #fff;
  padding-bottom: 160px;
  &__img1 {
    width: 272px;
    height: 198px;
    background: url("../assets/Product-1.png") no-repeat center;
  }
  &__img2 {
    width: 272px;
    height: 198px;
    background: url("../assets/Product-2.png") no-repeat center;
  }
  &__img3 {
    width: 272px;
    height: 198px;
    background: url("../assets/Product-3.png") no-repeat center;
  }
  &__img4 {
    width: 272px;
    height: 198px;
    background: url("../assets/Product-4.png") no-repeat center;
  }

  &__title {
    padding-top: 70px;
    margin: 0;
    font-family: "Roboto Condensed";
    font-weight: 700;
    font-size: 22px;
   color: #fff;
  }
  &__subtitle {
  
    line-height: 28px;
    padding-top: 27px;
    padding-bottom: 30px;

    margin: 0;
    font-size: 16px;
    font-weight: 300;
   color: #fff;
  }

  &__cost {
    padding-bottom: 50px;
    display: flex;
    color: #fff;
  }
  &__prise {
    padding-right: 35px;
  }
  &__discount{
    color: #AFAFAF;
    text-decoration: line-through;
  }
}
</style>