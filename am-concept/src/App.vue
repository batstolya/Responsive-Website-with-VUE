<template>
  <section class="first">
    <div class="container">
      <Header />
      <Decor />
      <Decor2 />
    </div>
  </section>

  <section class="second">
    <div class="container">
      <Preview />
      <Gadgets />
    </div>
  </section>

  <section class="third">
    <div class="container">
      <FasteningSystem/>
    </div>
  </section>
</template>

<script>
import Header from "./components/Header";
import Preview from "./components/Preview";
import Gadgets from "./components/Gadgets";
import Decor from "./components/Decor";
import Decor2 from "./components/Decor2";
import FasteningSystem from "./components/FasteningSystem";


export default {
  name: "App",

  components: {
    Header,

    Preview,
    Gadgets,
    Decor,
    Decor2,
    FasteningSystem
  },
};
</script>

<style lang='scss'>
@import url("https://fonts.googleapis.com/css2?family=MuseoModerno:wght@300;400;700&family=Roboto+Condensed:wght@400;700&display=swap");
$base-color: #fdc400;

html,
body {
  margin: 0;
  padding: 0;
}
#app {
  // font-family: "MuseoModerno", cursive;
  font-family: "Roboto Condensed", sans-serif;
  // font-family: Avenir, Helvetica, Arial, sans-serif;
  // -webkit-font-smoothing: antialiased;
  // -moz-osx-font-smoothing: grayscale;
  // text-align: center;
  // color: #2c3e50;
  // margin-top: 60px;
  background: #191e21;
  max-width: 1440px;
  width: 100%;
  height: 4000px;
  margin: 0 auto;
}
.first {
  background: url("assets/bg-1.png") no-repeat center;
  height: 745px;
}

.second {
  max-width: 1440px;
  margin: 0 auto;
  background: #191e21;
    height: 872px;
}

.container {
  box-sizing: border-box;
  max-width: 1290px;
  padding: 0 20px 0 20px;
  width: 100%;
  height: 1000px;

  margin: 0 auto;
  // border: $base-color solid 5px;
  position: relative;
}
</style>
