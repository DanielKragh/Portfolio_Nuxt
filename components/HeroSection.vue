<template>
  <header class="hero">
    <div class="hero__heading">
      <h1>
        HEJ, MIT NAVN ER DANIEL KLTGAARD.
        <br />JEG ER WEBUDVIKLER.
      </h1>
    </div>
  </header>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.hero {
  height: 100vh;
  position: relative;
  &__heading {
    position: absolute;
    top: 60%;
    left: 10%;
  }
}
</style>