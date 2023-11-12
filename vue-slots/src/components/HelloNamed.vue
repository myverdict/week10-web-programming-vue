<template>
  <p>
    This class is
    <slot name="subject"></slot>
  </p>

  <p>
    And it is on
    <slot name="day"></slot>
  </p>
</template>

<script>
export default {
  name: 'HelloNamed',
};
</script>
