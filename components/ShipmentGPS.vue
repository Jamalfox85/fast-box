<template lang="">
  <div class="network_wrapper">
    <div class="network_left">
      <img src="../assets/images/world_map.png" class="network-img" />
    </div>
    <div class="network_right">
      <h2 class="network-header">Follow your shipment via GPS</h2>
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
      src="../assets/decorative-imges/green-star.svg"
      class="gps-green-star"
    />
  </div>
</template>
<script>
export default {};
</script>
<style lang="scss" scoped>
.network_wrapper {
  display: flex;
  flex-direction: row-reverse;
  height: fit-content;
  position: relative;
  .network_left {
    width: 50%;
    .network-img {
      width: 100%;
      margin: 0 auto;
      position: relative;
      left: 4em;
    }
  }
  .network_right {
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
    width: 50%;
    margin: auto;
    padding-left: 10%;
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
  /* Decorative Images */
  .gps-green-star {
    position: absolute;
    width: 4em;
    top: 0;
    left: 12em;
  }
}

@media screen and (max-width: 1100px) {
  .network_wrapper {
    .network_left {
      width: 100%;
      position: absolute;
      z-index: -1;
      opacity: 0.5;
      .network-img {
        left: 0;
        top: 0;
      }
    }
    .network_right {
      width: 100%;
      align-items: center;
      text-align: center;
    }
  }
}
</style>
