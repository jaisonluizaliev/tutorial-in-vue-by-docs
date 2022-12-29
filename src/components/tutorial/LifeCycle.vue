<script lang="ts">
import * as runtimeCore from '@vue/runtime-core'



declare module '@vue/runtime-core' {

  interface ComponentCustomProperties {
    $refs: {
      [key: string]: HTMLElement | any,
    },
    // ... more stuff  

  }
}

export default {

  mounted() {

    setTimeout(() => {
      this.$refs.p.textContent = "oi",
      this.$refs.h3.textContent = "serei o que eu quiser"
    }, 1000)


    setTimeout(() => {
      this.$refs.p.textContent = "tchau",
        this.$refs.h3.textContent = "serei o não"
    }, 2000)

  },
}

  // ..
</script>

<template>
  <div class="classBox">
    <h1>##08 LIFECYCLE</h1>

    <p ref="p">hello</p>


    <h3 ref="h3">serei outra coisa</h3>
  </div>
</template>