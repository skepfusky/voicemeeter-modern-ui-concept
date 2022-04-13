<script setup lang="ts">
import HelloWorld from './components/HelloWorld.vue'
import TrackBarItem from './components/TrackBarItem.vue';
</script>

<template>
  <HelloWorld msg="Hello Vue 3 + TypeScript + Vite" />
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
