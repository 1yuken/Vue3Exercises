<script>
export default{
data(){
  return{
    newItem: '',
    items: ['text', 'emran', 'down', 'text', 'text'],
  }
},
methods: {
  removeItem: function (index) {
    this.items.splice(index, 1);
  }
}
}
</script>

<template>
<ul class="styled">
  <li v-for="(item, index) in 
			items" :key="index">
    {{ item }}
    <br>
    <button class="button" @click="removeItem(index)">remove</button>
  </li>
</ul>
</template>

<style scoped>
</style>