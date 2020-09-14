<template>
  <div class="links-con">
    <a href="https://github.com/DanielKragh" target="_blank" class="text-decoration-none">
      <v-btn fab small text>
        <v-icon size="30px" color="#121212">mdi-github</v-icon>
      </v-btn>
    </a>
    <a href="https://linkedin.com/in/danielklitgaard" target="_blank" class="text-decoration-none">
      <v-btn fab small text>
        <v-icon size="30px" color="#121212">mdi-linkedin</v-icon>
      </v-btn>
    </a>
    <a href="/Daniel_Kragh_Klitgaard_CV.pdf" target="_blank" class="text-decoration-none">
      <v-btn fab small text>
        <v-icon size="30px" color="#121212">mdi-file-account</v-icon>
      </v-btn>
    </a>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.links-con {
  position: fixed;
  top: 50%;
  right: 0;
  transform: translateY(-50%);
  width: 50px;
  height: 200px;
  background-color: #fff;
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  align-items: center;
}
</style>