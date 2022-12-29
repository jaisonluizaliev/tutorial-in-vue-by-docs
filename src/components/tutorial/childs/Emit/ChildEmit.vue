<script lang="ts">
const umaPropsLocal = "isso"
export default {
  data() {
    return {
      native: umaPropsLocal
    }
  },
  emits: [
    'response'
  ], created() {
      this.$emit('response', umaPropsLocal)
  },
}
</script>

<template>
  <div class="classBox" >
    <h2>Sou o Filho que Vai manda um emit</h2>
    {{ native }}
  </div>
</template>