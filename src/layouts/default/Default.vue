<template>
  <v-app>
    <default-bar />

    <default-view />
  </v-app>
</template>

<script setup>
  import DefaultBar from './AppBar.vue'
  import DefaultView from './View.vue'
</script>

<style>
.cormorant-font {
  font-family: 'Cormorant';
}
/* .japanese-font {
  font-family: 'Noto Serif Japanese';
} */
/* .vibes-font {
  font-family: 'Great Vibes';
} */
</style>
