<script lang="ts">

type Person = {
  id: number;
  name: string;
  age: number;
};

export default {
  
  props: {
    msg: String,
    data: Array<Person>
  }
}
</script>

<template>
  <h2>{{ msg || 'No props passed yet' }}</h2>
  <ul>
    <li v-for="single of data">
      nome: {{ single.name }} <br> idade: {{ single.age }}

    </li>
  </ul>
</template>