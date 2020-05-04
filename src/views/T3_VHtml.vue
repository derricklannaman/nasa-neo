<!-- Task 3 - v-html -->
<template>
  <div>
    <h1 v-once>{{ title }}</h1>
    <h1>{{ asteriodHunter() }}</h1>
    <h4>{{ subtitle }}</h4>
    <div>
      <a v-bind:href="link">Topgolf</a>
    </div>
    <hr>
    <!-- v-html -->
    <div>{{ finishedLink }}</div>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        title: "Welcome to Nasa",
        subtitle: "Searching for Near-Earth Objects",
        link: "http://topgolf.com",
        finishedLink: '<a href="http://google.com">Google</a>'
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