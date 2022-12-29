<script lang="ts">
export default {
  data() {
    return {
      count: 0,
    }
  },
  methods: {
    incrementThisInOne() {
      this.count++;
    },
    clear() {
      this.count = 0;
    }
  }
}
</script>

<template>
  <div class="classBox">
    <h1>##04 INCREMENT</h1>


    <div class="box-button">

      <h1>
        {{ count }}
      </h1> 
    </div>
    <div class="box-button">

      <button class="button-85" @click="incrementThisInOne">Increment</button>
    </div>

    <div class="box-button">

      <button class="button-85" @click="clear">clear</button>
    </div>


  </div>
  <!-- make this button work -->
</template>