<script>
export default {
  data() {
    return {
      arr: ['a', 'c', 'd'],
    }
  },
  methods: {
    add: function() {
		  this.arr.push('b');
  },
    delFirst: function() {
      this.arr.shift();
  },
    delLast: function() {
      this.arr.pop();
  },
    delSecondToLast: function() {
      this.arr.splice(-2, 1);
  },
    sortArr: function() {
      this.arr.sort();
  },
    reverseOrder: function() {
      this.arr.reverse();
  }
}
}
</script>
<template>
  <button @click.once="add">Task 1</button>
  <button @click.once="delFirst">Task 2</button>
  <button @click.once="delLast">Task 3</button>
  <button @click.once="delSecondToLast">Task 4</button>
  <button @click.once="sortArr">Task 5</button>
  <button @click.once="reverseOrder">Task 6</button>
  <ul v-for="elem in arr">
    <li>{{ elem }}</li>
  </ul><br>
</template>