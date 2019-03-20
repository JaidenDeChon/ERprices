<template>
	<div class="hero-container">
		<img src="../assets/undraw_doctor_kw5l .svg">
	</div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'CallToAction'
})
</script>

<style scoped lang="sass">

.hero-container

	height: 400px
	// border: solid white

	margin: 40px 0 -40px 0

	display: flex
	flex-direction: row
	align-items: flex-end
	justify-content: space-around

	img

		height: 400px
		width: 400px

		object-fit: cover

		z-index: 0

		// border: solid white
		// border-radius: 175px

</style>