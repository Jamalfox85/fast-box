<template lang="">
  <div class="nav_wrapper">
    <div class="nav_logo">
      <img src="../assets/icons/box-green.svg" />
      FAST BOX
    </div>
    <nav class="nav_links">
      <p class="nav-link active">Home</p>
      <p class="nav-link">Tracking</p>
      <p class="nav-link">Shipping</p>
      <p class="nav-link">Locations</p>
      <p class="nav-link">Shipping</p>
    </nav>
    <div class="nav_ctas">
      <p class="nav-link">Signin</p>
      <button class="register-bttn">Register</button>
    </div>
    <!-- Decorative Elements -->
    <img src="../assets/decorative-imges/nav-blob.svg" class="nav-blob" />
  </div>
</template>
<script>
export default {};
</script>
<style lang="scss">
.nav_wrapper {
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 90%;
  margin: 0 auto;
  .nav_logo {
    font-weight: bold;
    font-size: 1.5em;
    img {
      width: 2em;
      margin-right: 0.5em;
    }
  }
  & > * {
    display: flex;
    .nav-link {
      margin: 0 1.25em;
      color: #777;
      &.active {
        font-weight: bold;
        color: #000;
      }
    }
    .register-bttn {
      background-color: rgb(60, 189, 150);
      padding: 0 1.25em;
      border-radius: 8px;
      color: #fff;
      cursor: pointer;
      transition: 0.1s ease-in;
      &:hover {
        background-color: rgb(30, 146, 112);
      }
    }
  }

  /* Decorative Images */
  .nav-blob {
    width: 25%;
    position: absolute;
    top: -22em;
    left: 2em;
    transform: rotate(290deg) scale(2);
    z-index: -1;
  }
}
</style>
