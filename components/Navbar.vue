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
export default {
  data() {
    return {
      menuOpen: true,
    };
  },
  methods: {
    toggleMobileMenu() {
      this.menuOpen = !this.menuOpen;
    },
  },
};
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
  .mobile-menu {
    display: none;
    cursor: pointer;
    background-color: rgb(60, 189, 150);
    img {
      width: 1.5em;
    }
    .mobile-main {
      top: 0;
      right: 0;
      height: 100vh;
      padding: 2em 4em;
      display: none;
      .mobile-open-icon {
        z-index: 4;
        width: 1.5em;
        position: absolute;
        top: 25px;
        right: 25px;
      }
      .mobile-nav-links {
        height: 50%;
        display: flex;
        flex-direction: column;
        justify-content: space-evenly;
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

@media screen and (max-width: 1000px) {
  .nav_wrapper {
    flex-wrap: wrap;

    .nav_logo {
      width: 50%;
      order: 1;
    }
    .nav_links {
      justify-content: space-between !important;
      width: 100%;
      order: 3;
    }
    .nav_ctas {
      justify-content: flex-end;
      width: 50%;
      order: 2;
    }
  }
}
</style>
