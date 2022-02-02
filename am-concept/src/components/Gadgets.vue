<template>
  <div class="gadgets">
    <h4 class="gadgets__title">Buy a set with a <span>30%</span> discount</h4>
    <p class="gadgets__subtitle">
      These baby filters make your drone look faster. Or at least you won’t lose
      them like those other black filters
    </p>
    <div class="gadgets__products">
      <Product :img1="true" discount="270 USD" />
      <Product
        :img2="true"
        subtitle="Not only do these filters work seamlessly with the camera mounts on both Mavic 2 Drones..."
      />
      <Product
        :img3="true"
        subtitle="The helipad that does more for you. Like a changing mat for your surf session, the landing pad acts as..."
      />
      <Product
        :img4="true"
        subtitle=" Inspired by filmmakers, drone flyers, and minimalists this is the case you don’t have to take off to use. "
        discount="210 USD"
      />
    </div>
  </div>
</template>

<script>
import Product from "@/components/Product";

export default {
  // name: "App",
  components: {
    Product,
  },
};
</script>


<style lang="scss" scoped>
.gadgets {

  color: #fff;
  &__title {
    font-family: "Roboto Condensed";
    font-size: 40px;
    font-weight: 700;
    margin: 0;
    padding: 0;
    span {
      color: #fdc400;
    }
    
  }
  &__subtitle {
      max-width: 550px;
      width: 100%;
      font-weight: 300;
      font-size: 16px;
      margin-top: 23px;
      margin-bottom: 70px;
      line-height: 28px;
    }
  &__products {
    display: flex;
    justify-content: space-between;
      flex-wrap: wrap;
  }
}
</style>>

