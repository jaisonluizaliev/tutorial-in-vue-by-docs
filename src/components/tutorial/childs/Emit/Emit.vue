<script lang="ts">
import ChildEmit from "./ChildEmit.vue"

export default {
  components: {
    ChildEmit
  },
  data() {
    return {
      childMsg: 'No child msg yet'
    }
  }
}


</script>

<template>
  <div class="classBox">
    <h1>##11 EMIT</h1>
    <ChildEmit @response="(msg) => childMsg = msg" />
    <p>{{ childMsg }}</p>

  </div>
</template>