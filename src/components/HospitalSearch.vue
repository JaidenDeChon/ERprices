<template>
	<div class="material-shadow hospital-search">

		<div class="header">
			<p>Choose an option...</p>
			<button class="blue-hover">	
				<i class="fas fa-question"></i>
			</button>
		</div>

		<div class="options-container">

			<button class="option blue-hover">
				<img src="../assets/undraw_directions_x53j.svg"></img>
				<p>Detect my location</p>
			</button>

			<button class="option blue-hover">
				<img src="../assets/undraw_navigation_lytx.svg">
				<p>Enter my zipcode</p>
			</button>
		</div>

	</div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'HospitalSearch'
})
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="sass">

$gradient-blue-1: #0575E6
$gradient-blue-2: #021B79

$gradient-orange-1: #ff9966
$gradient-orange-2: #ff5e62

html, body
	margin: 0
	padding: 0

// Reset for mobile browsers
h1, h2, h3, h4, h5, h6
	font-weight: normal

.blue-hover

	color: #555
	font-size: 15px

	background: #e8e8e8

	cursor: pointer
	transition: all .2s ease
	border: none

	&:hover

		background: $gradient-orange-2
		box-shadow: 0 8px 60px rgba(255, 94, 98, 0.5), 0 6px 25px rgba(255, 94, 98, 0.5)
		color: #ffffff

.header

	text-align: center
	// font-size: 15px

	display: flex
	flex-direction: row
	align-items: center
	justify-content: center

	position: relative

	.blue-hover

		padding: 8px 12px

		position: absolute
		right: 0

		font-size: 13px

		box-sizing: border-box
		border-radius: 10px

.options-container

	display: flex
	flex-direction: column
	align-items: center

	.option

		// background: url("../assets/undraw_doctor_kw5l.svg")

		font-family: 'IBM Plex Sans'
		font-weight: 400

		width: 75%
		height: 200px

		margin: 10px 0

		border-radius: 20px

		display: flex
		align-items: center
		justify-content: center
		flex-direction: column

		img

			height: 120px
			width: 120px

			margin: 0
			padding: 0

			object-fit: fit

			// background-color: #ffffff

		.numbers

			font-family: 'Quicksand'

// smartphones, portrait iPhone, portrait 480x320 phones (Android)
// @media (min-width: 280px)

// Higher resolution portrait mobile devices
// @media (min-width: 400px)

// Landscape iPhones
@media (min-width: 568px)

	.options-container

		flex-direction: row
		justify-content: space-around

		.option

			width: 45%
			min-height: 300px

			img

				min-height: 160px
				min-width: 160px

// Portrait iPad
@media (min-width: 750px)

	.options-container

		.option

			// min-height: 200px

			img

				min-height: 160px
				min-width: 160px

// Landscape standard tablets, lo-res laptops and desktops
@media (min-width: 801px)

	.options-container

			.option

				min-height: 300px

// For laptops and desktops, and landscape big tablets
@media (min-width: 1000px)

	.options-container

		.option

			min-height: 400px

			font-size: 20px

			img

				min-width: 200px
				min-height: 250px

// Full HD laptops & desktops, big tablets
// @media (min-width: 1920px)

// 4K screens
// @media (min-width: 1400px)

</style>
