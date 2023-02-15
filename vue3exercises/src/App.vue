<script>
export default {
  data() {
    return {
      visibility: false,
    }
  },
  methods: {
    toggle: function() {
      this.visibility = !this.visibility;
    }
  }
}
</script>
<template>
  <p v-show="visibility">yuken</p><br>
  <button @click="toggle">Toggle</button>
</template>