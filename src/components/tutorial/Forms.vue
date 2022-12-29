<script lang="ts">
export default {
  data() {
    return {
      text: ''
    }
  },
  methods: {
    clearAll() {
      this.text = ''
    }
  }
}
</script>

<template >
  <div class="classBox">
    
    <h1>##05 FORMS</h1>
    <div class="box-button">

    </div>

    <div class="box-button">

      <p style="font-size: 1.8rem;">{{ text }}</p>
    </div>


    <div class="box-button">

      <input v-model="text" placeholder="oi" />
    </div>

    <div class="box-button">

      <button class="button-85" type="button" @click="clearAll">limpar</button>
    </div>



  </div>
  <!-- <input :value="text" @input="onInput" placeholder="Type here"> -->
</template>