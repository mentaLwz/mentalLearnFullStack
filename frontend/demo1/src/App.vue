<template>
 <h1>我是傻逼杨银弟</h1>
<h2> {{name}} {{age}}</h2>
<button @click="sayHello">fuck you</button>

</template>



<script>
  import {h} from 'vue'
  export default {
	name: 'App',
	setup() {
	  let name = 'zx'
	  let age = 18

	  // methods
	  function sayHello() {
		alert(`my name is ${name}, my age is ${age}`)
	  }

	  /*return {
		name,
		age,
		sayHello
	  }
	  */
	  return ()=> h('h1', 'Big pig!!!')


	}


  }



</script>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
