<template>
  <button>
    {{ text }}
  </button>
</template>

<script>
export default {
  name: "base-button",
  props: {
    text: String,
    disabled: Boolean,
  }
}
</script>

<style scoped>
</style>