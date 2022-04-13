<script setup lang="ts">
defineProps<{ value: number }>();
</script>

<template>
  <div id="track-bar">
    <input class="slider" type="range" v-model="value" min="0" max="100" />
  </div>
</template>

<style lang="scss" scoped>
#track-bar {
  display: flex;
  align-items: center;
  justify-content: center;
  height: 200px;
  width: 175px;
  position: relative;
}

@mixin trackThumb {
  width: 25px;
  height: 25px;
  background: #04aa6d;
  border-radius: 50%;
  cursor: pointer;
  transform: scale(1.85);
}

.slider {
  --thumb-hover: #05c982;
  -webkit-appearance: none;
  background: #d3d3d3;
  outline: none;
  transform: rotateZ(270deg);
  width: 100%;
  overflow: visible;
  border-radius: 3rem;

  &::-webkit-slider-thumb {
    -webkit-appearance: none;
    appearance: none;
    @include trackThumb;

    &:hover {
      background-color: var(--thumb-hover);
    }
  }

  &::-moz-range-thumb {
    @include trackThumb;

    &:hover {
      background-color: var(--thumb-hover);
    }
  }
}
</style>