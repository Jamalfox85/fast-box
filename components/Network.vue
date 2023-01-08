<template lang="">
  <div class="network_wrapper">
    <div class="network_left">
      <img src="../assets/images/network_truck.svg" class="network-img" />
    </div>
    <div class="network_right">
      <h2 class="network-header">We Have the Largest Network</h2>
      <p class="network-text">
        Lorem ipsum, dolor sit amet consectetur adipisicing elit. Molestiae
        error dolor, excepturi veniam animi, quae tenetur nihil soluta,
        consequuntur rem absum, dolor sit amet consectetur adipisicing elit.
        Molestiae error dolor, excepturi veniam animi, quae tenetur nihil
        soluta, consequuntur rem ab quos libero voluptates. Consequatur
        recusandae unde odio illum hic. quos libero voluptates. Consequatur
        recusandae unde odio illum hic.
      </p>
      <button class="network-cta">Learn More</button>
    </div>
    <!-- Decorative Images -->
    <img
      src="../assets/decorative-imges/network-rectangle.png"
      class="network-rectangle"
    />
    <img src="../assets/decorative-imges/blob2.svg" class="blob2" />
  </div>
</template>
<script>
export default {};
</script>
<style lang="scss" scoped>
.network_wrapper {
  display: flex;
  height: fit-content;
  width: 100%;
  margin: 6em auto;
  flex-direction: row;
  position: relative;
  .network_left {
    width: 55%;
    display: flex;
    align-items: center;
    .network-img {
      width: 100%;
      margin: 0 auto;
      position: relative;
      left: -2em;
    }
  }
  .network_right {
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
    width: 45%;
    margin: auto;
    padding: 1em;
    height: 500px;
    .network-header {
      font-size: 3em;
      color: rgb(58, 86, 83);
      font-weight: bold;
    }
    .network-text {
      width: 75%;
      color: #777;
    }
    .network-cta {
      background-color: rgb(60, 189, 150);
      padding: 0 1.25em;
      border-radius: 8px;
      color: #fff;
      cursor: pointer;
      font-size: 16px;
      height: 2.75em;
      width: 8.5em;
      transition: 0.1s ease-in;
      &:hover {
        background-color: rgb(30, 146, 112);
      }
    }
  }
  /* Decorative Image */
  .network-rectangle {
    position: absolute;
    left: -9.5em;
    height: 100%;
    z-index: -1;
    margin: auto 0;
    opacity: 0.75;
  }
  .blob2 {
    position: absolute;
    top: -30em;
    right: -32em;
    width: 800px;
    opacity: 75%;
  }
}
</style>
