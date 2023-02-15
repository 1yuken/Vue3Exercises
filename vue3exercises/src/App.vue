<script>
export default {
  data() {
    return {
      text: 'valorant',
      data: 'omen',
    }
  },
  methods: {
    changeToType: function() {
      this.text = 'type';
    },
    changeToWrite: function() {
      this.text = 'write';
    }
  }
}
</script>
<template>
  <h1>Vue exercises {{ text }} here</h1><br>
  <button @click="changeToWrite">Change to "write"</button><br>
  <button @click="changeToType">Change to "type"</button> 
</template>