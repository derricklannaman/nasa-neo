<!-- Task 1 - Binding to attributes -->
<template>
  <div>
    <h1>{{ title }}</h1>
    <h1>Asteroid Hunter</h1>
    <h4>{{ subtitle }}</h4>
    <div>
      <!-- <a href="{{ link }}">Topgolf</a> -->
    </div>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        title: "",
        subtitle: "Searching for Near-Earth Objects",
        link: "http://topgolf.com"
      }
    },
    // methods: {
    //   asteriodHunter: function() {
    //     return this.title = "Asteroid Hunter";
    //   }
    // }
  }
</script>

<style scoped>

</style>