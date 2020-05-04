<template>
  <div id="app">
    <Neo />
  </div>
</template>

<script>
// import Neo from '@/views/T1_BindingAttributes.vue';
// import Neo from '@/views/T2_VOnce.vue';
// import Neo from '@/views/T3_VHtml.vue';
// import Neo from '@/views/T4_Events.vue';
// import Neo from '@/views/T5_TwowayBinding.vue';
import Neo from '@/views/T6_ComputedProperty.vue';
export default {
  name: 'app',
  components: {
    Neo
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
