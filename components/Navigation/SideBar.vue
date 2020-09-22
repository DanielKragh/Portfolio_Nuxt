<template>
  <div>
    <div class="logo-con">
      <nuxt-link to="/">
        <span class="logo-con__letter">D</span>
      </nuxt-link>
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
    handleScroll() {
      let scrollPercentage =
        (document.documentElement.scrollTop + document.body.scrollTop) /
        (document.documentElement.scrollHeight -
          document.documentElement.clientHeight) * 100;

      window.console.log(scrollPercentage);

      let sidebar = document.querySelector(".scroll-con__bar-filler");
      // window.console.log(sidebar);
      sidebar.style.height = scrollPercentage + '%';

    }
  },
  mounted() {
    this.$nextTick(() => {
       window.addEventListener("scroll", this.handleScroll);
    });
  }
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
  }
}
</style>