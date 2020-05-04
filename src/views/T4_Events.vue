<!-- Task 4 - Events -->
<template>
  <div>
    <h1 v-once>{{ title }}</h1>
    <h1>{{ asteriodHunter() }}</h1>
    <h4>{{ subtitle }}</h4>
    <div>
      <!-- Step 1 Click to increase -->
      <!-- v-on:click="increase" -->
      <!-- v-on:click="increase(2, $event)" -->
      <button class="btn btn-success" v-on:click="increase">Click Me</button>
      <h3>{{ counter }}</h3>
    </div>
      <hr>

      <!-- step 2 MouseCoordinates -->
      <!-- v-on:mousemove="updateCoordinates" -->
    <div v-on:mousemove="updateCoordinates">
      <h3> Coordinates: {{ x }} / {{ y }}</h3>
    </div>


  </div>
</template>

<script>
  export default {
    data() {
      return {
        title: "Welcome to Nasa",
        subtitle: "Searching for Near-Earth Objects",
        link: "http://topgolf.com",
        finishedLink: '<a href="http://google.com">Google</a>',
        counter: 0,
        x: 0,
        y: 0
      }
    },
    methods: {
      asteriodHunter: function() {
        return this.title = "Asteroid Hunter";
      },
      increase: function() {
        // num, event
        return this.counter++;
      },
      updateCoordinates: function(event) {
        this.x = event.clientX;
        this.y = event.clientY;
      }
    }
  }
</script>

<style scoped>

</style>