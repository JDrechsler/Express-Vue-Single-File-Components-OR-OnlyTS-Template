<template>
	<div id="app" class="container-fluid">
		<img src="./assets/logo.png">
		<ManageProducts></ManageProducts>
		<SocketTest></SocketTest>
		<Music></Music>
		<TsTest></TsTest>

	</div>
</template>

<script lang="ts">
	import Vue from 'vue'
	import Component from 'vue-class-component'

	import ManageProducts from './components/ManageProducts.vue'
	import SocketTest from './components/SocketTest.vue'
	import Music from './components/Music.vue'
	import TsTest from './components/TsTestFolder/TsTest.vue'

	@Component({
		components: {
			ManageProducts,
			SocketTest,
			Music,
			TsTest
		}
	})

	export default class App extends Vue {
		msg: string = "I am the parent of all childs!!!"
	}

</script>

<style>
	#app {
		font-family: 'Avenir', Helvetica, Arial, sans-serif;
		-webkit-font-smoothing: antialiased;
		-moz-osx-font-smoothing: grayscale;
		color: #2c3e50;
		background-color: mintcream;
	}

</style>
