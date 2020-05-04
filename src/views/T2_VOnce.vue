<!-- Task 2 - using v-once -->
<template>
  <div>
    <h1 v-once>{{ title }}</h1>
    <h1>{{ asteriodHunter() }}</h1>
    <h4>{{ subtitle }}</h4>
    <div>
      <a v-bind:href="link">Topgolf</a>
    </div>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        title: "Welcome to Nasa",
        subtitle: "Searching for Near-Earth Objects",
        link: "http://topgolf.com"
      }
    },
    methods: {
      asteriodHunter: function() {
        return this.title = "Asteroid Hunter";
      }
    }
  }
</script>

<style scoped>

</style>