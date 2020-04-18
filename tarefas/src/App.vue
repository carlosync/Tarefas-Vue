<template>
	<div id="app">
		<h1>Tarefas</h1>
    <Taskgrid :tasks="tasks"/>
	</div>
</template>

<script>
import Taskgrid  from "./components/Taskgrid.vue"

export default {
  components : { Taskgrid },
  data (){
    return {
      tasks: [
        { name: "API Rest Spring", pending: false },
        { name: "Aprender VueJS", pending: true },
      ]
    }
  }
}
</script>

<style>
	body {
		font-family: 'Lato', sans-serif;
		background:rgb(58, 96, 115);
		color: #FFF;
	}

	#app {
		display: flex;
		flex: 1;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		height: 100vh;
	}

	#app h1 {
		margin-bottom: 5px;
		font-weight: 300;
		font-size: 3rem;
	}
</style>
