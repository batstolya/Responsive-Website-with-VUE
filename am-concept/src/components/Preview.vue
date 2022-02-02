<template>
  <div class="preview">
    <div class="preview__img">
      <img src="../assets/img-1.png"  alt="" />
      <img class="preview__logo"  src="../assets/logo-2.png"  alt="" />
    </div>
    <div class="preview__info">
      <h3 class="preview__decor">essential</h3>
      <h4 class="preview__title">
        Essential <span class="color">blogger</span> accessories and
        <span>filmmaker’s </span> tool
      </h4>
      <p class="preview__subtitle">
        We put our prototypes in the hands of our favorite drone flyers and
        filmmakers. What they captured in a few days blew our minds. We can't
        wait to see what you capture with this gear.
      </p>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>

.preview {
    box-sizing: border-box;
    display: flex;



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
