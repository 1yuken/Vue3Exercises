<script>
  export default {
    data() {
	      return {
                name: 'Omen',
    attr: 'omen.png',
    text: 'page',
		            href: 'page.html',
    num: 5,
    num1: 1,
                num2: 2,
                num3: 3,
    arr1: ['x', 'y', 'z'], 
    arr2: [1, 2, 3], 
    obj: {x: 1, y: 2, z: 3}, 
	      }   
},

methods: { 
 show: function() { 
  alert(today); 
 },
 summ: function() {
  alert(this.num1 + this.num2)
 }
}
}
  let today = new Date(); 
</script>

<template>
  <div>
		<h1> Vue exercises </h1>
	</div>
  <br>
  <img :src="attr">
  <div> <p> I'm {{ name }}</p>
    <p>Solve this task for me <a href="page.html">here</a></p>
    <p class="sc">Квадрат неизвестного num равен {{num*num}}, А сумма num1,num2,num3 равна {{num1+num2+num3}}.</p>
    <p class="sc">Выведем каждую букву массива в отдельном абзаце: <br> {{arr1[0]}} <br> {{arr1[1]}} <br> {{arr1[2]}} <br> Теперь выведем сумму элементов второго массива : {{arr2[0] + arr2[1] + arr2[2]}}</p>
    <p class="sc">Выведем сумму элементов объекта obj : {{obj.x + obj.y + obj.z}} </p>
    <button class="button button1" @click="show">Узнать дату по нажатию</button>
    <button class="button button2" @mouseenter="show"> Узнать дату по наведению</button> 
  </div>
</template>

<style >

header {
  line-height: 1.5;
}
.sc {
  font-size: medium;
 color: #22235c;
}

p {
  line-height: 2.5;
  font-size: large;
  letter-spacing: 2px;
  font-family: 'Montserrat', sans-serif;
  color: #22235c;
}
.logo {
  display: block;
  margin: 0 auto 2rem;
}
@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }
  .logo {
    margin: 0 2rem 0 0;
  }
  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>