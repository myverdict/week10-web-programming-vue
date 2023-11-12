<template>
  <h1>{{ msg }}</h1>
  <!--
    Text from inside the HelloWorld component element in the parent App.vue is rendered inside the slot element below.
  -->
  <slot></slot>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String,
  },
};
</script>
