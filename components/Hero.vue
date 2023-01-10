<template lang="">
  <div class="hero_wrapper">
    <div class="hero-left">
      <h1 class="hero-main-text">
        Largest and most reliable courier service in your city
      </h1>
      <p class="hero-sec-text">
        Lorem ipsum, dolor sit amet consectetur adipisicing elit. Maxime et
        adipisci quia delectus, tenetur quod possimus optio corporis nam.
      </p>
      <div class="tracking-input-group">
        <input
          type="text"
          id="tracking-number-input"
          name="tracking-number-input"
          aria-label="tracking-number-input"
          class="tracking-input"
          placeholder="Enter Tracking Number"
        />
        <button class="check-tracking-bttn">Check</button>
      </div>
    </div>
    <div class="hero-right">
      <a
        class="img-attr"
        href="https://www.freevector.com/man-riding-bicycle-30077#"
        >FreeVector.com</a
      >
      <img src="../assets/images/hero-img.svg" class="hero-img" />
    </div>
    <!-- Decorative Images -->
    <img src="../assets/decorative-imges/gold-star.svg" class="gold-star" />
    <img src="../assets/decorative-imges/green-star.svg" class="green-star" />
    <img src="../assets/decorative-imges/hero-globe.png" class="hero-globe" />
  </div>
</template>
<script>
export default {};
</script>
<style lang="scss">
// .register-bttn {
//   background-color: rgb(60, 189, 150);
//   padding: 0 1.25em;
//   border-radius: 8px;
//   color: #fff;
//   cursor: pointer;
//   transition: 0.1s ease-in;
//   &:hover {
//     background-color: rgb(30, 146, 112);
//   }
// }
.hero_wrapper {
  display: flex;
  align-items: center;
  min-height: 700px;
  width: 90%;
  margin: 0 auto;
  position: relative;
  .hero-left {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    width: 60%;
    .hero-main-text {
      font-size: 5em;
      line-height: 1.25em;
      width: 100%;
      padding: 0;
      font-weight: bold;
    }
    .hero-sec-text {
      color: #777;
      width: 65%;
      margin: 2em 0;
    }
    .tracking-input-group {
      padding: 0;
      height: 3em;
      display: flex;
      align-items: center;
      background-color: rgb(226, 245, 239);
      border-radius: 8px;
      .tracking-input {
        height: 100%;
        margin: 0;
        padding: 0 2em;
        font-size: 0.75em;
        width: 300px;
        background-color: rgb(226, 245, 239);
        border-radius: 8px 0 0 8px;
        &:focus {
          outline: solid 2px rgb(60, 189, 150);
        }
      }
      .check-tracking-bttn {
        background-color: rgb(60, 189, 150);
        padding: 0 1.25em;
        border-radius: 8px;
        color: #fff;
        height: 100%;
        margin: 0;
      }
    }
  }
  .hero-right {
    display: flex;
    justify-content: center;
    width: 50%;

    .img-attr {
      display: none;
    }
    .hero-img {
      position: absolute;
      width: 75%;
      top: 8em;
      right: -12em;
      z-index: -1;
    }
  }
  /* Decorative Images */
  .gold-star {
    position: absolute;
    width: 3em;
    left: 40%;
    top: 3em;
  }
  .green-star {
    position: absolute;
    width: 4em;
    left: 50%;
  }
  .hero-globe {
    position: absolute;
    top: -12em;
    right: -8em;
    opacity: 0.5;
    z-index: -2;
    width: 50vw;
  }
}

@media screen and (max-width: 1200px) {
  .hero_wrapper {
    flex-direction: column;
    .hero-left {
      width: 100%;
      position: relative;
      z-index: 2;
      margin-bottom: 2em;
      align-items: center;
      text-align: center;
      .tracking-input-group {
        .tracking-input {
          width: 70vw;
        }
      }
    }
    .hero-right {
      width: 100%;
      .hero-img {
        position: relative;
        width: 100%;
        top: 0;
        right: 0;
      }
    }
  }
  .hero-globe {
    display: none;
  }
}

@media screen and (max-width: 600px) {
  .hero_wrapper {
    .hero-left {
      .hero-main-text {
        font-size: 3em;
      }
    }
  }
}
</style>
