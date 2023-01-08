<template lang="">
  <div class="howitworks_wrapper">
    <div class="section1">
      <h2 class="section-header">Our Specialties</h2>
      <p class="section-subheader">
        Lorem, ipsum dolor sit amet consectetur adipisicing elit. Velit culpa
        veniam exercitationem nisi.
      </p>
    </div>
    <div class="section2">
      <div class="step-group">
        <div class="step-group-left">01</div>
        <div class="step-group-right">
          <h3>Easy to order</h3>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipisicing elit.
            Architecto, sint.
          </p>
        </div>
      </div>
      <div class="step-group">
        <div class="step-group-left">02</div>
        <div class="step-group-right">
          <h3>Cash on delivery</h3>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipisicing elit.
            Architecto, sint.
          </p>
        </div>
      </div>
      <div class="step-group">
        <div class="step-group-left">03</div>
        <div class="step-group-right">
          <h3>Live tracking</h3>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipisicing elit.
            Architecto, sint.
          </p>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {};
</script>
<style lang="scss" scoped>
.howitworks_wrapper {
  height: 450px;
  width: 90%;
  margin: 2em auto;
  display: flex;
  flex-direction: column;
  .section1 {
    display: flex;
    justify-content: center;
    width: 100%;
    margin: 2em 0;
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
    justify-content: space-evenly;
    width: 75%;
    margin: 0 auto;
    .step-group {
      display: flex;
      justify-content: center;
      flex-direction: row;
      width: 400px;
      .step-group-left {
        font-size: 2em;
        font-weight: lighter;
        color: rgb(60, 189, 150);
        margin-right: 1em;
        align-self: flex-start;
      }
      .step-group-right {
        width: 50%;
        h3 {
          font-weight: 900;
        }
        p {
          color: #777;
        }
      }
    }
  }
}
</style>
