<script>
export default {
  data() {
    return {
      age: "Vue3 exercises",
    }
  },
  methods: {
  }
}
</script>
<template>
  <h3>Enter age: </h3><br>
  <input type="number" v-model.number="age">
  <p v-if="age < 18">Подросток</p>
  <p v-else-if="age < 25">Молодой человек</p>
  <p v-else-if="age >= 25">Мужчина</p>
</template>