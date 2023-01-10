<template lang="">
  <div class="social_proof_wrapper">
    <div class="social-proof-block">
      <img class="social-proof-img" src="../assets/images/airtable_png.png" />
    </div>
    <div class="social-proof-block">
      <img class="social-proof-img" src="../assets/images/sketch_png.png" />
    </div>
    <div class="social-proof-block">
      <img class="social-proof-img" src="../assets/images/dribbble_png.png" />
    </div>
    <div class="social-proof-block">
      <img class="social-proof-img" src="../assets/images/slack_png.png" />
    </div>
    <div class="social-proof-block">
      <img class="social-proof-img" src="../assets/images/livechat_png.png" />
    </div>
    <div class="social-proof-block">
      <img class="social-proof-img" src="../assets/images/gitlab_png.png" />
    </div>
  </div>
</template>
<script>
export default {};
</script>
<style lang="scss">
.social_proof_wrapper {
  background-color: rgb(227, 248, 231);
  width: 100%;
  height: 150px;
  display: flex;
  align-items: center;
  justify-content: space-evenly;
  .social-proof-block {
    height: 115%;
    aspect-ratio: 1;
    display: flex;
    align-items: center;
    .social-proof-img {
      width: 100%;
    }
  }
}

@media screen and (max-width: 1050px) {
  .social-proof-block {
    .social-proof-img {
      width: 75% !important;
    }
  }
}

@media screen and (max-width: 900px) {
  .social_proof_wrapper {
    padding: 0 2em;
    justify-content: flex-start;
    overflow-x: scroll;
    overflow-y: hidden;
    &::-webkit-scrollbar-thumb {
      background: rgb(30, 146, 112);
      border-radius: 8px;
      height: 4px;
      width: 4px;
    }
    &::-webkit-scrollbar {
      background: rgb(214, 213, 213);
      height: 8px;
    }
    &::-webkit-scrollbar-track {
      height: 4px;
    }
  }
}
</style>
