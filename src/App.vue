<template>
	<div id="app">
		<h1>Rotas com VueRouter</h1>
		<Menu />
		<router-view name="menu"/>
		<transition mode="out-in"
			 enter-active-class="animate__animated animate__backInLeft animate_faster" 
			 leave-active-class="animate__animated animate__backOutRight animate_faster">
			<router-view/>
		</transition>
	</div>
</template>

<script>
export default {

}
</script>

<style>
	#app {
		display: flex;
		flex-direction: column;
		align-items: center;
	}
</style>
