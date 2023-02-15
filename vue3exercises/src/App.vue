<script>
export default {
  data() {
    return {
      visibility: true,
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
  <div v-if="visibility">
  <p>yuken</p>
  <p>yuken2</p>
  <p>yuken3</p>
  </div><br>
  <button @click="toggle">Toggle</button>
</template>