<template>
  <div class="mb-3">
    <img @click="$emit('input', !value)" width="50" height="50" :class="{ active: value }" src="../assets/light.jpg" />
  </div>
</template>

<script>
export default {
  props: ['value']
}
</script>

<style scoped>
  img {
    filter: grayscale(100%);
  }
  .active {
    filter: grayscale(0%);
  }
</style>
