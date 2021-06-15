<template>
  <div class="fasteningSystem">
    <div class="fasteningSystem__img">
      <img src="../assets/img-2.png" alt="" />
    </div>
    <div class="fasteningSystem__info">
      <h3 class="fasteningSystem__decor">LOCK</h3>
      <h4 class="fasteningSystem__title">
        <span> Lock</span> and <span> balance</span> mounting system
      </h4>
      <p class="fasteningSystem__subtitle">
        There is no standard for how to attach and balance a lens on a drone, so
        we made one. Introducing our Lock and Balance Mounting System. It’s a
        two part design with a lens on one side and a counterweight on the
        other. The two parts clamp together over the drone’s camera, creating a
        secure lock that doesn’t impede the gimbal.
      </p>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>

.fasteningSystem {
    box-sizing: border-box;
    display: flex;
    margin-top: 700px;

  &__img {
 
   position: relative;   

   margin:147px 98px 180px 0px ;
  }
  &__logo {
    position: absolute;
    right: -12px;
    top: -6px;
  }
  &__info {
      margin-top:179px;
  }
  &__decor {
    position: absolute;
    top: 160px;
    font-size: 100px;
    font-weight:900 ;
    text-transform: uppercase;
    color: rgba(246, 246, 246, 0.05);
    margin: 0;
  }
  &__title {
    max-width: 500px;
    width: 100%;
    font-family: "Roboto Condensed", sans-serif;
    font-size: 40px;
    font-weight: 700;
    color: #fff;
    font: 700;
     margin: 0;
     padding-top:50px ;
  }
    span {
        color: #fdc400;
    }
    
    &__subtitle{
        padding-top:20px;
        margin: 0;
        max-width: 574px;
        width: 100%;
        font-family: "MuseoModerno";
        font-weight: 300;
        font-size: 16px;
        line-height: 28px;
        color: #fff;
    }

  }
</style>