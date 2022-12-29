<script lang="ts">
import Child01 from "./Child01.vue";
import Child02 from "./Child02.vue";


export default {
  data() {
    return {

    }
  },
  components: {
    Child01,
    Child02
  }
}
</script>

<template>
  <div class="classBox">
    <h1>##09 WATCHERS</h1>
    <div class="classBox">
      <Child01 />
    </div>
    <div class="classBox">
      <Child02 />
    </div>
  </div>
</template>