<template>
  <section class="buttonselector">
    <button class="adwButton">Slides</button>
    <button class="adwButton">Camera</button>
    <button class="adwButton">Slides pip</button>
    <button class="adwButton">Camera pip</button>
  </section>
</template>

<script>
export default {
  name: 'VideoSelector',
  props: {
    msg: String
  },
}
</script>

<style scoped>
section.buttonselector {
  padding: 20px;
  display: flex;
  gap: 20px;
}

button {
  flex: 1 1 0;
}
</style>
