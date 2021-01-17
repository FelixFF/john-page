<template>
  <div class="home">
    <info :infoText="'Test message'"></info>
  </div>
</template>

<script>
import Info from "@/components/info.vue"

export default {
  name: "Home",
  components: {
    Info
  }
};
</script>
<style scoped lang="scss">
</style>
