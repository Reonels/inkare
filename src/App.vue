<template>
  <v-app>
    <v-main>
      <router-view />
    </v-main>
  </v-app>
</template>

<script>
export default {
  name: 'App',

  data: () => ({
    //
  }),
};
</script>

<style>
@font-face{
  font-family: Roboto;
  src: url(../src/font/Roboto/Roboto-Regular.ttf);
  font-style: normal;
  font-weight: normal;
}
</style>
