<template>
  <div>
    <button class="btn btn-success" v-on:click="counter++">Increase</button>
    <button class="btn btn-danger" v-on:click="counter--">Decrease</button>
    <button class="btn btn-info" v-on:click="secondCounter++">Increase Second Counter</button>
    <p>Counter: {{ counter }} | {{ secondCounter }}</p>
    <p>Result: {{ result() | output }}</p>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        counter: 0,
        secondCounter: 0
      }
    },
    computed: {
      output: function() {
        console.log("INSIDE output");
        return this.counter > 5 ? "Greater than 5" : "Less than 5";
      }
    },
    methods: {
      result: function() {
        console.log("INSIDE result");
        return this.counter > 5 ? "Greater than 5" : "Less than 5";
      }
    }
  }
</script>

<style scoped>

</style>