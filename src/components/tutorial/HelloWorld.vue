<script lang="ts">
import Interpolation from './Interpolation.vue';
import Child1Vue from './childs/Child.vue';


export default {
    data() {
        return {
            name: "jaison",
            dynamic: "this will be displayed in screen dynamicatly"
        };
    },
    components: { Interpolation, Child1Vue }
};
</script>

<template>
  <div class="classBox">
    <!-- <Interpolation />
    <Child1Vue /> -->
    <h1>##02</h1>
    <h1>
      meu hello world oi estou iniciando em vue {{ name }} <br> {{ dynamic }}
    </h1>
  </div>
</template>

