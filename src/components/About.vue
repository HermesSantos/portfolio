<script setup lang="ts">
</script>

<template>
  <div class="about-main">
    <h1>Hermes Santos</h1>
    <div class="text-about">
      Passionate developer with a knack for solving complex problems through code. Mostly self-taught and driven by an unyielding curiosity to explore and master new technologies.
    </div>
  </div>
</template>
<style lang="scss" scoped>
.about-main{
  h1{
    font-size: 3rem;
    background: linear-gradient(
      to right,
      #7953cd 20%,
      #00affa 30%,
      #0190cd 70%,
      #764ada 80%
      );
    -webkit-background-clip: text;
    background-clip: text;
    -webkit-text-fill-color: transparent;
    text-fill-color: transparent;
    background-size: 500% auto;
    animation: textShine 5s ease-in-out infinite alternate;
  }
  text-align: center;
  padding: 6rem 25rem;
  .text-about {
    font-size: 1rem;
    margin-top: 2rem;
  }
  @keyframes textShine {
  0% {
    background-position: 0% 50%;
  }
  100% {
    background-position: 100% 50%;
  }
  }
}
</style>
