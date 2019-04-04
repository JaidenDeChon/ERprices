<template lang="pug">

	div(class="hero-container")

		h2 Find hospital prices that matter to you. 
		img(src="../assets/undraw_doctor_kw5l.svg")
		p Start by choosing an option below. 


</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'CallToAction'
})
</script>

<style scoped lang="sass">

.hero-container

	box-sizing: border-box
	// border: solid black

	// height: 400px
	width: 80vw

	margin: 40px auto 40px

	color: #ffffff
	text-align: center

	display: flex
	flex-direction: column
	align-items: center
	justify-content: space-around

	img, h2, p

		// width: 33.333%

	img

		display: none

	h2

		font-family: 'Quicksand'
		font-weight: bold

// smartphones, portrait iPhone, portrait 480x320 phones (Android)
// @media (min-width: 280px)

// Higher resolution portrait mobile devices
// @media (min-width: 400px)

// Landscape iPhones
// @media (min-width: 568px)

// Portrait iPad
// @media (min-width: 750px)

// Landscape standard tablets, lo-res laptops and desktops
@media (min-width: 801px)

	.hero-container

		flex-direction: row
		margin: 40px auto -40px

		img

			display: block

			height: auto
			width: 80%

			object-fit: cover

			z-index: 0

		img, h2, p

			width: 33.3%

// For laptops and desktops, and landscape big tablets
// @media (min-width: 1000px)

// Not a standard measurement; just for resizing header
@media (min-width: 1350px)

	.hero-container

		h2

			font-size: 30px

		p

			font-size: 20px

// Full HD laptops & desktops, big tablets
@media (min-width: 1920px)

	.hero-container

		h2

			font-size: 33px

		p

			font-size: 25px

// 4K screens
// @media (min-width: 1400px)

</style>