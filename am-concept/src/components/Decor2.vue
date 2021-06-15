<template>
  <div class="decor2 product">
    <span class="decor2__title">ENTIAL BLOGGER</span>
    <span class="decor2__subtitle"
      >Essential lens, filters, and cases for drones</span
    >
    <div class="product__interaction interaction">
      <Button :background="true" />
      <a href="#" class="interaction__delirev"><p>How do we deliver?</p></a>
      <a href="#" class="interaction__switch"
        ><img src="../assets/decor-2.png" alt=""
      /></a>
    </div>
  </div>
</template>

<script>
import Button from "@/components/Button";

export default {
  name: "Decor2",
  components: {
    Button,
  },
};
</script>

<style scoped lang="scss">
.decor2 {
  position: absolute;
  top: 299px;
  left: -75px;

  max-width: 925px;
  width: 100%;
  height: 447px;
  display: block;
  background: #191e21;
  z-index: 0;

  &__title {
    // font-family: "Roboto";
    position: absolute;
    top: 65px;
    left: 100px;
    font-size: 100px;
    color: rgba(246, 246, 246, 0.05);

    font-family: "Roboto Condensed";
  }
  &__subtitle {
    max-width: 752px;
    position: absolute;
    top: 90px;
    left: 100px;
    color: #fff;
    font-family: "Roboto Condensed";
    font-weight: 700;
    font-size: 74px;
  }

  .interaction {
    max-width: 400px;
    width: 100%;

    display: flex;
    align-items: center;

    position: absolute;
    top: 308px;
    left: 100px;
    &__delirev {
      color: #fff;
      font-size: 16px;
      margin-left: 35px;
      text-decoration: none;
      padding-right: 20px;
    }
  }
}
</style>