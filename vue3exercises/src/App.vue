<script>
export default {
  data() {
    return {
      selected: "Выберите город",
    };
  },
  methods: {},
};
</script>
<template>
  <select v-model="selected">
    <option>Сады Хана Алана</option>
    <option>Центрум</option>
    <option>Старый Крым</option>
    <option>Симферополь</option>
    <option>Кипу</option>
    <option>Ускут</option>
  </select>
  &nbsp;
  <p>{{ selected }}</p>
</template>