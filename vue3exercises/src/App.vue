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
	      }   
}
  }
</script>

<template>
  <div>
		<h1> Vue exercises </h1>
	</div>
  <br>
  <br>
  <br>
  <br>
  <img :src="attr">
  <div> <p> My name is {{ name }}</p>
    <p>Solve this problem <a href="page.html">here</a></p>
    <p class="sc">Квадрат неизвестного num равен {{num*num}}, А сумма num1,num2,num3 равна {{num1+num2+num3}}.</p>
    <p class="sc"> Выведем каждую букву массива в отдельном абзаце: <br> {{arr1[0]}} <br> {{arr1[1]}} <br> {{arr1[2]}} <br> Теперь выведем сумму элементов второго массива : {{arr2[0] + arr2[1] + arr2[2]}}</p>
  </div>
</template>

<style >
header {
  line-height: 1.5;
}


p {
  line-height: 2.5;
  font-size: large;
  letter-spacing: 2px;
  font-family: 'Montserrat', sans-serif;
  color: rgb(34, 35, 92);
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