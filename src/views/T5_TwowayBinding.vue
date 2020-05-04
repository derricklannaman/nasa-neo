<!-- Task 5 Two-Way Binding- -->
<template>
  <div>
    <h1>{{ title }}, {{ asteriodHunter }}</h1>
    <h4>{{ subtitle }}</h4>

    <input type="text">
    <h4>{{ name }}</h4>

  </div>
</template>

<script>
  export default {
    data() {
      return {
        title: "Welcome to Nasa",
        subtitle: "Searching for Near-Earth Objects",
        asteriodHunter: "Asteroid Hunter",
        name: "Derrick"
      }
    },
    methods: {
    }
  }
</script>

<style scoped>

</style>