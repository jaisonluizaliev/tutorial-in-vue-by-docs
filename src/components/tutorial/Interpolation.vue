<script lang="ts">

import Child1Vue from './childs/Child.vue';
export default {
  data() {
    return {
      one: 1
    }
  },

  components: { Child1Vue }

};
</script>

  
<template>
  <div class="classBox">
    <h1>##01</h1>

    <h1>
      meu hello world oi estou iniciando em vue
    </h1>
    <Child1Vue />
  </div>
</template>

