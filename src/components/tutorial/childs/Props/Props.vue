<script lang="ts">
import ChildProps from './ChildProps.vue';
export default {
  data() {
    return {
      greeting: 'Hello from parent',
      data: [{ id: 1, name: "jaison", age: 28 }, {id: 2, name: "juraci", age: 28}]
    }
  },
  components: { ChildProps }

}
</script>

<template>
  <div class="classBox">
    <h1>##10 PROPS</h1>
    <ChildProps :msg="greeting" :data="data"/>
  </div>
</template>