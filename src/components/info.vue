<template>
  <div class="info">
      {{ infoText }}
  </div>
</template>

<script>
export default {
  name: "Info",
  props: {
      infoText: {
          type: String,
          default: null,
          required: true
      }
  }
};
</script>

<style scoped lang="scss"></style>
