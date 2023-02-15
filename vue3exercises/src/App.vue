<script>
export default {
  data() {
    return {
    }
  },
  methods: {
    alyarm: function() {
      alert(`This will only be shown once`);
    }
  }
}
</script>
<template>
  <a href.prevent="https://www.youtube.com/watch?v=dQw4w9WgXcQ&ab_channel=RickAstley" target="_blank">Link</a><br>
  <button @click.once="alyarm">Button</button>
</template>