<template>
  <div id="app">
    <div id="nav">
      <div class="links">
        <router-link to="/">Home</router-link>
        <router-link to="/about">About</router-link>
        <router-link to="/disclaimer">Disclaimer</router-link>
      </div>
      <div class="logo">
        <p>
          <span class="bold">ER</span>
          <span class="llight">prices</span>
        </p>
      </div>
    </div>
    <router-view/>
  </div>
</template>

<style lang="sass">

html, body
  margin: 0
  padding: 0

  height: 100vh
  width: 100vw

// Reset for mobile browsers
h1, h2, h3, h4, h5, h6
  font-weight: normal

#app

  font-family: Arial, sans-serif, 'IBM Plex Sans','Quicksand'
  -webkit-font-smoothing: antialiased
  -moz-osx-font-smoothing: grayscale
  color: #0C479D

#nav

  width: 90%

  margin: 20px auto
  padding: 20px 0

  // border: solid red

  display: flex
  align-items: center
  justify-content: space-between
  flex-direction: column-reverse

  border-radius: 15px
  box-shadow: 0 8px 60px rgba(12, 71, 157, 0.2), 0 6px 25px rgba(12, 71, 157, 0.15)

  .links

    font-family: 'IBM Plex Sans'

    width: 100%

    display: flex
    align-items: center
    justify-content: space-around

    a

      color: #0C479D
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
      // border: solid red


    .bold

      font-weight: 700
      color: #e80000

    .light

      font-weight: 300
      color: #0C479D

// smartphones, portrait iPhone, portrait 480x320 phones (Android)
// @media (min-width: 280px)

// Higher resolution portrait mobile devices
// @media (min-width: 400px)

// Landscape iPhones
@media (min-width: 568px)

  #nav

    flex-direction: row
    justify-content: space-between
    width: 85%
    padding: 20px 40px
    margin: 40px auto

    .links, .logo

      width: 49%

    .links

      justify-content: flex-start

      a

        padding: 0 25px

    .logo

      text-align: right

// Portrait iPad
@media (min-width: 750px)

  #nav

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
