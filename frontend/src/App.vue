<template>
  <div id="app">
    <HelloWorld message="Hello World! from App.vue" />
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue';

export default {
  name: 'App',
  components: {
    HelloWorld,
  },
};
</script>
