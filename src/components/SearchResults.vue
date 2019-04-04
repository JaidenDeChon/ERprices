<template lang="pug">

	div(class="parent")

		div(class="container")

			div(class="hover-container")
				div(class="card")
					div(class="title-cont")
						p Diagnostic X-Ray (Chest)
					div(class="info-cont")
						div
							i(class="fas fa-dollar-sign")
							p $314
						div
							i(class="fas fa-h-square")
							p Fort Walton Beach Medical Center
						div
							i(class="fas fa-phone")
							a(href="tel:850-678-4131") 850-678-4131
						div
							i(class="fas fa-map-marker-alt")
							p 1000 Mar-Walt Dr., Fort Walton Beach FL
					button 
						p More information
						i(class="fas fa-angle-right")

			div(class="hover-container")
				div(class="card")
					div(class="title-cont")
						p Mammography Routine Screening
					div(class="info-cont")
						div
							i(class="fas fa-dollar-sign")
							p $120
						div
							i(class="fas fa-h-square")
							p Twin Cities Hospital
						div
							i(class="fas fa-phone")
							a(href="tel:850-862-1111") 850-862-1111
						div
							i(class="fas fa-map-marker-alt")
							p   2190 Florida 85, Niceville FL
					button 
						p More information
						i(class="fas fa-angle-right")

			div(class="hover-container")
				div(class="card")
					div(class="title-cont")
						p Anti-Inflammatory Lumbar Injection
					div(class="info-cont")
						div
							i(class="fas fa-dollar-sign")
							p $829
						div
							i(class="fas fa-h-square")
							p Twin Cities Hospital
						div
							i(class="fas fa-phone")
							a(href="tel:850-862-1111") 850-862-1111
						div
							i(class="fas fa-map-marker-alt")
							p   2190 Florida 85, Niceville FL
					button 
						p More information
						i(class="fas fa-angle-right")

			div(class="hover-container")
				div(class="card")
					div(class="title-cont")
						p Pneumonia
					div(class="info-cont")
						div
							i(class="fas fa-dollar-sign")
							p $22,427
						div
							i(class="fas fa-h-square")
							p Fort Walton Beach Medical Center
						div
							i(class="fas fa-phone")
							a(href="tel:850-678-4131") 850-678-4131
						div
							i(class="fas fa-map-marker-alt")
							p   1000 Mar-Walt Dr., Fort Walton Beach FL
					button 
						p More information
						i(class="fas fa-angle-right")

			div(class="hover-container")
				div(class="card")
					div(class="title-cont")
						p Chest Pain
					div(class="info-cont")
						div
							i(class="fas fa-dollar-sign")
							p $15,785
						div
							i(class="fas fa-h-square")
							p Twin Cities Hospital
						div
							i(class="fas fa-phone")
							a(href="tel:850-862-1111") 850-862-1111
						div
							i(class="fas fa-map-marker-alt")
							p   2190 Florida 85, Niceville FL
					button 
						p More information
						i(class="fas fa-angle-right")

</template>

<script lang="ts">
	import Vue from 'vue'

	export default Vue.extend({
	  name: 'SearchResults'
	})
</script>

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

	.container

		box-sizing: border-box
		// border: solid white

		height: 600px
		width: 100vw

		margin: 0 auto
		padding-left: 10vw

		display: flex
		align-items: center
		flex-wrap: nowrap
		overflow-x: auto

		-webkit-overflow-scrolling: touch

		&::-webkit-scrollbar
			display: none

		.hover-container

			height: 500px
			width: 80%
			margin: 0 15px 0 0
			padding: 20px 0 20px 0

			flex: 0 0 auto

			&:last-child

				border-right: 10vw solid transparent

			&:hover

				.card

					box-shadow: 0 40px 40px rgba(0,0,0,.16)
					transform: translate(0, -20px)

					.title-cont, button

						background: $gradient-orange-2
						color: #ffffff

			.card

				box-sizing: border-box
				border-radius: 22px

				width: 100%
				height: 100%

				font-family: 'IBM Plex Sans'

				background: #ffffff
				box-shadow: 0 20px 20px rgba(0,0,0,.08)
				transition: all 250ms cubic-bezier(.02, .01, .47, 1)

				display: flex
				flex-direction: column

				div

					box-sizing: border-box
					// border: 2px solid red

					width: 100%

					padding: 20px

				.title-cont

					height: 30%
					border-radius: 22px 22px 0 0
					background: #e8e8e8

					font-family: 'Quicksand'
					color: #666
					font-size: 30px
					text-align: center

					display: flex
					align-items: center
					justify-content: center

				.info-cont

					margin: 0
					padding: 0

					height: 55%
					font-family: 'IBM Plex Sans'

					display: flex
					flex-direction: column
					justify-content: space-around

					div

						font-family: 'IBM Plex Sans'
						color: $gradient-blue-2

						margin: 0

						height: 25%
						width: 100%

						display: flex
						flex-direction: row
						align-items: center
						justify-content: space-between
						text-align: center

						i

							margin: 0 10px
							font-size: 18px
							color: $gradient-blue-1

						a

							color: inherit

						p

							text-align: right

				button

					height: 15%
					width: 100%

					border-radius: 0 0 22px 22px
					border: none

					background: #e8e8e8

					font-family: 'Quicksand'
					color: #666
					font-size: 20px
					font-weight: bold

					display: flex
					flex-direction: row
					align-items: center
					justify-content: center

					cursor: pointer

					transition: background 250ms cubic-bezier(.02, .01, .47, 1)

					i, p

						margin: 0 10px

					&:hover

						background: $gradient-orange-1

					// Reset for focus outline
					&:focus
						outline: none
						box-shadow: inset 0px 0px 3px blue

	// smartphones, portrait iPhone, portrait 480x320 phones (Android)
	// @media (min-width: 280px)

	// Higher resolution portrait mobile devices
	// @media (min-width: 400px)

	// Landscape iPhones
	@media (min-width: 568px)

		.parent
			.container
				.hover-container
					width: 400px

	// Portrait iPad
	// @media (min-width: 750px)

	// Landscape standard tablets, lo-res laptops and desktops
	// @media (min-width: 801px)

	// For laptops and desktops, and landscape big tablets
	// @media (min-width: 1000px)

	// Full HD laptops & desktops, big tablets
	// @media (min-width: 1920px)

	// 4K screens
	// @media (min-width: 1400px)

</style>
