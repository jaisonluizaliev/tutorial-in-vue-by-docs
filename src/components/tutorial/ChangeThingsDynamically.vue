<script lang="ts">
export default {
  data() {
    return {
      titleClass: 'title'
    }
  }
};
</script>

<template>
  <div class="classBox">
    <h1>##03</h1>


    <div class="box-button">

      
      <h1 :class="titleClass">in here has a example of use of directive v-bind: in shorthand is :property-name ((Make me
        red))
        more information is in here
        <a href="https://vuejs.org/tutorial/#step-3" target="_blank"
        rel="noopener noreferrer">https://vuejs.org/tutorial/#step-3</a>
        
        
        
      </h1> <!-- add dynamic class binding here -->
    </div>
  </div>
</template>

<style scoped>
.title {
  color: red;
}
</style>