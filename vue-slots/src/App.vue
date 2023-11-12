<template>
  <!--
    The text inside the HelloWorld component tags will be passed to the HelloWorld component and rendered in a slot.
  -->
  <HelloWorld msg="Welcome to your VueJS app">
    <img src="./assets/hello.png" alt="Hello icon" />
    <p>Hello, ITEC 2650 Students!</p>
  </HelloWorld>

  <HelloNamed>
    <template v-slot:subject>Web Programming</template>
    <template v-slot:day>Thursday</template>
  </HelloNamed>
</template>

<script>
import HelloNamed from './components/HelloNamed.vue';
import HelloWorld from './components/HelloWorld.vue';

export default {
  name: 'App',
  components: {
    HelloWorld,
    HelloNamed,
  },
};
</script>

<style scoped></style>
