<script setup lang="ts">
import TrackBarItem from './components/TrackBarItem.vue';
import TitleBar from './components/TitleBar.vue';
</script>

<template>
  <TitleBar />
  <TrackBarItem :value=69 />
  <TrackBarItem :value=21 />
</template>

<style>
*, ::before, ::after {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

body {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  font-family: Avenir, Helvetica, Arial, sans-serif;
}

</style>
