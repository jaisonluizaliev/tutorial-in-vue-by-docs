<script lang="ts">
import ChildSlot from './ChildSlot.vue'

export default {
  components: {
    ChildSlot
  },
  data() {
    return {
      msg: 'from parent'
    }
  }
}
</script>

<template>
  <div class="classBox">
    <h1>##12 SLOT</h1>

    <ChildSlot>Message: {{ msg }}</ChildSlot>
  </div>
</template>