<template>
  <v-app dark>
    <Links/>
    <v-container fluid>
      <v-row no-gutters>
        <v-col cols="1">
          <SideBar />
        </v-col>
        <v-col cols="11">
          <v-main>
            <v-container>
              <nuxt />
            </v-container>
          </v-main>
        </v-col>
      </v-row>
    </v-container>
  </v-app>
</template>

<script>
export default {
  data() {
    return {};
  }
};
</script>
