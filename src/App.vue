<template>
  <div id="app">
    <div id="nav" class="material-shadow">
      <div class="links">
        <router-link to="/">Home</router-link>
        <router-link to="/about">About</router-link>
        <router-link to="/disclaimer">Disclaimer</router-link>
      </div>
      <div class="logo">
        <p>
          <span class="bold">ER</span>
          <span class="light">prices</span>
        </p>
      </div>
    </div>
    <router-view/>
  </div>
</template>

<style lang="sass">

$logo-blue: #0C479D
$logo-red: #e80000

$gradient-blue-1: #0575E6
$gradient-blue-2: #021B79

$gradient-orange-1: #ff9966
$gradient-orange-2: #ff5e62

html, body
  margin: 0
  padding: 20px 0

  // height: 100%
  width: 100vw

  background: fixed linear-gradient(45deg, $gradient-blue-1, $gradient-blue-2)

// Reset for mobile browsers
h1, h2, h3, h4, h5, h6
  font-weight: normal

#app

  font-family: Arial, sans-serif, 'IBM Plex Sans','Quicksand'
  -webkit-font-smoothing: antialiased
  -moz-osx-font-smoothing: grayscale
  color: #555
  width: 90vw
  margin: 0 auto

.material-shadow

  font-family: 'IBM Plex Sans'
  font-weight: 700
  background: #fff
  border-radius: 15px
  box-shadow: 0 8px 60px rgba(0, 0, 0, 0.2), 0 6px 25px rgba(0, 0, 0, 0.15)
  padding: 20px
  margin: 40px 0

#nav

  // width: 90%

  margin: 0 auto
  padding: 20px

  display: flex
  align-items: center
  justify-content: space-between
  flex-direction: column-reverse

  .links

    font-family: 'IBM Plex Sans'

    width: 100%

    display: flex
    align-items: center
    justify-content: space-around

    a

      color: #555
      text-decoration: none
      font-weight: bold

  .logo

    padding: 0
    margin: 0

    p
      font-size: 40px
      font-family: 'Quicksand', sans-serif

      height: 100%
      padding: 0
      margin: 20px

    .bold

      font-weight: 700
      color: $logo-red

    .light

      font-weight: 300
      color: $logo-blue

// smartphones, portrait iPhone, portrait 480x320 phones (Android)
// @media (min-width: 280px)

// Higher resolution portrait mobile devices
// @media (min-width: 400px)

// Landscape iPhones
// @media (min-width: 568px)

// Portrait iPad
@media (min-width: 750px)

  #nav

    flex-direction: row
    justify-content: space-between
    padding: 20px 40px
    margin: 0 auto

    .links, .logo

      width: 49%

    .links

      justify-content: flex-start

      a

        padding: 0 25px

    .logo

      text-align: right

    .links

      a

        padding: 0 30px

// Landscape standard tablets, lo-res laptops and desktops
// @media (min-width: 801px)

// For laptops and desktops, and landscape big tablets
// @media (min-width: 1000px)

// Full HD laptops & desktops, big tablets
// @media (min-width: 1920px)

// 4K screens
// @media (min-width: 1400px)

</style>
