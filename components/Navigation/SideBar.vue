<template>
  <div>
    <div class="logo-con">
      <nuxt-link to="/" ><span class="logo-con__letter">D</span></nuxt-link>
    </div>
    <div class="scroll-con">
      <div class="scroll-con__bar"></div>
      <div class="scroll-con__bar-filler"></div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      scrollLenght: 0
    };
  },
  methods: {
    scroll() {}
  },
  mounted() {}
};
</script>

<style lang="scss" scoped>
.logo-con {
  text-align: center;
  margin-top: 30px;
  margin-bottom: 50px;
  &__letter {
    font-size: 30px;
    font-weight: bold;
    text-decoration: none;
    color: #fff;
  }
}
.scroll-con {
  padding-left: 50%;    
  position: relative;
  &__bar {

    background-color: #fff;
    opacity: 0.3;
    width: 1px;
    height: 70vh;
    transform: translateX(50%);
  }
  &__bar-filler {
    position: absolute;
    top: 0;
    background-color: #fff;
    width: 1px;
    height: 100px;
  }
}
</style>