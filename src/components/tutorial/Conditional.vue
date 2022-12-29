<script lang="ts">
export default {
  data() {
    return {
      desapear: true
    }
  },
  methods: {
    desapearBtn() {
      this.desapear = !this.desapear
    }
  },
}
</script>

<template>
  <div class="classBox">

    <h1>##06</h1>


    <div class="box-button">
      <p v-if="desapear">desapear on tap button</p>
      <p v-else="desapear">sumiu</p>

    </div>

    
    <div class="box-button">

      <button class="button-85"  @click="desapearBtn">toggle</button>
    </div>




  </div>

</template>