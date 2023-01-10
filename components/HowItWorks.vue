<template lang="">
  <div class="howitworks_wrapper">
    <div class="section1">
      <h2 class="section-header">How Fast Box Works</h2>
      <p class="section-subheader">
        Lorem, ipsum dolor sit amet consectetur adipisicing elit. Velit culpa
        veniam exercitationem nisi.
      </p>
    </div>
    <div class="section2">
      <div class="step-group">
        <div class="icon-block">
          <img src="../assets/icons/calendar.svg" class="icon-block-img" />
        </div>
        <b class="step-label">Step 1</b>
        <h3 class="step-group-header">Booking</h3>
        <p class="step-group-text">
          Lorem ipsum, dolor sit amet consectetur adipisicing elit. Perspiciatis
          recusandae odio omnis quos qui.
        </p>
      </div>
      <div class="step-group">
        <div class="icon-block">
          <img src="../assets/icons/box.svg" class="icon-block-img" />
        </div>
        <b class="step-label">Step 2</b>
        <h3 class="step-group-header">Packing</h3>
        <p class="step-group-text">
          Lorem ipsum, dolor sit amet consectetur adipisicing elit. Perspiciatis
          recusandae odio omnis quos qui.
        </p>
      </div>
      <div class="step-group">
        <div class="icon-block">
          <img src="../assets/icons/truck.svg" class="icon-block-img" />
        </div>
        <b class="step-label">Step 3</b>
        <h3 class="step-group-header">Transportation</h3>
        <p class="step-group-text">
          Lorem ipsum, dolor sit amet consectetur adipisicing elit. Perspiciatis
          recusandae odio omnis quos qui.
        </p>
      </div>
      <div class="step-group">
        <div class="icon-block">
          <img src="../assets/icons/plane.svg" class="icon-block-img" />
        </div>
        <b class="step-label">Step 4</b>
        <h3 class="step-group-header">Delivery</h3>
        <p class="step-group-text">
          Lorem ipsum, dolor sit amet consectetur adipisicing elit. Perspiciatis
          recusandae odio omnis quos qui.
        </p>
      </div>
    </div>
    <!-- Decorative Images -->
    <img
      src="../assets/decorative-imges/green-star.svg"
      class="hiw-green-star"
    />
    <img src="../assets/decorative-imges/gold-star.svg" class="hiw-gold-star" />
  </div>
</template>
<script>
export default {};
</script>
<style lang="scss">
.howitworks_wrapper {
  min-height: 450px;
  width: 90%;
  margin: 2em auto 4em auto;
  display: flex;
  flex-direction: column;
  position: relative;
  z-index: 2;
  .section1 {
    display: flex;
    justify-content: center;
    width: 100%;
    margin: 2em 0;
    position: relative;
    z-index: 2;
    & > * {
      margin: 0 2em;
    }
    .section-header {
      font-size: 2em;
      font-weight: bold;
      color: rgb(58, 86, 83);
    }
    .section-subheader {
      width: 25%;
      color: #777;
    }
  }
  .section2 {
    display: flex;
    .step-group {
      display: flex;
      flex-direction: column;
      align-items: center;
      .icon-block {
        height: 75px;
        width: 75px;
        background-color: rgb(60, 189, 150);
        border-radius: 8px;
        margin-bottom: 0.5em;
        color: #fff;
        display: flex;
        align-items: center;
        justify-content: center;
        .icon-block-img {
          width: 60%;
        }
      }
      .step-label {
        color: #777;
        font-size: 0.75em;
      }
      .step-group-header {
        color: rgb(58, 86, 83);
        font-size: 1.25em;
        font-weight: bold;
      }
      .step-group-text {
        color: #777;
        width: 60%;
        text-align: center;
        font-size: 0.85em;
      }
    }
  }
  /* Decorative Images */
  .hiw-green-star {
    position: absolute;
    top: 2em;
    right: 10em;
    width: 4em;
  }
  .hiw-gold-star {
    position: absolute;
    bottom: -2em;
    left: 2em;
    width: 3em;
  }
}

@media screen and (max-width: 1100px) {
  .section2 {
    flex-wrap: wrap;
    .step-group {
      width: 50%;
    }
  }
  .hiw-green-star {
    opacity: 50%;
  }
}

@media screen and (max-width: 600px) {
  .section1 {
    flex-direction: column;
    align-items: center;
    .section-subheader {
      width: 80% !important;
      text-align: center;
    }
  }
  .section2 {
    .step-group {
      width: 100%;
    }
  }
}
</style>
