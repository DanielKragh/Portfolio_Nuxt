<template>
  <v-app dark>
    <Links/>
    <v-container fluid>
      <v-row no-gutters>
        <v-col cols="1" class="p-fixed">
          <SideBar />
        </v-col>
        <v-col cols="10" offset="1">
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
