<script>
export default {
  data() {
    return {
      obj: {
        done: true,
        selected: false,
      },
    };
  },
  methods: {},
};
</script>
<template>
  <p :class="obj">yuken</p>
</template>
<style>
.done {
  border: 5px solid red;
}
.selected {
  color: green;
  font-size: 10em;
}
</style>