<template>
	<div id="app">
		<Sidebar />
		<Header />
		<router-view></router-view>
	</div>
</template>

<script>
import Sidebar from './components/common/Sidebar.vue'
import Header from './components/common/Header.vue'
import '@/assets/scss/_index.scss';

export default {
	components: {
		Sidebar,
		Header,
	}
}
</script>

<style>
* {
	margin: 0;
	padding: 0;
	box-sizing: border-box;
}
html,
body {
	font-size: 14px;
}
#app {
	font-family: Avenir, Helvetica, Arial, sans-serif;
	-webkit-font-smoothing: antialiased;
	-moz-osx-font-smoothing: grayscale;
}
</style>
