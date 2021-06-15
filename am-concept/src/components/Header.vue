<template>
  <header class="header">
    <div class="logo">
      <img class="logo__img" src="../assets/logo.png" alt="" />
      <span class="logo__title"> Moments of air</span>
    </div>
    <ul class="header__ul">
      <a href="#"> <li>Features</li></a>
      <a href="#"><li>Technologies</li></a>
      <a href="#"><li>Who we are</li></a>
      <a href="#"><li>How do we deliver</li></a>
    </ul>
    <Button />
  </header>
</template>

<script>
import Button from "@/components/Button";
export default {
  name: "Header",
  components: {
    Button,
  },
};
</script>

<style lang="scss" scoped>
@import url("/fonts/proxima-nova-condensed-regular.ttf");
.header {
  margin: 0 auto;
  display: flex;
  justify-content: space-between;
  align-items: center;
  color: #fff;
  padding-top: 50px;

  .logo {
    z-index: 1;
    display: flex;
    align-items: center;
    &__title {
      text-transform: uppercase;
      font-family: "Roboto Condensed", sans-serif;
      font-weight: 300;
    }
  }

  &__ul {
    font-family: "MuseoModerno", cursive;
    font-weight: 300;
    max-width: 515px;
    width: 100%;
    display: flex;
    justify-content: space-between;
    list-style-type: none;
    z-index: 1;
    a {
      text-decoration: none;
        color: #fff;
        font-size: 14px;
    }
  }
}
</style>